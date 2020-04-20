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
$ docker pull mongo@sha256:045361cdccd20938baa5bf22c9723a58d6d1b2eef3e1b23da2f5c70fb290f14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:72605ac8f0e09e7d8e6d69b9d0d3dde9ed5e84cd5deb137e5d3837f38bfcde49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165705537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42dda7e6bc6222f7de7237406270b2f52108e259310d7f02325defa09d0622`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:01 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 16:53:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 16:53:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:21 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:21 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:21 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:22 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7c01deb0621cbc504ab4cd9a51f5cfd311c99c6283f34c785e34c27bfa9752`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e9a4da5d56fae7ffdc2014b07002f0b83c6faf6956e5eff6e52eabd1a62fea`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc013520249edbb1f93602cd7c0f85f27646a70eff47a785afaa3112bed02a09`  
		Last Modified: Fri, 17 Apr 2020 16:55:13 GMT  
		Size: 117.3 MB (117252470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73dc6946a91f0e64b73ad829cb40e9f18b747fee8e3919d203e5aa500386c46`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3565d572e9e93f03d67971f15464511edfeb4802e68bd02a9175086684e8c74d`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ebba12325ca3dd44ed64e37282f89f3b6b96f05cedc07211eade2f2d5bdb692e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155117398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c4d808467ed2b02b1c3c20e96d1cc1b3fb09ce15029d3170111d04d4905c6b6`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:49:55 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 10:49:57 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:49:59 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:00 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 10:50:01 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 10:50:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:50:30 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:50:33 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:50:34 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09ff957da76e3766bc42870ef6c3936782468071ab32545383cd5f3fe36680a`  
		Last Modified: Fri, 17 Apr 2020 10:53:26 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e5946587eedd6b644ef1e71eaf75d5273efa801ba469194729a9884dbe6d3b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae9b246bbc4b906da52fce7cd47318a0b610075484a28b1b128aec7774e24c6`  
		Last Modified: Fri, 17 Apr 2020 10:53:55 GMT  
		Size: 111.5 MB (111459811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a9c3e5a5773a5941884258babb3ba75eddb41b0c1518fae3075206106ecf99`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa63337249a8ac2b380dc7808c39a3fc354cb79d3045f526f46b5694a7f605b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:2ad038b8029f42ac88220c0d3c6797b0809c950a4004236f9673b200be31cbc0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821606870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590a4c61c6bc30e3ed45446f0dcbe013069705ae7b56c8d5077bd028a915d099`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:36:32 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 19:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 19:49:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 19:49:09 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 19:49:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e9fa0da56ade24c3e568bf7596673f57639c7ed6cbd088c0ed192fde3668c`  
		Last Modified: Wed, 15 Apr 2020 21:11:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27b8aa174553c5d6b83ed9c1f3829422e0730424c12945debd87be96177d6f`  
		Last Modified: Wed, 15 Apr 2020 21:11:31 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae114b0c74597963b9945618fdcce5d27a13e90eb02a392f336e769e662910`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc5318f6c07b8cb2f32c160d64179040f98f5c51bb63b437e2f4488137cb85`  
		Last Modified: Wed, 15 Apr 2020 21:11:50 GMT  
		Size: 93.5 MB (93531367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123bc7931ecaa846ab9b9466beee498abb2472e7cb91d73ae9258f955afb67`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216514753240f2ef45953d11052bf0936dd93b2fe2648f4be49903b9390eb35f`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d670e752b94e4007002fde91c4f19432ea9f989c1201d858d92f738dc8dd55e`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a064905482e8ea379e7f18b4904b8f88f8d4d1d40edeb39c9931ebe4778abd67
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363529840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2f3a2adf42a0ef0b335a00a0a01d258f3c67063d0b1c0f57dbfcc502701d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:49:17 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:49:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:49:19 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 20:02:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:02:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:02:58 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:03:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32eaddbbf64e167a8d76b71c66899143004c2fbe5f4766f4426ea84e713d0ca`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c57468d4b7999565099de1a9c9f9cdb9161aae34989b35a90f9dc12817974e`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6507fbba7468665907ecbbf5780b006ad495da6e41c2af8ee7e0875bdf8f4d0`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6a89713dfdcb39ef8f35065173480d59ee8642e8a88eff0126e4a50c5640e5`  
		Last Modified: Wed, 15 Apr 2020 21:12:23 GMT  
		Size: 92.8 MB (92814634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e151825f282187bab3b65866fc4de82ddf85961391875c26f0ef432d2f98e2`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d8eec224ec973fdbdb527993fca4283fd10cd10658ec4a031ae91a53bba1f`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c341b33407da3598f93102cc41ca103e249854a941436bac2f2a741faf0cb578`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:045361cdccd20938baa5bf22c9723a58d6d1b2eef3e1b23da2f5c70fb290f14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:72605ac8f0e09e7d8e6d69b9d0d3dde9ed5e84cd5deb137e5d3837f38bfcde49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165705537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42dda7e6bc6222f7de7237406270b2f52108e259310d7f02325defa09d0622`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:01 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 16:53:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 16:53:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:21 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:21 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:21 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:22 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7c01deb0621cbc504ab4cd9a51f5cfd311c99c6283f34c785e34c27bfa9752`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e9a4da5d56fae7ffdc2014b07002f0b83c6faf6956e5eff6e52eabd1a62fea`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc013520249edbb1f93602cd7c0f85f27646a70eff47a785afaa3112bed02a09`  
		Last Modified: Fri, 17 Apr 2020 16:55:13 GMT  
		Size: 117.3 MB (117252470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73dc6946a91f0e64b73ad829cb40e9f18b747fee8e3919d203e5aa500386c46`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3565d572e9e93f03d67971f15464511edfeb4802e68bd02a9175086684e8c74d`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ebba12325ca3dd44ed64e37282f89f3b6b96f05cedc07211eade2f2d5bdb692e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155117398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c4d808467ed2b02b1c3c20e96d1cc1b3fb09ce15029d3170111d04d4905c6b6`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:49:55 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 10:49:57 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:49:59 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:00 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 10:50:01 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 10:50:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:50:30 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:50:33 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:50:34 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09ff957da76e3766bc42870ef6c3936782468071ab32545383cd5f3fe36680a`  
		Last Modified: Fri, 17 Apr 2020 10:53:26 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e5946587eedd6b644ef1e71eaf75d5273efa801ba469194729a9884dbe6d3b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae9b246bbc4b906da52fce7cd47318a0b610075484a28b1b128aec7774e24c6`  
		Last Modified: Fri, 17 Apr 2020 10:53:55 GMT  
		Size: 111.5 MB (111459811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a9c3e5a5773a5941884258babb3ba75eddb41b0c1518fae3075206106ecf99`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa63337249a8ac2b380dc7808c39a3fc354cb79d3045f526f46b5694a7f605b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:2ad038b8029f42ac88220c0d3c6797b0809c950a4004236f9673b200be31cbc0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821606870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590a4c61c6bc30e3ed45446f0dcbe013069705ae7b56c8d5077bd028a915d099`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:36:32 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 19:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 19:49:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 19:49:09 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 19:49:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e9fa0da56ade24c3e568bf7596673f57639c7ed6cbd088c0ed192fde3668c`  
		Last Modified: Wed, 15 Apr 2020 21:11:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27b8aa174553c5d6b83ed9c1f3829422e0730424c12945debd87be96177d6f`  
		Last Modified: Wed, 15 Apr 2020 21:11:31 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae114b0c74597963b9945618fdcce5d27a13e90eb02a392f336e769e662910`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc5318f6c07b8cb2f32c160d64179040f98f5c51bb63b437e2f4488137cb85`  
		Last Modified: Wed, 15 Apr 2020 21:11:50 GMT  
		Size: 93.5 MB (93531367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123bc7931ecaa846ab9b9466beee498abb2472e7cb91d73ae9258f955afb67`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216514753240f2ef45953d11052bf0936dd93b2fe2648f4be49903b9390eb35f`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d670e752b94e4007002fde91c4f19432ea9f989c1201d858d92f738dc8dd55e`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a064905482e8ea379e7f18b4904b8f88f8d4d1d40edeb39c9931ebe4778abd67
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363529840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2f3a2adf42a0ef0b335a00a0a01d258f3c67063d0b1c0f57dbfcc502701d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:49:17 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:49:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:49:19 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 20:02:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:02:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:02:58 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:03:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32eaddbbf64e167a8d76b71c66899143004c2fbe5f4766f4426ea84e713d0ca`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c57468d4b7999565099de1a9c9f9cdb9161aae34989b35a90f9dc12817974e`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6507fbba7468665907ecbbf5780b006ad495da6e41c2af8ee7e0875bdf8f4d0`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6a89713dfdcb39ef8f35065173480d59ee8642e8a88eff0126e4a50c5640e5`  
		Last Modified: Wed, 15 Apr 2020 21:12:23 GMT  
		Size: 92.8 MB (92814634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e151825f282187bab3b65866fc4de82ddf85961391875c26f0ef432d2f98e2`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d8eec224ec973fdbdb527993fca4283fd10cd10658ec4a031ae91a53bba1f`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c341b33407da3598f93102cc41ca103e249854a941436bac2f2a741faf0cb578`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17`

```console
$ docker pull mongo@sha256:045361cdccd20938baa5bf22c9723a58d6d1b2eef3e1b23da2f5c70fb290f14e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:3.6.17` - linux; amd64

```console
$ docker pull mongo@sha256:72605ac8f0e09e7d8e6d69b9d0d3dde9ed5e84cd5deb137e5d3837f38bfcde49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165705537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42dda7e6bc6222f7de7237406270b2f52108e259310d7f02325defa09d0622`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:01 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 16:53:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 16:53:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:21 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:21 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:21 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:22 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7c01deb0621cbc504ab4cd9a51f5cfd311c99c6283f34c785e34c27bfa9752`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e9a4da5d56fae7ffdc2014b07002f0b83c6faf6956e5eff6e52eabd1a62fea`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc013520249edbb1f93602cd7c0f85f27646a70eff47a785afaa3112bed02a09`  
		Last Modified: Fri, 17 Apr 2020 16:55:13 GMT  
		Size: 117.3 MB (117252470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73dc6946a91f0e64b73ad829cb40e9f18b747fee8e3919d203e5aa500386c46`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3565d572e9e93f03d67971f15464511edfeb4802e68bd02a9175086684e8c74d`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ebba12325ca3dd44ed64e37282f89f3b6b96f05cedc07211eade2f2d5bdb692e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155117398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c4d808467ed2b02b1c3c20e96d1cc1b3fb09ce15029d3170111d04d4905c6b6`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:49:55 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 10:49:57 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:49:59 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:00 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 10:50:01 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 10:50:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:50:30 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:50:33 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:50:34 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09ff957da76e3766bc42870ef6c3936782468071ab32545383cd5f3fe36680a`  
		Last Modified: Fri, 17 Apr 2020 10:53:26 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e5946587eedd6b644ef1e71eaf75d5273efa801ba469194729a9884dbe6d3b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae9b246bbc4b906da52fce7cd47318a0b610075484a28b1b128aec7774e24c6`  
		Last Modified: Fri, 17 Apr 2020 10:53:55 GMT  
		Size: 111.5 MB (111459811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a9c3e5a5773a5941884258babb3ba75eddb41b0c1518fae3075206106ecf99`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa63337249a8ac2b380dc7808c39a3fc354cb79d3045f526f46b5694a7f605b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:2ad038b8029f42ac88220c0d3c6797b0809c950a4004236f9673b200be31cbc0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821606870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590a4c61c6bc30e3ed45446f0dcbe013069705ae7b56c8d5077bd028a915d099`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:36:32 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 19:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 19:49:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 19:49:09 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 19:49:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e9fa0da56ade24c3e568bf7596673f57639c7ed6cbd088c0ed192fde3668c`  
		Last Modified: Wed, 15 Apr 2020 21:11:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27b8aa174553c5d6b83ed9c1f3829422e0730424c12945debd87be96177d6f`  
		Last Modified: Wed, 15 Apr 2020 21:11:31 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae114b0c74597963b9945618fdcce5d27a13e90eb02a392f336e769e662910`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc5318f6c07b8cb2f32c160d64179040f98f5c51bb63b437e2f4488137cb85`  
		Last Modified: Wed, 15 Apr 2020 21:11:50 GMT  
		Size: 93.5 MB (93531367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123bc7931ecaa846ab9b9466beee498abb2472e7cb91d73ae9258f955afb67`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216514753240f2ef45953d11052bf0936dd93b2fe2648f4be49903b9390eb35f`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d670e752b94e4007002fde91c4f19432ea9f989c1201d858d92f738dc8dd55e`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a064905482e8ea379e7f18b4904b8f88f8d4d1d40edeb39c9931ebe4778abd67
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363529840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2f3a2adf42a0ef0b335a00a0a01d258f3c67063d0b1c0f57dbfcc502701d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:49:17 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:49:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:49:19 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 20:02:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:02:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:02:58 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:03:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32eaddbbf64e167a8d76b71c66899143004c2fbe5f4766f4426ea84e713d0ca`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c57468d4b7999565099de1a9c9f9cdb9161aae34989b35a90f9dc12817974e`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6507fbba7468665907ecbbf5780b006ad495da6e41c2af8ee7e0875bdf8f4d0`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6a89713dfdcb39ef8f35065173480d59ee8642e8a88eff0126e4a50c5640e5`  
		Last Modified: Wed, 15 Apr 2020 21:12:23 GMT  
		Size: 92.8 MB (92814634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e151825f282187bab3b65866fc4de82ddf85961391875c26f0ef432d2f98e2`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d8eec224ec973fdbdb527993fca4283fd10cd10658ec4a031ae91a53bba1f`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c341b33407da3598f93102cc41ca103e249854a941436bac2f2a741faf0cb578`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17-windowsservercore`

```console
$ docker pull mongo@sha256:cc192d5019217acb5b5d9782f46a0341abe17c7d8bfa58df28b16e95cf8ff4f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:3.6.17-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:2ad038b8029f42ac88220c0d3c6797b0809c950a4004236f9673b200be31cbc0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821606870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590a4c61c6bc30e3ed45446f0dcbe013069705ae7b56c8d5077bd028a915d099`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:36:32 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 19:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 19:49:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 19:49:09 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 19:49:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e9fa0da56ade24c3e568bf7596673f57639c7ed6cbd088c0ed192fde3668c`  
		Last Modified: Wed, 15 Apr 2020 21:11:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27b8aa174553c5d6b83ed9c1f3829422e0730424c12945debd87be96177d6f`  
		Last Modified: Wed, 15 Apr 2020 21:11:31 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae114b0c74597963b9945618fdcce5d27a13e90eb02a392f336e769e662910`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc5318f6c07b8cb2f32c160d64179040f98f5c51bb63b437e2f4488137cb85`  
		Last Modified: Wed, 15 Apr 2020 21:11:50 GMT  
		Size: 93.5 MB (93531367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123bc7931ecaa846ab9b9466beee498abb2472e7cb91d73ae9258f955afb67`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216514753240f2ef45953d11052bf0936dd93b2fe2648f4be49903b9390eb35f`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d670e752b94e4007002fde91c4f19432ea9f989c1201d858d92f738dc8dd55e`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a064905482e8ea379e7f18b4904b8f88f8d4d1d40edeb39c9931ebe4778abd67
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363529840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2f3a2adf42a0ef0b335a00a0a01d258f3c67063d0b1c0f57dbfcc502701d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:49:17 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:49:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:49:19 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 20:02:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:02:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:02:58 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:03:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32eaddbbf64e167a8d76b71c66899143004c2fbe5f4766f4426ea84e713d0ca`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c57468d4b7999565099de1a9c9f9cdb9161aae34989b35a90f9dc12817974e`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6507fbba7468665907ecbbf5780b006ad495da6e41c2af8ee7e0875bdf8f4d0`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6a89713dfdcb39ef8f35065173480d59ee8642e8a88eff0126e4a50c5640e5`  
		Last Modified: Wed, 15 Apr 2020 21:12:23 GMT  
		Size: 92.8 MB (92814634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e151825f282187bab3b65866fc4de82ddf85961391875c26f0ef432d2f98e2`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d8eec224ec973fdbdb527993fca4283fd10cd10658ec4a031ae91a53bba1f`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c341b33407da3598f93102cc41ca103e249854a941436bac2f2a741faf0cb578`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17-windowsservercore-1809`

```console
$ docker pull mongo@sha256:6a86515bb0970d7b80e2ab33ee2cb21e5f63a231d47a0eaf708dfe13b491127b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `mongo:3.6.17-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a064905482e8ea379e7f18b4904b8f88f8d4d1d40edeb39c9931ebe4778abd67
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363529840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2f3a2adf42a0ef0b335a00a0a01d258f3c67063d0b1c0f57dbfcc502701d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:49:17 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:49:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:49:19 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 20:02:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:02:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:02:58 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:03:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32eaddbbf64e167a8d76b71c66899143004c2fbe5f4766f4426ea84e713d0ca`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c57468d4b7999565099de1a9c9f9cdb9161aae34989b35a90f9dc12817974e`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6507fbba7468665907ecbbf5780b006ad495da6e41c2af8ee7e0875bdf8f4d0`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6a89713dfdcb39ef8f35065173480d59ee8642e8a88eff0126e4a50c5640e5`  
		Last Modified: Wed, 15 Apr 2020 21:12:23 GMT  
		Size: 92.8 MB (92814634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e151825f282187bab3b65866fc4de82ddf85961391875c26f0ef432d2f98e2`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d8eec224ec973fdbdb527993fca4283fd10cd10658ec4a031ae91a53bba1f`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c341b33407da3598f93102cc41ca103e249854a941436bac2f2a741faf0cb578`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:cf14c686fbf2088bfd778e806b278dc4a24aac8ad56f6156ff609677a7c883a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `mongo:3.6.17-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:2ad038b8029f42ac88220c0d3c6797b0809c950a4004236f9673b200be31cbc0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821606870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590a4c61c6bc30e3ed45446f0dcbe013069705ae7b56c8d5077bd028a915d099`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:36:32 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 19:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 19:49:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 19:49:09 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 19:49:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e9fa0da56ade24c3e568bf7596673f57639c7ed6cbd088c0ed192fde3668c`  
		Last Modified: Wed, 15 Apr 2020 21:11:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27b8aa174553c5d6b83ed9c1f3829422e0730424c12945debd87be96177d6f`  
		Last Modified: Wed, 15 Apr 2020 21:11:31 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae114b0c74597963b9945618fdcce5d27a13e90eb02a392f336e769e662910`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc5318f6c07b8cb2f32c160d64179040f98f5c51bb63b437e2f4488137cb85`  
		Last Modified: Wed, 15 Apr 2020 21:11:50 GMT  
		Size: 93.5 MB (93531367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123bc7931ecaa846ab9b9466beee498abb2472e7cb91d73ae9258f955afb67`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216514753240f2ef45953d11052bf0936dd93b2fe2648f4be49903b9390eb35f`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d670e752b94e4007002fde91c4f19432ea9f989c1201d858d92f738dc8dd55e`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.17-xenial`

```console
$ docker pull mongo@sha256:744ec4b7aa612862ba1f3decd18c6a08ae21fb732b3b93c1330741158529dc73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.17-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:72605ac8f0e09e7d8e6d69b9d0d3dde9ed5e84cd5deb137e5d3837f38bfcde49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165705537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42dda7e6bc6222f7de7237406270b2f52108e259310d7f02325defa09d0622`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:01 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 16:53:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 16:53:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:21 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:21 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:21 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:22 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7c01deb0621cbc504ab4cd9a51f5cfd311c99c6283f34c785e34c27bfa9752`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e9a4da5d56fae7ffdc2014b07002f0b83c6faf6956e5eff6e52eabd1a62fea`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc013520249edbb1f93602cd7c0f85f27646a70eff47a785afaa3112bed02a09`  
		Last Modified: Fri, 17 Apr 2020 16:55:13 GMT  
		Size: 117.3 MB (117252470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73dc6946a91f0e64b73ad829cb40e9f18b747fee8e3919d203e5aa500386c46`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3565d572e9e93f03d67971f15464511edfeb4802e68bd02a9175086684e8c74d`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.17-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ebba12325ca3dd44ed64e37282f89f3b6b96f05cedc07211eade2f2d5bdb692e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155117398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c4d808467ed2b02b1c3c20e96d1cc1b3fb09ce15029d3170111d04d4905c6b6`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:49:55 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 10:49:57 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:49:59 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:00 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 10:50:01 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 10:50:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:50:30 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:50:33 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:50:34 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09ff957da76e3766bc42870ef6c3936782468071ab32545383cd5f3fe36680a`  
		Last Modified: Fri, 17 Apr 2020 10:53:26 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e5946587eedd6b644ef1e71eaf75d5273efa801ba469194729a9884dbe6d3b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae9b246bbc4b906da52fce7cd47318a0b610075484a28b1b128aec7774e24c6`  
		Last Modified: Fri, 17 Apr 2020 10:53:55 GMT  
		Size: 111.5 MB (111459811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a9c3e5a5773a5941884258babb3ba75eddb41b0c1518fae3075206106ecf99`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa63337249a8ac2b380dc7808c39a3fc354cb79d3045f526f46b5694a7f605b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:cc192d5019217acb5b5d9782f46a0341abe17c7d8bfa58df28b16e95cf8ff4f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:2ad038b8029f42ac88220c0d3c6797b0809c950a4004236f9673b200be31cbc0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821606870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590a4c61c6bc30e3ed45446f0dcbe013069705ae7b56c8d5077bd028a915d099`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:36:32 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 19:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 19:49:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 19:49:09 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 19:49:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e9fa0da56ade24c3e568bf7596673f57639c7ed6cbd088c0ed192fde3668c`  
		Last Modified: Wed, 15 Apr 2020 21:11:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27b8aa174553c5d6b83ed9c1f3829422e0730424c12945debd87be96177d6f`  
		Last Modified: Wed, 15 Apr 2020 21:11:31 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae114b0c74597963b9945618fdcce5d27a13e90eb02a392f336e769e662910`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc5318f6c07b8cb2f32c160d64179040f98f5c51bb63b437e2f4488137cb85`  
		Last Modified: Wed, 15 Apr 2020 21:11:50 GMT  
		Size: 93.5 MB (93531367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123bc7931ecaa846ab9b9466beee498abb2472e7cb91d73ae9258f955afb67`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216514753240f2ef45953d11052bf0936dd93b2fe2648f4be49903b9390eb35f`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d670e752b94e4007002fde91c4f19432ea9f989c1201d858d92f738dc8dd55e`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a064905482e8ea379e7f18b4904b8f88f8d4d1d40edeb39c9931ebe4778abd67
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363529840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2f3a2adf42a0ef0b335a00a0a01d258f3c67063d0b1c0f57dbfcc502701d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:49:17 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:49:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:49:19 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 20:02:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:02:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:02:58 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:03:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32eaddbbf64e167a8d76b71c66899143004c2fbe5f4766f4426ea84e713d0ca`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c57468d4b7999565099de1a9c9f9cdb9161aae34989b35a90f9dc12817974e`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6507fbba7468665907ecbbf5780b006ad495da6e41c2af8ee7e0875bdf8f4d0`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6a89713dfdcb39ef8f35065173480d59ee8642e8a88eff0126e4a50c5640e5`  
		Last Modified: Wed, 15 Apr 2020 21:12:23 GMT  
		Size: 92.8 MB (92814634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e151825f282187bab3b65866fc4de82ddf85961391875c26f0ef432d2f98e2`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d8eec224ec973fdbdb527993fca4283fd10cd10658ec4a031ae91a53bba1f`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c341b33407da3598f93102cc41ca103e249854a941436bac2f2a741faf0cb578`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:6a86515bb0970d7b80e2ab33ee2cb21e5f63a231d47a0eaf708dfe13b491127b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a064905482e8ea379e7f18b4904b8f88f8d4d1d40edeb39c9931ebe4778abd67
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363529840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2f3a2adf42a0ef0b335a00a0a01d258f3c67063d0b1c0f57dbfcc502701d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:49:17 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:49:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:49:19 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 20:02:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:02:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:02:58 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:03:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32eaddbbf64e167a8d76b71c66899143004c2fbe5f4766f4426ea84e713d0ca`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c57468d4b7999565099de1a9c9f9cdb9161aae34989b35a90f9dc12817974e`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6507fbba7468665907ecbbf5780b006ad495da6e41c2af8ee7e0875bdf8f4d0`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6a89713dfdcb39ef8f35065173480d59ee8642e8a88eff0126e4a50c5640e5`  
		Last Modified: Wed, 15 Apr 2020 21:12:23 GMT  
		Size: 92.8 MB (92814634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e151825f282187bab3b65866fc4de82ddf85961391875c26f0ef432d2f98e2`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d8eec224ec973fdbdb527993fca4283fd10cd10658ec4a031ae91a53bba1f`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c341b33407da3598f93102cc41ca103e249854a941436bac2f2a741faf0cb578`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:cf14c686fbf2088bfd778e806b278dc4a24aac8ad56f6156ff609677a7c883a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:2ad038b8029f42ac88220c0d3c6797b0809c950a4004236f9673b200be31cbc0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821606870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590a4c61c6bc30e3ed45446f0dcbe013069705ae7b56c8d5077bd028a915d099`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:36:32 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 19:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 19:49:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 19:49:09 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 19:49:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e9fa0da56ade24c3e568bf7596673f57639c7ed6cbd088c0ed192fde3668c`  
		Last Modified: Wed, 15 Apr 2020 21:11:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27b8aa174553c5d6b83ed9c1f3829422e0730424c12945debd87be96177d6f`  
		Last Modified: Wed, 15 Apr 2020 21:11:31 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae114b0c74597963b9945618fdcce5d27a13e90eb02a392f336e769e662910`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc5318f6c07b8cb2f32c160d64179040f98f5c51bb63b437e2f4488137cb85`  
		Last Modified: Wed, 15 Apr 2020 21:11:50 GMT  
		Size: 93.5 MB (93531367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123bc7931ecaa846ab9b9466beee498abb2472e7cb91d73ae9258f955afb67`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216514753240f2ef45953d11052bf0936dd93b2fe2648f4be49903b9390eb35f`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d670e752b94e4007002fde91c4f19432ea9f989c1201d858d92f738dc8dd55e`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:744ec4b7aa612862ba1f3decd18c6a08ae21fb732b3b93c1330741158529dc73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:72605ac8f0e09e7d8e6d69b9d0d3dde9ed5e84cd5deb137e5d3837f38bfcde49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165705537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42dda7e6bc6222f7de7237406270b2f52108e259310d7f02325defa09d0622`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:01 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 16:53:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 16:53:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:21 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:21 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:21 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:22 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7c01deb0621cbc504ab4cd9a51f5cfd311c99c6283f34c785e34c27bfa9752`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e9a4da5d56fae7ffdc2014b07002f0b83c6faf6956e5eff6e52eabd1a62fea`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc013520249edbb1f93602cd7c0f85f27646a70eff47a785afaa3112bed02a09`  
		Last Modified: Fri, 17 Apr 2020 16:55:13 GMT  
		Size: 117.3 MB (117252470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73dc6946a91f0e64b73ad829cb40e9f18b747fee8e3919d203e5aa500386c46`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3565d572e9e93f03d67971f15464511edfeb4802e68bd02a9175086684e8c74d`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ebba12325ca3dd44ed64e37282f89f3b6b96f05cedc07211eade2f2d5bdb692e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155117398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c4d808467ed2b02b1c3c20e96d1cc1b3fb09ce15029d3170111d04d4905c6b6`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:49:55 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 10:49:57 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:49:59 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:00 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 10:50:01 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 10:50:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:50:30 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:50:33 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:50:34 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09ff957da76e3766bc42870ef6c3936782468071ab32545383cd5f3fe36680a`  
		Last Modified: Fri, 17 Apr 2020 10:53:26 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e5946587eedd6b644ef1e71eaf75d5273efa801ba469194729a9884dbe6d3b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae9b246bbc4b906da52fce7cd47318a0b610075484a28b1b128aec7774e24c6`  
		Last Modified: Fri, 17 Apr 2020 10:53:55 GMT  
		Size: 111.5 MB (111459811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a9c3e5a5773a5941884258babb3ba75eddb41b0c1518fae3075206106ecf99`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa63337249a8ac2b380dc7808c39a3fc354cb79d3045f526f46b5694a7f605b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:cc192d5019217acb5b5d9782f46a0341abe17c7d8bfa58df28b16e95cf8ff4f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:3-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:2ad038b8029f42ac88220c0d3c6797b0809c950a4004236f9673b200be31cbc0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821606870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590a4c61c6bc30e3ed45446f0dcbe013069705ae7b56c8d5077bd028a915d099`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:36:32 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 19:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 19:49:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 19:49:09 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 19:49:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e9fa0da56ade24c3e568bf7596673f57639c7ed6cbd088c0ed192fde3668c`  
		Last Modified: Wed, 15 Apr 2020 21:11:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27b8aa174553c5d6b83ed9c1f3829422e0730424c12945debd87be96177d6f`  
		Last Modified: Wed, 15 Apr 2020 21:11:31 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae114b0c74597963b9945618fdcce5d27a13e90eb02a392f336e769e662910`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc5318f6c07b8cb2f32c160d64179040f98f5c51bb63b437e2f4488137cb85`  
		Last Modified: Wed, 15 Apr 2020 21:11:50 GMT  
		Size: 93.5 MB (93531367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123bc7931ecaa846ab9b9466beee498abb2472e7cb91d73ae9258f955afb67`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216514753240f2ef45953d11052bf0936dd93b2fe2648f4be49903b9390eb35f`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d670e752b94e4007002fde91c4f19432ea9f989c1201d858d92f738dc8dd55e`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a064905482e8ea379e7f18b4904b8f88f8d4d1d40edeb39c9931ebe4778abd67
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363529840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2f3a2adf42a0ef0b335a00a0a01d258f3c67063d0b1c0f57dbfcc502701d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:49:17 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:49:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:49:19 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 20:02:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:02:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:02:58 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:03:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32eaddbbf64e167a8d76b71c66899143004c2fbe5f4766f4426ea84e713d0ca`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c57468d4b7999565099de1a9c9f9cdb9161aae34989b35a90f9dc12817974e`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6507fbba7468665907ecbbf5780b006ad495da6e41c2af8ee7e0875bdf8f4d0`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6a89713dfdcb39ef8f35065173480d59ee8642e8a88eff0126e4a50c5640e5`  
		Last Modified: Wed, 15 Apr 2020 21:12:23 GMT  
		Size: 92.8 MB (92814634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e151825f282187bab3b65866fc4de82ddf85961391875c26f0ef432d2f98e2`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d8eec224ec973fdbdb527993fca4283fd10cd10658ec4a031ae91a53bba1f`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c341b33407da3598f93102cc41ca103e249854a941436bac2f2a741faf0cb578`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:6a86515bb0970d7b80e2ab33ee2cb21e5f63a231d47a0eaf708dfe13b491127b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a064905482e8ea379e7f18b4904b8f88f8d4d1d40edeb39c9931ebe4778abd67
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363529840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2f3a2adf42a0ef0b335a00a0a01d258f3c67063d0b1c0f57dbfcc502701d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:49:17 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:49:18 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:49:19 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 20:02:56 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:02:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:02:58 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:03:00 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32eaddbbf64e167a8d76b71c66899143004c2fbe5f4766f4426ea84e713d0ca`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c57468d4b7999565099de1a9c9f9cdb9161aae34989b35a90f9dc12817974e`  
		Last Modified: Wed, 15 Apr 2020 21:12:07 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6507fbba7468665907ecbbf5780b006ad495da6e41c2af8ee7e0875bdf8f4d0`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6a89713dfdcb39ef8f35065173480d59ee8642e8a88eff0126e4a50c5640e5`  
		Last Modified: Wed, 15 Apr 2020 21:12:23 GMT  
		Size: 92.8 MB (92814634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e151825f282187bab3b65866fc4de82ddf85961391875c26f0ef432d2f98e2`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9d8eec224ec973fdbdb527993fca4283fd10cd10658ec4a031ae91a53bba1f`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c341b33407da3598f93102cc41ca103e249854a941436bac2f2a741faf0cb578`  
		Last Modified: Wed, 15 Apr 2020 21:12:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:cf14c686fbf2088bfd778e806b278dc4a24aac8ad56f6156ff609677a7c883a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:2ad038b8029f42ac88220c0d3c6797b0809c950a4004236f9673b200be31cbc0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5821606870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590a4c61c6bc30e3ed45446f0dcbe013069705ae7b56c8d5077bd028a915d099`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 19:36:32 GMT
ENV MONGO_VERSION=3.6.17
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.17-signed.msi
# Wed, 15 Apr 2020 19:36:33 GMT
ENV MONGO_DOWNLOAD_SHA256=b20b72d5366a7a00cb85245ebedd01b665bbac4f918dd5fac7a7c5eb68477c26
# Wed, 15 Apr 2020 19:49:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 19:49:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 19:49:09 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 19:49:10 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8e9fa0da56ade24c3e568bf7596673f57639c7ed6cbd088c0ed192fde3668c`  
		Last Modified: Wed, 15 Apr 2020 21:11:32 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e27b8aa174553c5d6b83ed9c1f3829422e0730424c12945debd87be96177d6f`  
		Last Modified: Wed, 15 Apr 2020 21:11:31 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ae114b0c74597963b9945618fdcce5d27a13e90eb02a392f336e769e662910`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bc5318f6c07b8cb2f32c160d64179040f98f5c51bb63b437e2f4488137cb85`  
		Last Modified: Wed, 15 Apr 2020 21:11:50 GMT  
		Size: 93.5 MB (93531367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb123bc7931ecaa846ab9b9466beee498abb2472e7cb91d73ae9258f955afb67`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216514753240f2ef45953d11052bf0936dd93b2fe2648f4be49903b9390eb35f`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d670e752b94e4007002fde91c4f19432ea9f989c1201d858d92f738dc8dd55e`  
		Last Modified: Wed, 15 Apr 2020 21:11:29 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:744ec4b7aa612862ba1f3decd18c6a08ae21fb732b3b93c1330741158529dc73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:72605ac8f0e09e7d8e6d69b9d0d3dde9ed5e84cd5deb137e5d3837f38bfcde49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165705537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf42dda7e6bc6222f7de7237406270b2f52108e259310d7f02325defa09d0622`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:01 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 16:53:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:02 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 16:53:02 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 16:53:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:21 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:21 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:21 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:22 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7c01deb0621cbc504ab4cd9a51f5cfd311c99c6283f34c785e34c27bfa9752`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e9a4da5d56fae7ffdc2014b07002f0b83c6faf6956e5eff6e52eabd1a62fea`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc013520249edbb1f93602cd7c0f85f27646a70eff47a785afaa3112bed02a09`  
		Last Modified: Fri, 17 Apr 2020 16:55:13 GMT  
		Size: 117.3 MB (117252470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73dc6946a91f0e64b73ad829cb40e9f18b747fee8e3919d203e5aa500386c46`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3565d572e9e93f03d67971f15464511edfeb4802e68bd02a9175086684e8c74d`  
		Last Modified: Fri, 17 Apr 2020 16:54:54 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ebba12325ca3dd44ed64e37282f89f3b6b96f05cedc07211eade2f2d5bdb692e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155117398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c4d808467ed2b02b1c3c20e96d1cc1b3fb09ce15029d3170111d04d4905c6b6`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:49:55 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 17 Apr 2020 10:49:57 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:49:58 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:49:59 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:00 GMT
ENV MONGO_MAJOR=3.6
# Fri, 17 Apr 2020 10:50:01 GMT
ENV MONGO_VERSION=3.6.17
# Fri, 17 Apr 2020 10:50:03 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:50:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:50:30 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:50:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:50:31 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:50:33 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:50:34 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09ff957da76e3766bc42870ef6c3936782468071ab32545383cd5f3fe36680a`  
		Last Modified: Fri, 17 Apr 2020 10:53:26 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e5946587eedd6b644ef1e71eaf75d5273efa801ba469194729a9884dbe6d3b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae9b246bbc4b906da52fce7cd47318a0b610075484a28b1b128aec7774e24c6`  
		Last Modified: Fri, 17 Apr 2020 10:53:55 GMT  
		Size: 111.5 MB (111459811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a9c3e5a5773a5941884258babb3ba75eddb41b0c1518fae3075206106ecf99`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa63337249a8ac2b380dc7808c39a3fc354cb79d3045f526f46b5694a7f605b`  
		Last Modified: Fri, 17 Apr 2020 10:53:25 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:0e1b5e4493ff8174be20fc5145ac09979a1b67ec4808bbedd1debfc63a9688e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:89f221f5b10932104d379821e3e1e802060b97f20a75052d5cd056f9b751d091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164593985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fddee5bccba313f4c1cbdd08b9e70aa8d712a5ba7135991d9496a9fbcacd1474`
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
# Fri, 17 Apr 2020 16:53:54 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:53:54 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:54:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:54:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:54:11 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 16:54:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:54:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:54:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 16:54:14 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:54:35 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:54:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:54:36 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:54:36 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:54:36 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:54:36 GMT
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
	-	`sha256:8cdf1eb96f71308e6f5be52c3f5278ff6de496b971e1a94d6adb60fc52b2835f`  
		Last Modified: Fri, 17 Apr 2020 16:55:51 GMT  
		Size: 5.8 MB (5824593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39c254c62945d89e0d0e07c721ca9da0ee5848ace6fd9ce95f719a6b721c2be`  
		Last Modified: Fri, 17 Apr 2020 16:55:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110f77aab367a0f38f766fa5d307186a68fdd7483177e20a62c2eee431fb244d`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e0c6e877ce94a0cd7ebe568b442b5521cca34ef2a227665ce524437adb7e3a`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a88f43fe6b6071a9a9f6f8ececf15a8ada76c539c146b6c18492f4f9515793`  
		Last Modified: Fri, 17 Apr 2020 16:56:07 GMT  
		Size: 129.1 MB (129051908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0887c944645013ce04d023545d234e4ac9d423babc4705d4aa92cd59c1c3a4d2`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fb442f2202e0015e8e7e44857411f7ff8a3819170149f6eb4ee6f252be9473`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:21576cacc788c25ca4e06e525d5b5bd2d05d59bc002799e9ef52b0bce80458ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154629734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7da1fd6e5f81854c26091beeb8fcc64131412ff213fd148d30c23f3026256`
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
# Fri, 17 Apr 2020 10:51:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:51:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:52:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:52:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:52:25 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 10:52:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 10:52:31 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 10:52:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:53:01 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:53:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:53:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:53:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:53:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:53:08 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:53:09 GMT
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
	-	`sha256:359f8ab2389dda541f4ea7175f79d4588b4d6413c675ac28d92f3dc5e270bff2`  
		Last Modified: Fri, 17 Apr 2020 10:55:02 GMT  
		Size: 5.3 MB (5345170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338168077ef84b0dd691aa474a890be2fcb5675909cc4ede618fb5e2dcf0b0d5`  
		Last Modified: Fri, 17 Apr 2020 10:55:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036835a8de4a031b2f5b0cb2db030ef5f4813b34ececb319430a10be48ad259f`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058346411dc3615748a52978f2f1cc870f0386a1bf844efec790e604b1facd13`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fc00548613112d608f2ca07314032763c4e9d9f88ea1e4520dfcd1a3d6ac11`  
		Last Modified: Fri, 17 Apr 2020 10:55:27 GMT  
		Size: 122.8 MB (122844535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0b99c4162ecfbef2b02f419ca99afbce313b66d90e66d35cc164883fcb51fc`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa203ef91e47930fcf9d9262ac7123b01816e17e76d60645144f73866a2b8450`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:a5cd8123a14b1c250fdac0cc984f4e11c491354f5d06acf2cd4823fe13cfb733
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.5 MB (160515262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a334551bf6f630002fd7039a7fcc9147ec860a1cf1185f997588888c9cb8669`
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
# Thu, 26 Mar 2020 20:32:45 GMT
ENV MONGO_VERSION=4.2.5
# Thu, 26 Mar 2020 20:32:47 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Mar 2020 20:33:29 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Mar 2020 20:33:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Mar 2020 20:33:43 GMT
VOLUME [/data/db /data/configdb]
# Thu, 26 Mar 2020 20:33:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Thu, 26 Mar 2020 20:33:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Mar 2020 20:33:44 GMT
EXPOSE 27017
# Thu, 26 Mar 2020 20:33:45 GMT
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
	-	`sha256:b0bc568f169f0973f95718b30983404f77d9ccf078535b5633160695c9e97c9f`  
		Last Modified: Thu, 26 Mar 2020 20:33:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb351a08b77478c6f6ebf863c6aa1da86c8564e6e6a8823fdbf4d08c4ffcdfe`  
		Last Modified: Thu, 26 Mar 2020 20:34:31 GMT  
		Size: 126.7 MB (126703840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2432dfcb365082baa859e0d9f787bc5ec2a80685c3a29a3e50ea483782305291`  
		Last Modified: Thu, 26 Mar 2020 20:33:57 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b24d21421c7d527eb400c331af9683edc0050b894e1b1ccfc0df8fd5e3150`  
		Last Modified: Thu, 26 Mar 2020 20:34:28 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:570b2b7dd754b690ff4a64d39ed6d8456999dbaa4ba2d2e032210b709fe888f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6184470548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1564d1a7061940dfd4f5ce6afb7fa0de74b9bb6db451a87c126735837ec3b04e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:38:53 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:38:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:38:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 20:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:56:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:56:10 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:56:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7183023bfc47b156833d099ec072e30552b6c3ae1148546c1b24fc88268d0e`  
		Last Modified: Wed, 15 Apr 2020 21:15:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5212dfec30fa94bd24d14a73aabe8b15d5892016055570da9e77f17b2789630`  
		Last Modified: Wed, 15 Apr 2020 21:15:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7c44b34050d9488b7ee9bab70c9c1f02cd97a56b385eb92d557dced23b245`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815b3fb9a5a74fc20aca81e434e7a6b2ab796275e60167058e42e5de653b8573`  
		Last Modified: Wed, 15 Apr 2020 21:16:41 GMT  
		Size: 456.4 MB (456395041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39f6d69d951d73c0273b6ad4d4f039892b653b4c4fd84773a5a8e83d880f6f`  
		Last Modified: Wed, 15 Apr 2020 21:15:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c83426ac577cfb863e9ad1ba79db0f511ed2af0c08a074b3311b5fce18517b5`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c282651ff846b3e9e55ac002cdc5b350c0771a240df7207a395c33e657a7d3`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a8a6d04d41e01dfbc02408b77bb1e0beb9ae615083fa9c04f3db3672ac6a1c02
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366414904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6829e0b0f6f84c9eca04b29189804a8c3f45c3341769abb07317d0f32bda029`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:56:25 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:56:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:56:27 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 21:10:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 21:10:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 21:10:49 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 21:10:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca88a48aaf0aa4dc4e47de49d9add2a7264dc292b980d6b3e635dcc46397f5`  
		Last Modified: Wed, 15 Apr 2020 21:17:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263290359bdaf92a5a3f2b21f333480b16c9a81fb5a8d6d0dc0215d55f763c30`  
		Last Modified: Wed, 15 Apr 2020 21:17:02 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb70be986bd93dea1f2cdeaefaffd711bb178452f30bf3f7c24a3070f0dd09a`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9249f6f6826ce0cabd70ecae3280744020a3efed1ec39974482fb3583699c79c`  
		Last Modified: Wed, 15 Apr 2020 21:17:24 GMT  
		Size: 95.7 MB (95699676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8784409f54b9047ea60e92f33a738d30d7c85d7fc71d720176c58eaa2b01`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e02c9261106941464a0c822d6761fed8c12987ca0b8e559798fefb5a79d965`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f27b03d944457cc29673c483eb6a2f76fd68ab4ead87ccc564c8b0fb83cd88`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:74a364c5a142b1887456289405b4428f6f0aa92c5955b4ff10e477ae2a7795b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:5ff4514ff351575aa37842896ea330dc14ea026f0baabddc7d7988eeda72bd3d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153661651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d82b5301d74ec719432a0521d65e6a7e4ff4e5e54a4acc789cb4e895e9f16c1`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:28 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 17 Apr 2020 16:53:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:29 GMT
ENV MONGO_MAJOR=4.0
# Fri, 17 Apr 2020 16:53:30 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 17 Apr 2020 16:53:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:49 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:49 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665eda6efe5a2ca89da71b3ec6c8008d061966135b267f56d91cb89160a709aa`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f249afb8789ebd2cd3fa3191b4cf216f2762efa63a931238da6e4d0f8be691`  
		Last Modified: Fri, 17 Apr 2020 16:55:23 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9817b982630eb9b50d91d1fb8d3421347d0e3689ced1362228a59220a12883`  
		Last Modified: Fri, 17 Apr 2020 16:55:43 GMT  
		Size: 105.2 MB (105209155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bfe96ec699c4207b7a1cbbabb525e7d2c0522c43715f911f89427ffc17e48`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f87759b290cbd65a430b16abe35549620c225a0644191b793a7cab038c4e25a`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f026723b70d0ae7f7c35631b66ed7adba1e266c8985f93d22a2ba2c758c6f501
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143300953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba4643089e4f32429988c2e9f34183c634f4af21b5934925aa1fb75e9905027`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:50:50 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 17 Apr 2020 10:50:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:50:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:50:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:56 GMT
ENV MONGO_MAJOR=4.0
# Fri, 17 Apr 2020 10:50:56 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 17 Apr 2020 10:50:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:51:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:51:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:51:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:51:40 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:51:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:51:42 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:51:43 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad6560c08cf5edb0c4757533d372b748d98a8186af4c29a26050731def381f`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da737cab03c94d1e948c418c99bdd24b7b3821afd056d5d7d2fda002ad43108`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c5136b5072aeb58868f1cff74c11edf6920d934abfcabde2766f7ee6a7afc`  
		Last Modified: Fri, 17 Apr 2020 10:54:52 GMT  
		Size: 99.6 MB (99643943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadf3f1dd44a90d33adba18db2ffd82166fd93bbbd5bcc1c6f22b53d2eca0d72`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb74b70fed112813ad277fb808749b431068193a8291e882c5a8a47bfc5f27fe`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:b6e7d94f10b514a0034e43613a7231c9205b851edcd434a220366754980e3d16
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6174608935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9204ac12d78304d62efc38d691baec06bb99ffd71ef6b6c0c7dfb33bd48abd04`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:15:31 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:15:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:15:33 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:33:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:33:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:33:44 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:33:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a6cd4c1ece17777a2c32dd239a8ba395e23c44f29e0233e281af26c9d2857d`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8b4dd88b18a52ca34aea2c9d21fc28a99db5737a9abd526f97ea9af1f38b2`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd28aa952c4558acafcc059815a66472bb0f5eb7ef0cd1d0f851b3354301b140`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3765d0be3c9c109c970bfd4e310c53d3d2d8b1006b87ec93fd9240c577fa2`  
		Last Modified: Thu, 16 Apr 2020 00:50:01 GMT  
		Size: 446.5 MB (446533412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df155fc8098cf06f4508cb44bde84bfe1d4fb867ade29aa374cd0861de8161e4`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad101aceee320e60f5dd9bba9839a069ef5d4a0ead6ad6c29b833328d2b5396`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3415fe8d1273fa9bd484bc97b45f1dc83defdc87330120c128494d264022d5b5`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:ccd97bd444338973ac143a22753e6b73a3e707a6a3edd512311a418a3e432cdb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2356541115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c9945d9fe9ca658fb0b08de9eac6736f7f9f6f6132782ad2f1a33419787310`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:33:51 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:33:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:33:53 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:47:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:47:20 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:47:21 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:47:23 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d06c5b7d240f934d1a803e7c0affb983bb556079edf76645f5ea89f3eb6ca0`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c8999ac54863eceb53a9253dd6ce7446db0ce0b49f75110116faea049b988`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c62229a21e021c6afa0a2d47c9da44bed4152a29f163402db1c46226598c62`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b6a77bfcdf682061579dbfd42fb85c94f50e2772f0492635662a42b568d11f`  
		Last Modified: Thu, 16 Apr 2020 00:50:58 GMT  
		Size: 85.8 MB (85825866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376560267143c527c9e648c8674aa8d68445b9af83e1c126daab2c89e4333d12`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be795de606456ac97d7b3b1bb6f04c78dc3623e093cc10f27ee1c445974c76bb`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c07d006bdcb6ede32d05a301be6b76d939a6d859a5149d7d7d766627e66a218`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18`

```console
$ docker pull mongo@sha256:74a364c5a142b1887456289405b4428f6f0aa92c5955b4ff10e477ae2a7795b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:4.0.18` - linux; amd64

```console
$ docker pull mongo@sha256:5ff4514ff351575aa37842896ea330dc14ea026f0baabddc7d7988eeda72bd3d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153661651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d82b5301d74ec719432a0521d65e6a7e4ff4e5e54a4acc789cb4e895e9f16c1`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:28 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 17 Apr 2020 16:53:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:29 GMT
ENV MONGO_MAJOR=4.0
# Fri, 17 Apr 2020 16:53:30 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 17 Apr 2020 16:53:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:49 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:49 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665eda6efe5a2ca89da71b3ec6c8008d061966135b267f56d91cb89160a709aa`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f249afb8789ebd2cd3fa3191b4cf216f2762efa63a931238da6e4d0f8be691`  
		Last Modified: Fri, 17 Apr 2020 16:55:23 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9817b982630eb9b50d91d1fb8d3421347d0e3689ced1362228a59220a12883`  
		Last Modified: Fri, 17 Apr 2020 16:55:43 GMT  
		Size: 105.2 MB (105209155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bfe96ec699c4207b7a1cbbabb525e7d2c0522c43715f911f89427ffc17e48`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f87759b290cbd65a430b16abe35549620c225a0644191b793a7cab038c4e25a`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f026723b70d0ae7f7c35631b66ed7adba1e266c8985f93d22a2ba2c758c6f501
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143300953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba4643089e4f32429988c2e9f34183c634f4af21b5934925aa1fb75e9905027`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:50:50 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 17 Apr 2020 10:50:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:50:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:50:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:56 GMT
ENV MONGO_MAJOR=4.0
# Fri, 17 Apr 2020 10:50:56 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 17 Apr 2020 10:50:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:51:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:51:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:51:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:51:40 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:51:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:51:42 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:51:43 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad6560c08cf5edb0c4757533d372b748d98a8186af4c29a26050731def381f`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da737cab03c94d1e948c418c99bdd24b7b3821afd056d5d7d2fda002ad43108`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c5136b5072aeb58868f1cff74c11edf6920d934abfcabde2766f7ee6a7afc`  
		Last Modified: Fri, 17 Apr 2020 10:54:52 GMT  
		Size: 99.6 MB (99643943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadf3f1dd44a90d33adba18db2ffd82166fd93bbbd5bcc1c6f22b53d2eca0d72`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb74b70fed112813ad277fb808749b431068193a8291e882c5a8a47bfc5f27fe`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:b6e7d94f10b514a0034e43613a7231c9205b851edcd434a220366754980e3d16
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6174608935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9204ac12d78304d62efc38d691baec06bb99ffd71ef6b6c0c7dfb33bd48abd04`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:15:31 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:15:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:15:33 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:33:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:33:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:33:44 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:33:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a6cd4c1ece17777a2c32dd239a8ba395e23c44f29e0233e281af26c9d2857d`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8b4dd88b18a52ca34aea2c9d21fc28a99db5737a9abd526f97ea9af1f38b2`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd28aa952c4558acafcc059815a66472bb0f5eb7ef0cd1d0f851b3354301b140`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3765d0be3c9c109c970bfd4e310c53d3d2d8b1006b87ec93fd9240c577fa2`  
		Last Modified: Thu, 16 Apr 2020 00:50:01 GMT  
		Size: 446.5 MB (446533412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df155fc8098cf06f4508cb44bde84bfe1d4fb867ade29aa374cd0861de8161e4`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad101aceee320e60f5dd9bba9839a069ef5d4a0ead6ad6c29b833328d2b5396`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3415fe8d1273fa9bd484bc97b45f1dc83defdc87330120c128494d264022d5b5`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:ccd97bd444338973ac143a22753e6b73a3e707a6a3edd512311a418a3e432cdb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2356541115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c9945d9fe9ca658fb0b08de9eac6736f7f9f6f6132782ad2f1a33419787310`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:33:51 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:33:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:33:53 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:47:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:47:20 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:47:21 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:47:23 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d06c5b7d240f934d1a803e7c0affb983bb556079edf76645f5ea89f3eb6ca0`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c8999ac54863eceb53a9253dd6ce7446db0ce0b49f75110116faea049b988`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c62229a21e021c6afa0a2d47c9da44bed4152a29f163402db1c46226598c62`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b6a77bfcdf682061579dbfd42fb85c94f50e2772f0492635662a42b568d11f`  
		Last Modified: Thu, 16 Apr 2020 00:50:58 GMT  
		Size: 85.8 MB (85825866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376560267143c527c9e648c8674aa8d68445b9af83e1c126daab2c89e4333d12`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be795de606456ac97d7b3b1bb6f04c78dc3623e093cc10f27ee1c445974c76bb`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c07d006bdcb6ede32d05a301be6b76d939a6d859a5149d7d7d766627e66a218`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18-windowsservercore`

```console
$ docker pull mongo@sha256:9ff147feebb98918c160ec6bc52c5cb7d2a6d1a2484f9509409a9caad28a9219
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:4.0.18-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:b6e7d94f10b514a0034e43613a7231c9205b851edcd434a220366754980e3d16
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6174608935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9204ac12d78304d62efc38d691baec06bb99ffd71ef6b6c0c7dfb33bd48abd04`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:15:31 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:15:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:15:33 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:33:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:33:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:33:44 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:33:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a6cd4c1ece17777a2c32dd239a8ba395e23c44f29e0233e281af26c9d2857d`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8b4dd88b18a52ca34aea2c9d21fc28a99db5737a9abd526f97ea9af1f38b2`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd28aa952c4558acafcc059815a66472bb0f5eb7ef0cd1d0f851b3354301b140`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3765d0be3c9c109c970bfd4e310c53d3d2d8b1006b87ec93fd9240c577fa2`  
		Last Modified: Thu, 16 Apr 2020 00:50:01 GMT  
		Size: 446.5 MB (446533412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df155fc8098cf06f4508cb44bde84bfe1d4fb867ade29aa374cd0861de8161e4`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad101aceee320e60f5dd9bba9839a069ef5d4a0ead6ad6c29b833328d2b5396`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3415fe8d1273fa9bd484bc97b45f1dc83defdc87330120c128494d264022d5b5`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:ccd97bd444338973ac143a22753e6b73a3e707a6a3edd512311a418a3e432cdb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2356541115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c9945d9fe9ca658fb0b08de9eac6736f7f9f6f6132782ad2f1a33419787310`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:33:51 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:33:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:33:53 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:47:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:47:20 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:47:21 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:47:23 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d06c5b7d240f934d1a803e7c0affb983bb556079edf76645f5ea89f3eb6ca0`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c8999ac54863eceb53a9253dd6ce7446db0ce0b49f75110116faea049b988`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c62229a21e021c6afa0a2d47c9da44bed4152a29f163402db1c46226598c62`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b6a77bfcdf682061579dbfd42fb85c94f50e2772f0492635662a42b568d11f`  
		Last Modified: Thu, 16 Apr 2020 00:50:58 GMT  
		Size: 85.8 MB (85825866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376560267143c527c9e648c8674aa8d68445b9af83e1c126daab2c89e4333d12`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be795de606456ac97d7b3b1bb6f04c78dc3623e093cc10f27ee1c445974c76bb`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c07d006bdcb6ede32d05a301be6b76d939a6d859a5149d7d7d766627e66a218`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a9b083f53dd089dd440cf5ed74930321789f2aa0dd617106f147df77fedcf731
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `mongo:4.0.18-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:ccd97bd444338973ac143a22753e6b73a3e707a6a3edd512311a418a3e432cdb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2356541115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c9945d9fe9ca658fb0b08de9eac6736f7f9f6f6132782ad2f1a33419787310`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:33:51 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:33:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:33:53 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:47:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:47:20 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:47:21 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:47:23 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d06c5b7d240f934d1a803e7c0affb983bb556079edf76645f5ea89f3eb6ca0`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c8999ac54863eceb53a9253dd6ce7446db0ce0b49f75110116faea049b988`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c62229a21e021c6afa0a2d47c9da44bed4152a29f163402db1c46226598c62`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b6a77bfcdf682061579dbfd42fb85c94f50e2772f0492635662a42b568d11f`  
		Last Modified: Thu, 16 Apr 2020 00:50:58 GMT  
		Size: 85.8 MB (85825866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376560267143c527c9e648c8674aa8d68445b9af83e1c126daab2c89e4333d12`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be795de606456ac97d7b3b1bb6f04c78dc3623e093cc10f27ee1c445974c76bb`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c07d006bdcb6ede32d05a301be6b76d939a6d859a5149d7d7d766627e66a218`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:a869c2a880cc57c5c93e56a9dc5ea6950b4d905471b65ecacd94c8107e225470
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `mongo:4.0.18-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:b6e7d94f10b514a0034e43613a7231c9205b851edcd434a220366754980e3d16
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6174608935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9204ac12d78304d62efc38d691baec06bb99ffd71ef6b6c0c7dfb33bd48abd04`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:15:31 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:15:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:15:33 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:33:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:33:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:33:44 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:33:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a6cd4c1ece17777a2c32dd239a8ba395e23c44f29e0233e281af26c9d2857d`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8b4dd88b18a52ca34aea2c9d21fc28a99db5737a9abd526f97ea9af1f38b2`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd28aa952c4558acafcc059815a66472bb0f5eb7ef0cd1d0f851b3354301b140`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3765d0be3c9c109c970bfd4e310c53d3d2d8b1006b87ec93fd9240c577fa2`  
		Last Modified: Thu, 16 Apr 2020 00:50:01 GMT  
		Size: 446.5 MB (446533412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df155fc8098cf06f4508cb44bde84bfe1d4fb867ade29aa374cd0861de8161e4`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad101aceee320e60f5dd9bba9839a069ef5d4a0ead6ad6c29b833328d2b5396`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3415fe8d1273fa9bd484bc97b45f1dc83defdc87330120c128494d264022d5b5`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.18-xenial`

```console
$ docker pull mongo@sha256:7d6e77fa3d16f4190ff33e17d432fe3b433ae52782ae98d498c1bc5dda27fe81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.18-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:5ff4514ff351575aa37842896ea330dc14ea026f0baabddc7d7988eeda72bd3d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153661651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d82b5301d74ec719432a0521d65e6a7e4ff4e5e54a4acc789cb4e895e9f16c1`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:28 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 17 Apr 2020 16:53:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:29 GMT
ENV MONGO_MAJOR=4.0
# Fri, 17 Apr 2020 16:53:30 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 17 Apr 2020 16:53:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:49 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:49 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665eda6efe5a2ca89da71b3ec6c8008d061966135b267f56d91cb89160a709aa`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f249afb8789ebd2cd3fa3191b4cf216f2762efa63a931238da6e4d0f8be691`  
		Last Modified: Fri, 17 Apr 2020 16:55:23 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9817b982630eb9b50d91d1fb8d3421347d0e3689ced1362228a59220a12883`  
		Last Modified: Fri, 17 Apr 2020 16:55:43 GMT  
		Size: 105.2 MB (105209155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bfe96ec699c4207b7a1cbbabb525e7d2c0522c43715f911f89427ffc17e48`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f87759b290cbd65a430b16abe35549620c225a0644191b793a7cab038c4e25a`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.18-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f026723b70d0ae7f7c35631b66ed7adba1e266c8985f93d22a2ba2c758c6f501
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143300953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba4643089e4f32429988c2e9f34183c634f4af21b5934925aa1fb75e9905027`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:50:50 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 17 Apr 2020 10:50:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:50:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:50:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:56 GMT
ENV MONGO_MAJOR=4.0
# Fri, 17 Apr 2020 10:50:56 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 17 Apr 2020 10:50:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:51:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:51:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:51:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:51:40 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:51:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:51:42 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:51:43 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad6560c08cf5edb0c4757533d372b748d98a8186af4c29a26050731def381f`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da737cab03c94d1e948c418c99bdd24b7b3821afd056d5d7d2fda002ad43108`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c5136b5072aeb58868f1cff74c11edf6920d934abfcabde2766f7ee6a7afc`  
		Last Modified: Fri, 17 Apr 2020 10:54:52 GMT  
		Size: 99.6 MB (99643943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadf3f1dd44a90d33adba18db2ffd82166fd93bbbd5bcc1c6f22b53d2eca0d72`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb74b70fed112813ad277fb808749b431068193a8291e882c5a8a47bfc5f27fe`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:9ff147feebb98918c160ec6bc52c5cb7d2a6d1a2484f9509409a9caad28a9219
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:b6e7d94f10b514a0034e43613a7231c9205b851edcd434a220366754980e3d16
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6174608935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9204ac12d78304d62efc38d691baec06bb99ffd71ef6b6c0c7dfb33bd48abd04`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:15:31 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:15:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:15:33 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:33:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:33:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:33:44 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:33:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a6cd4c1ece17777a2c32dd239a8ba395e23c44f29e0233e281af26c9d2857d`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8b4dd88b18a52ca34aea2c9d21fc28a99db5737a9abd526f97ea9af1f38b2`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd28aa952c4558acafcc059815a66472bb0f5eb7ef0cd1d0f851b3354301b140`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3765d0be3c9c109c970bfd4e310c53d3d2d8b1006b87ec93fd9240c577fa2`  
		Last Modified: Thu, 16 Apr 2020 00:50:01 GMT  
		Size: 446.5 MB (446533412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df155fc8098cf06f4508cb44bde84bfe1d4fb867ade29aa374cd0861de8161e4`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad101aceee320e60f5dd9bba9839a069ef5d4a0ead6ad6c29b833328d2b5396`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3415fe8d1273fa9bd484bc97b45f1dc83defdc87330120c128494d264022d5b5`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:ccd97bd444338973ac143a22753e6b73a3e707a6a3edd512311a418a3e432cdb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2356541115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c9945d9fe9ca658fb0b08de9eac6736f7f9f6f6132782ad2f1a33419787310`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:33:51 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:33:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:33:53 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:47:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:47:20 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:47:21 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:47:23 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d06c5b7d240f934d1a803e7c0affb983bb556079edf76645f5ea89f3eb6ca0`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c8999ac54863eceb53a9253dd6ce7446db0ce0b49f75110116faea049b988`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c62229a21e021c6afa0a2d47c9da44bed4152a29f163402db1c46226598c62`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b6a77bfcdf682061579dbfd42fb85c94f50e2772f0492635662a42b568d11f`  
		Last Modified: Thu, 16 Apr 2020 00:50:58 GMT  
		Size: 85.8 MB (85825866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376560267143c527c9e648c8674aa8d68445b9af83e1c126daab2c89e4333d12`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be795de606456ac97d7b3b1bb6f04c78dc3623e093cc10f27ee1c445974c76bb`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c07d006bdcb6ede32d05a301be6b76d939a6d859a5149d7d7d766627e66a218`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a9b083f53dd089dd440cf5ed74930321789f2aa0dd617106f147df77fedcf731
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:ccd97bd444338973ac143a22753e6b73a3e707a6a3edd512311a418a3e432cdb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2356541115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2c9945d9fe9ca658fb0b08de9eac6736f7f9f6f6132782ad2f1a33419787310`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:33:51 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:33:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:33:53 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:47:19 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:47:20 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:47:21 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:47:23 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d06c5b7d240f934d1a803e7c0affb983bb556079edf76645f5ea89f3eb6ca0`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1c8999ac54863eceb53a9253dd6ce7446db0ce0b49f75110116faea049b988`  
		Last Modified: Thu, 16 Apr 2020 00:50:27 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c62229a21e021c6afa0a2d47c9da44bed4152a29f163402db1c46226598c62`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b6a77bfcdf682061579dbfd42fb85c94f50e2772f0492635662a42b568d11f`  
		Last Modified: Thu, 16 Apr 2020 00:50:58 GMT  
		Size: 85.8 MB (85825866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376560267143c527c9e648c8674aa8d68445b9af83e1c126daab2c89e4333d12`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be795de606456ac97d7b3b1bb6f04c78dc3623e093cc10f27ee1c445974c76bb`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c07d006bdcb6ede32d05a301be6b76d939a6d859a5149d7d7d766627e66a218`  
		Last Modified: Thu, 16 Apr 2020 00:50:24 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:a869c2a880cc57c5c93e56a9dc5ea6950b4d905471b65ecacd94c8107e225470
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:b6e7d94f10b514a0034e43613a7231c9205b851edcd434a220366754980e3d16
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6174608935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9204ac12d78304d62efc38d691baec06bb99ffd71ef6b6c0c7dfb33bd48abd04`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Apr 2020 00:15:31 GMT
ENV MONGO_VERSION=4.0.18
# Thu, 16 Apr 2020 00:15:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.18-signed.msi
# Thu, 16 Apr 2020 00:15:33 GMT
ENV MONGO_DOWNLOAD_SHA256=8f326aff375480941e48852314fbfd4e4e186de6556d753cf09b890ab9241ecf
# Thu, 16 Apr 2020 00:33:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Thu, 16 Apr 2020 00:33:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Apr 2020 00:33:44 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 00:33:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a6cd4c1ece17777a2c32dd239a8ba395e23c44f29e0233e281af26c9d2857d`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8b4dd88b18a52ca34aea2c9d21fc28a99db5737a9abd526f97ea9af1f38b2`  
		Last Modified: Thu, 16 Apr 2020 00:48:37 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd28aa952c4558acafcc059815a66472bb0f5eb7ef0cd1d0f851b3354301b140`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3765d0be3c9c109c970bfd4e310c53d3d2d8b1006b87ec93fd9240c577fa2`  
		Last Modified: Thu, 16 Apr 2020 00:50:01 GMT  
		Size: 446.5 MB (446533412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df155fc8098cf06f4508cb44bde84bfe1d4fb867ade29aa374cd0861de8161e4`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad101aceee320e60f5dd9bba9839a069ef5d4a0ead6ad6c29b833328d2b5396`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3415fe8d1273fa9bd484bc97b45f1dc83defdc87330120c128494d264022d5b5`  
		Last Modified: Thu, 16 Apr 2020 00:48:34 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:7d6e77fa3d16f4190ff33e17d432fe3b433ae52782ae98d498c1bc5dda27fe81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:5ff4514ff351575aa37842896ea330dc14ea026f0baabddc7d7988eeda72bd3d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.7 MB (153661651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d82b5301d74ec719432a0521d65e6a7e4ff4e5e54a4acc789cb4e895e9f16c1`
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
# Fri, 17 Apr 2020 16:52:33 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:52:33 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:53:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:53:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:53:28 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 17 Apr 2020 16:53:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:53:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:53:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:29 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:53:29 GMT
ENV MONGO_MAJOR=4.0
# Fri, 17 Apr 2020 16:53:30 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 17 Apr 2020 16:53:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:53:47 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:53:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:53:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:53:48 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:53:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:53:49 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:53:49 GMT
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
	-	`sha256:67a4fc8b9ac596e924ec523f4f913cec4c02bf316c82fab3b22c51e25d54d638`  
		Last Modified: Fri, 17 Apr 2020 16:54:56 GMT  
		Size: 1.3 MB (1305292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2afe62084c30f7e3e50835c0b6462b1f995eb96ec333987aaf1d2ee4db6157`  
		Last Modified: Fri, 17 Apr 2020 16:54:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665eda6efe5a2ca89da71b3ec6c8008d061966135b267f56d91cb89160a709aa`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f249afb8789ebd2cd3fa3191b4cf216f2762efa63a931238da6e4d0f8be691`  
		Last Modified: Fri, 17 Apr 2020 16:55:23 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9817b982630eb9b50d91d1fb8d3421347d0e3689ced1362228a59220a12883`  
		Last Modified: Fri, 17 Apr 2020 16:55:43 GMT  
		Size: 105.2 MB (105209155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52bfe96ec699c4207b7a1cbbabb525e7d2c0522c43715f911f89427ffc17e48`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f87759b290cbd65a430b16abe35549620c225a0644191b793a7cab038c4e25a`  
		Last Modified: Fri, 17 Apr 2020 16:55:24 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f026723b70d0ae7f7c35631b66ed7adba1e266c8985f93d22a2ba2c758c6f501
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143300953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba4643089e4f32429988c2e9f34183c634f4af21b5934925aa1fb75e9905027`
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
# Fri, 17 Apr 2020 10:48:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:48:17 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:49:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:49:54 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:50:50 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 17 Apr 2020 10:50:53 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:50:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:50:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:50:56 GMT
ENV MONGO_MAJOR=4.0
# Fri, 17 Apr 2020 10:50:56 GMT
ENV MONGO_VERSION=4.0.18
# Fri, 17 Apr 2020 10:50:59 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:51:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:51:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:51:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:51:40 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:51:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:51:42 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:51:43 GMT
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
	-	`sha256:670e78efbc635a9e0e0c24eb73ca42ed30de0e568902e47126a95f7d49cca566`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 1.2 MB (1232292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbc249fd535624ac715fdcd4d6c45bb8b2b7da8579860a23ca50d7f0f9fe055`  
		Last Modified: Fri, 17 Apr 2020 10:53:30 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad6560c08cf5edb0c4757533d372b748d98a8186af4c29a26050731def381f`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da737cab03c94d1e948c418c99bdd24b7b3821afd056d5d7d2fda002ad43108`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5c5136b5072aeb58868f1cff74c11edf6920d934abfcabde2766f7ee6a7afc`  
		Last Modified: Fri, 17 Apr 2020 10:54:52 GMT  
		Size: 99.6 MB (99643943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadf3f1dd44a90d33adba18db2ffd82166fd93bbbd5bcc1c6f22b53d2eca0d72`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb74b70fed112813ad277fb808749b431068193a8291e882c5a8a47bfc5f27fe`  
		Last Modified: Fri, 17 Apr 2020 10:54:04 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:0e1b5e4493ff8174be20fc5145ac09979a1b67ec4808bbedd1debfc63a9688e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:89f221f5b10932104d379821e3e1e802060b97f20a75052d5cd056f9b751d091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164593985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fddee5bccba313f4c1cbdd08b9e70aa8d712a5ba7135991d9496a9fbcacd1474`
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
# Fri, 17 Apr 2020 16:53:54 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:53:54 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:54:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:54:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:54:11 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 16:54:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:54:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:54:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 16:54:14 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:54:35 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:54:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:54:36 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:54:36 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:54:36 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:54:36 GMT
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
	-	`sha256:8cdf1eb96f71308e6f5be52c3f5278ff6de496b971e1a94d6adb60fc52b2835f`  
		Last Modified: Fri, 17 Apr 2020 16:55:51 GMT  
		Size: 5.8 MB (5824593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39c254c62945d89e0d0e07c721ca9da0ee5848ace6fd9ce95f719a6b721c2be`  
		Last Modified: Fri, 17 Apr 2020 16:55:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110f77aab367a0f38f766fa5d307186a68fdd7483177e20a62c2eee431fb244d`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e0c6e877ce94a0cd7ebe568b442b5521cca34ef2a227665ce524437adb7e3a`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a88f43fe6b6071a9a9f6f8ececf15a8ada76c539c146b6c18492f4f9515793`  
		Last Modified: Fri, 17 Apr 2020 16:56:07 GMT  
		Size: 129.1 MB (129051908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0887c944645013ce04d023545d234e4ac9d423babc4705d4aa92cd59c1c3a4d2`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fb442f2202e0015e8e7e44857411f7ff8a3819170149f6eb4ee6f252be9473`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:21576cacc788c25ca4e06e525d5b5bd2d05d59bc002799e9ef52b0bce80458ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154629734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7da1fd6e5f81854c26091beeb8fcc64131412ff213fd148d30c23f3026256`
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
# Fri, 17 Apr 2020 10:51:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:51:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:52:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:52:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:52:25 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 10:52:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 10:52:31 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 10:52:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:53:01 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:53:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:53:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:53:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:53:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:53:08 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:53:09 GMT
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
	-	`sha256:359f8ab2389dda541f4ea7175f79d4588b4d6413c675ac28d92f3dc5e270bff2`  
		Last Modified: Fri, 17 Apr 2020 10:55:02 GMT  
		Size: 5.3 MB (5345170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338168077ef84b0dd691aa474a890be2fcb5675909cc4ede618fb5e2dcf0b0d5`  
		Last Modified: Fri, 17 Apr 2020 10:55:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036835a8de4a031b2f5b0cb2db030ef5f4813b34ececb319430a10be48ad259f`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058346411dc3615748a52978f2f1cc870f0386a1bf844efec790e604b1facd13`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fc00548613112d608f2ca07314032763c4e9d9f88ea1e4520dfcd1a3d6ac11`  
		Last Modified: Fri, 17 Apr 2020 10:55:27 GMT  
		Size: 122.8 MB (122844535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0b99c4162ecfbef2b02f419ca99afbce313b66d90e66d35cc164883fcb51fc`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa203ef91e47930fcf9d9262ac7123b01816e17e76d60645144f73866a2b8450`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; s390x

```console
$ docker pull mongo@sha256:a5cd8123a14b1c250fdac0cc984f4e11c491354f5d06acf2cd4823fe13cfb733
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.5 MB (160515262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a334551bf6f630002fd7039a7fcc9147ec860a1cf1185f997588888c9cb8669`
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
# Thu, 26 Mar 2020 20:32:45 GMT
ENV MONGO_VERSION=4.2.5
# Thu, 26 Mar 2020 20:32:47 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Mar 2020 20:33:29 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Mar 2020 20:33:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Mar 2020 20:33:43 GMT
VOLUME [/data/db /data/configdb]
# Thu, 26 Mar 2020 20:33:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Thu, 26 Mar 2020 20:33:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Mar 2020 20:33:44 GMT
EXPOSE 27017
# Thu, 26 Mar 2020 20:33:45 GMT
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
	-	`sha256:b0bc568f169f0973f95718b30983404f77d9ccf078535b5633160695c9e97c9f`  
		Last Modified: Thu, 26 Mar 2020 20:33:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb351a08b77478c6f6ebf863c6aa1da86c8564e6e6a8823fdbf4d08c4ffcdfe`  
		Last Modified: Thu, 26 Mar 2020 20:34:31 GMT  
		Size: 126.7 MB (126703840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2432dfcb365082baa859e0d9f787bc5ec2a80685c3a29a3e50ea483782305291`  
		Last Modified: Thu, 26 Mar 2020 20:33:57 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b24d21421c7d527eb400c331af9683edc0050b894e1b1ccfc0df8fd5e3150`  
		Last Modified: Thu, 26 Mar 2020 20:34:28 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:570b2b7dd754b690ff4a64d39ed6d8456999dbaa4ba2d2e032210b709fe888f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6184470548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1564d1a7061940dfd4f5ce6afb7fa0de74b9bb6db451a87c126735837ec3b04e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:38:53 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:38:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:38:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 20:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:56:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:56:10 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:56:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7183023bfc47b156833d099ec072e30552b6c3ae1148546c1b24fc88268d0e`  
		Last Modified: Wed, 15 Apr 2020 21:15:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5212dfec30fa94bd24d14a73aabe8b15d5892016055570da9e77f17b2789630`  
		Last Modified: Wed, 15 Apr 2020 21:15:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7c44b34050d9488b7ee9bab70c9c1f02cd97a56b385eb92d557dced23b245`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815b3fb9a5a74fc20aca81e434e7a6b2ab796275e60167058e42e5de653b8573`  
		Last Modified: Wed, 15 Apr 2020 21:16:41 GMT  
		Size: 456.4 MB (456395041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39f6d69d951d73c0273b6ad4d4f039892b653b4c4fd84773a5a8e83d880f6f`  
		Last Modified: Wed, 15 Apr 2020 21:15:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c83426ac577cfb863e9ad1ba79db0f511ed2af0c08a074b3311b5fce18517b5`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c282651ff846b3e9e55ac002cdc5b350c0771a240df7207a395c33e657a7d3`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a8a6d04d41e01dfbc02408b77bb1e0beb9ae615083fa9c04f3db3672ac6a1c02
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366414904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6829e0b0f6f84c9eca04b29189804a8c3f45c3341769abb07317d0f32bda029`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:56:25 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:56:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:56:27 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 21:10:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 21:10:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 21:10:49 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 21:10:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca88a48aaf0aa4dc4e47de49d9add2a7264dc292b980d6b3e635dcc46397f5`  
		Last Modified: Wed, 15 Apr 2020 21:17:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263290359bdaf92a5a3f2b21f333480b16c9a81fb5a8d6d0dc0215d55f763c30`  
		Last Modified: Wed, 15 Apr 2020 21:17:02 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb70be986bd93dea1f2cdeaefaffd711bb178452f30bf3f7c24a3070f0dd09a`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9249f6f6826ce0cabd70ecae3280744020a3efed1ec39974482fb3583699c79c`  
		Last Modified: Wed, 15 Apr 2020 21:17:24 GMT  
		Size: 95.7 MB (95699676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8784409f54b9047ea60e92f33a738d30d7c85d7fc71d720176c58eaa2b01`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e02c9261106941464a0c822d6761fed8c12987ca0b8e559798fefb5a79d965`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f27b03d944457cc29673c483eb6a2f76fd68ab4ead87ccc564c8b0fb83cd88`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.6`

**does not exist** (yet?)

## `mongo:4.2.6-bionic`

**does not exist** (yet?)

## `mongo:4.2.6-windowsservercore`

**does not exist** (yet?)

## `mongo:4.2.6-windowsservercore-1809`

**does not exist** (yet?)

## `mongo:4.2.6-windowsservercore-ltsc2016`

**does not exist** (yet?)

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:7c4f62da38f9e779ffbf3e0bd3bb2a6010074893a4459e0a548ef6d3e0e84c2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:89f221f5b10932104d379821e3e1e802060b97f20a75052d5cd056f9b751d091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164593985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fddee5bccba313f4c1cbdd08b9e70aa8d712a5ba7135991d9496a9fbcacd1474`
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
# Fri, 17 Apr 2020 16:53:54 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:53:54 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:54:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:54:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:54:11 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 16:54:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:54:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:54:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 16:54:14 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:54:35 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:54:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:54:36 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:54:36 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:54:36 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:54:36 GMT
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
	-	`sha256:8cdf1eb96f71308e6f5be52c3f5278ff6de496b971e1a94d6adb60fc52b2835f`  
		Last Modified: Fri, 17 Apr 2020 16:55:51 GMT  
		Size: 5.8 MB (5824593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39c254c62945d89e0d0e07c721ca9da0ee5848ace6fd9ce95f719a6b721c2be`  
		Last Modified: Fri, 17 Apr 2020 16:55:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110f77aab367a0f38f766fa5d307186a68fdd7483177e20a62c2eee431fb244d`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e0c6e877ce94a0cd7ebe568b442b5521cca34ef2a227665ce524437adb7e3a`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a88f43fe6b6071a9a9f6f8ececf15a8ada76c539c146b6c18492f4f9515793`  
		Last Modified: Fri, 17 Apr 2020 16:56:07 GMT  
		Size: 129.1 MB (129051908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0887c944645013ce04d023545d234e4ac9d423babc4705d4aa92cd59c1c3a4d2`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fb442f2202e0015e8e7e44857411f7ff8a3819170149f6eb4ee6f252be9473`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:21576cacc788c25ca4e06e525d5b5bd2d05d59bc002799e9ef52b0bce80458ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154629734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7da1fd6e5f81854c26091beeb8fcc64131412ff213fd148d30c23f3026256`
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
# Fri, 17 Apr 2020 10:51:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:51:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:52:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:52:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:52:25 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 10:52:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 10:52:31 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 10:52:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:53:01 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:53:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:53:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:53:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:53:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:53:08 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:53:09 GMT
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
	-	`sha256:359f8ab2389dda541f4ea7175f79d4588b4d6413c675ac28d92f3dc5e270bff2`  
		Last Modified: Fri, 17 Apr 2020 10:55:02 GMT  
		Size: 5.3 MB (5345170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338168077ef84b0dd691aa474a890be2fcb5675909cc4ede618fb5e2dcf0b0d5`  
		Last Modified: Fri, 17 Apr 2020 10:55:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036835a8de4a031b2f5b0cb2db030ef5f4813b34ececb319430a10be48ad259f`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058346411dc3615748a52978f2f1cc870f0386a1bf844efec790e604b1facd13`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fc00548613112d608f2ca07314032763c4e9d9f88ea1e4520dfcd1a3d6ac11`  
		Last Modified: Fri, 17 Apr 2020 10:55:27 GMT  
		Size: 122.8 MB (122844535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0b99c4162ecfbef2b02f419ca99afbce313b66d90e66d35cc164883fcb51fc`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa203ef91e47930fcf9d9262ac7123b01816e17e76d60645144f73866a2b8450`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:1c6e5703fe76550e003785ebfcadcc957764324f3fe85a225aa3116b725329b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160572665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e318ce9a859412e64d576e6faa7c7562aa06dd184456eda59837606a92ab0de`
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
# Thu, 16 Apr 2020 18:49:06 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 18:49:06 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 16 Apr 2020 18:49:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Apr 2020 18:49:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 18:49:23 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 16 Apr 2020 18:49:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 16 Apr 2020 18:49:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 16 Apr 2020 18:49:30 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 16 Apr 2020 18:49:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 16 Apr 2020 18:49:30 GMT
ENV MONGO_MAJOR=4.2
# Thu, 16 Apr 2020 18:49:30 GMT
ENV MONGO_VERSION=4.2.5
# Thu, 16 Apr 2020 18:49:31 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 16 Apr 2020 18:49:48 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 16 Apr 2020 18:49:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 16 Apr 2020 18:49:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 16 Apr 2020 18:49:52 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Thu, 16 Apr 2020 18:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 18:49:53 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 18:49:53 GMT
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
	-	`sha256:19e6e34a860b503227acfb3e159dc0b7a5c15b35be812b57f68625ef5e6d8881`  
		Last Modified: Thu, 16 Apr 2020 18:50:11 GMT  
		Size: 5.7 MB (5744726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62ba0d359bc9052f648f28cdccf1b022a7d3e83ed973559176d1cc71e3ff2f4`  
		Last Modified: Thu, 16 Apr 2020 18:50:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6aad4201de6306326277c19724581e499e991b48e2bb179d36414911b5c860`  
		Last Modified: Thu, 16 Apr 2020 18:50:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8955fd34f2c6e31809b72ccd067e6c810b20e971b2277dca55b28a81203e07b`  
		Last Modified: Thu, 16 Apr 2020 18:50:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad04994f473f9c6a68c6f5d199325ea2d2805a04f693226d2219788f14918ac9`  
		Last Modified: Thu, 16 Apr 2020 18:50:28 GMT  
		Size: 126.7 MB (126703742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb86f5dce597408b95ac76d9aea1c782b1e0ce7e89ef09193dcf81e86e4593`  
		Last Modified: Thu, 16 Apr 2020 18:50:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cee8043ce690a7034411dc0c58d4559f752c73d2ea173e122c3051b2c5db2d4`  
		Last Modified: Thu, 16 Apr 2020 18:50:24 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:b06d8c9a3afb253955f2edddb5d9fbcb1330de371673b403651bf5aec0998c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:570b2b7dd754b690ff4a64d39ed6d8456999dbaa4ba2d2e032210b709fe888f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6184470548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1564d1a7061940dfd4f5ce6afb7fa0de74b9bb6db451a87c126735837ec3b04e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:38:53 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:38:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:38:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 20:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:56:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:56:10 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:56:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7183023bfc47b156833d099ec072e30552b6c3ae1148546c1b24fc88268d0e`  
		Last Modified: Wed, 15 Apr 2020 21:15:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5212dfec30fa94bd24d14a73aabe8b15d5892016055570da9e77f17b2789630`  
		Last Modified: Wed, 15 Apr 2020 21:15:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7c44b34050d9488b7ee9bab70c9c1f02cd97a56b385eb92d557dced23b245`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815b3fb9a5a74fc20aca81e434e7a6b2ab796275e60167058e42e5de653b8573`  
		Last Modified: Wed, 15 Apr 2020 21:16:41 GMT  
		Size: 456.4 MB (456395041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39f6d69d951d73c0273b6ad4d4f039892b653b4c4fd84773a5a8e83d880f6f`  
		Last Modified: Wed, 15 Apr 2020 21:15:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c83426ac577cfb863e9ad1ba79db0f511ed2af0c08a074b3311b5fce18517b5`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c282651ff846b3e9e55ac002cdc5b350c0771a240df7207a395c33e657a7d3`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a8a6d04d41e01dfbc02408b77bb1e0beb9ae615083fa9c04f3db3672ac6a1c02
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366414904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6829e0b0f6f84c9eca04b29189804a8c3f45c3341769abb07317d0f32bda029`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:56:25 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:56:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:56:27 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 21:10:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 21:10:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 21:10:49 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 21:10:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca88a48aaf0aa4dc4e47de49d9add2a7264dc292b980d6b3e635dcc46397f5`  
		Last Modified: Wed, 15 Apr 2020 21:17:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263290359bdaf92a5a3f2b21f333480b16c9a81fb5a8d6d0dc0215d55f763c30`  
		Last Modified: Wed, 15 Apr 2020 21:17:02 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb70be986bd93dea1f2cdeaefaffd711bb178452f30bf3f7c24a3070f0dd09a`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9249f6f6826ce0cabd70ecae3280744020a3efed1ec39974482fb3583699c79c`  
		Last Modified: Wed, 15 Apr 2020 21:17:24 GMT  
		Size: 95.7 MB (95699676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8784409f54b9047ea60e92f33a738d30d7c85d7fc71d720176c58eaa2b01`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e02c9261106941464a0c822d6761fed8c12987ca0b8e559798fefb5a79d965`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f27b03d944457cc29673c483eb6a2f76fd68ab4ead87ccc564c8b0fb83cd88`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:92ecd6251e6a3b58406a7c415b651f6d2c899b2d9b89314ba0d48a3b4b89cf2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a8a6d04d41e01dfbc02408b77bb1e0beb9ae615083fa9c04f3db3672ac6a1c02
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366414904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6829e0b0f6f84c9eca04b29189804a8c3f45c3341769abb07317d0f32bda029`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:56:25 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:56:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:56:27 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 21:10:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 21:10:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 21:10:49 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 21:10:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca88a48aaf0aa4dc4e47de49d9add2a7264dc292b980d6b3e635dcc46397f5`  
		Last Modified: Wed, 15 Apr 2020 21:17:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263290359bdaf92a5a3f2b21f333480b16c9a81fb5a8d6d0dc0215d55f763c30`  
		Last Modified: Wed, 15 Apr 2020 21:17:02 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb70be986bd93dea1f2cdeaefaffd711bb178452f30bf3f7c24a3070f0dd09a`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9249f6f6826ce0cabd70ecae3280744020a3efed1ec39974482fb3583699c79c`  
		Last Modified: Wed, 15 Apr 2020 21:17:24 GMT  
		Size: 95.7 MB (95699676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8784409f54b9047ea60e92f33a738d30d7c85d7fc71d720176c58eaa2b01`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e02c9261106941464a0c822d6761fed8c12987ca0b8e559798fefb5a79d965`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f27b03d944457cc29673c483eb6a2f76fd68ab4ead87ccc564c8b0fb83cd88`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:a191a8e0f644b4ac41ed08daf87fe807896701b96fc09c6880ebc201c984c8a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:570b2b7dd754b690ff4a64d39ed6d8456999dbaa4ba2d2e032210b709fe888f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6184470548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1564d1a7061940dfd4f5ce6afb7fa0de74b9bb6db451a87c126735837ec3b04e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:38:53 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:38:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:38:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 20:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:56:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:56:10 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:56:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7183023bfc47b156833d099ec072e30552b6c3ae1148546c1b24fc88268d0e`  
		Last Modified: Wed, 15 Apr 2020 21:15:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5212dfec30fa94bd24d14a73aabe8b15d5892016055570da9e77f17b2789630`  
		Last Modified: Wed, 15 Apr 2020 21:15:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7c44b34050d9488b7ee9bab70c9c1f02cd97a56b385eb92d557dced23b245`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815b3fb9a5a74fc20aca81e434e7a6b2ab796275e60167058e42e5de653b8573`  
		Last Modified: Wed, 15 Apr 2020 21:16:41 GMT  
		Size: 456.4 MB (456395041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39f6d69d951d73c0273b6ad4d4f039892b653b4c4fd84773a5a8e83d880f6f`  
		Last Modified: Wed, 15 Apr 2020 21:15:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c83426ac577cfb863e9ad1ba79db0f511ed2af0c08a074b3311b5fce18517b5`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c282651ff846b3e9e55ac002cdc5b350c0771a240df7207a395c33e657a7d3`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:7c4f62da38f9e779ffbf3e0bd3bb2a6010074893a4459e0a548ef6d3e0e84c2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:89f221f5b10932104d379821e3e1e802060b97f20a75052d5cd056f9b751d091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164593985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fddee5bccba313f4c1cbdd08b9e70aa8d712a5ba7135991d9496a9fbcacd1474`
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
# Fri, 17 Apr 2020 16:53:54 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:53:54 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:54:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:54:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:54:11 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 16:54:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:54:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:54:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 16:54:14 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:54:35 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:54:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:54:36 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:54:36 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:54:36 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:54:36 GMT
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
	-	`sha256:8cdf1eb96f71308e6f5be52c3f5278ff6de496b971e1a94d6adb60fc52b2835f`  
		Last Modified: Fri, 17 Apr 2020 16:55:51 GMT  
		Size: 5.8 MB (5824593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39c254c62945d89e0d0e07c721ca9da0ee5848ace6fd9ce95f719a6b721c2be`  
		Last Modified: Fri, 17 Apr 2020 16:55:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110f77aab367a0f38f766fa5d307186a68fdd7483177e20a62c2eee431fb244d`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e0c6e877ce94a0cd7ebe568b442b5521cca34ef2a227665ce524437adb7e3a`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a88f43fe6b6071a9a9f6f8ececf15a8ada76c539c146b6c18492f4f9515793`  
		Last Modified: Fri, 17 Apr 2020 16:56:07 GMT  
		Size: 129.1 MB (129051908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0887c944645013ce04d023545d234e4ac9d423babc4705d4aa92cd59c1c3a4d2`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fb442f2202e0015e8e7e44857411f7ff8a3819170149f6eb4ee6f252be9473`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:21576cacc788c25ca4e06e525d5b5bd2d05d59bc002799e9ef52b0bce80458ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154629734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7da1fd6e5f81854c26091beeb8fcc64131412ff213fd148d30c23f3026256`
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
# Fri, 17 Apr 2020 10:51:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:51:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:52:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:52:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:52:25 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 10:52:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 10:52:31 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 10:52:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:53:01 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:53:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:53:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:53:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:53:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:53:08 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:53:09 GMT
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
	-	`sha256:359f8ab2389dda541f4ea7175f79d4588b4d6413c675ac28d92f3dc5e270bff2`  
		Last Modified: Fri, 17 Apr 2020 10:55:02 GMT  
		Size: 5.3 MB (5345170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338168077ef84b0dd691aa474a890be2fcb5675909cc4ede618fb5e2dcf0b0d5`  
		Last Modified: Fri, 17 Apr 2020 10:55:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036835a8de4a031b2f5b0cb2db030ef5f4813b34ececb319430a10be48ad259f`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058346411dc3615748a52978f2f1cc870f0386a1bf844efec790e604b1facd13`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fc00548613112d608f2ca07314032763c4e9d9f88ea1e4520dfcd1a3d6ac11`  
		Last Modified: Fri, 17 Apr 2020 10:55:27 GMT  
		Size: 122.8 MB (122844535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0b99c4162ecfbef2b02f419ca99afbce313b66d90e66d35cc164883fcb51fc`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa203ef91e47930fcf9d9262ac7123b01816e17e76d60645144f73866a2b8450`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:1c6e5703fe76550e003785ebfcadcc957764324f3fe85a225aa3116b725329b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160572665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e318ce9a859412e64d576e6faa7c7562aa06dd184456eda59837606a92ab0de`
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
# Thu, 16 Apr 2020 18:49:06 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 18:49:06 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 16 Apr 2020 18:49:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Apr 2020 18:49:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 18:49:23 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 16 Apr 2020 18:49:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 16 Apr 2020 18:49:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 16 Apr 2020 18:49:30 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 16 Apr 2020 18:49:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 16 Apr 2020 18:49:30 GMT
ENV MONGO_MAJOR=4.2
# Thu, 16 Apr 2020 18:49:30 GMT
ENV MONGO_VERSION=4.2.5
# Thu, 16 Apr 2020 18:49:31 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 16 Apr 2020 18:49:48 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 16 Apr 2020 18:49:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 16 Apr 2020 18:49:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 16 Apr 2020 18:49:52 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Thu, 16 Apr 2020 18:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 18:49:53 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 18:49:53 GMT
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
	-	`sha256:19e6e34a860b503227acfb3e159dc0b7a5c15b35be812b57f68625ef5e6d8881`  
		Last Modified: Thu, 16 Apr 2020 18:50:11 GMT  
		Size: 5.7 MB (5744726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62ba0d359bc9052f648f28cdccf1b022a7d3e83ed973559176d1cc71e3ff2f4`  
		Last Modified: Thu, 16 Apr 2020 18:50:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6aad4201de6306326277c19724581e499e991b48e2bb179d36414911b5c860`  
		Last Modified: Thu, 16 Apr 2020 18:50:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8955fd34f2c6e31809b72ccd067e6c810b20e971b2277dca55b28a81203e07b`  
		Last Modified: Thu, 16 Apr 2020 18:50:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad04994f473f9c6a68c6f5d199325ea2d2805a04f693226d2219788f14918ac9`  
		Last Modified: Thu, 16 Apr 2020 18:50:28 GMT  
		Size: 126.7 MB (126703742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb86f5dce597408b95ac76d9aea1c782b1e0ce7e89ef09193dcf81e86e4593`  
		Last Modified: Thu, 16 Apr 2020 18:50:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cee8043ce690a7034411dc0c58d4559f752c73d2ea173e122c3051b2c5db2d4`  
		Last Modified: Thu, 16 Apr 2020 18:50:24 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:b06d8c9a3afb253955f2edddb5d9fbcb1330de371673b403651bf5aec0998c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:4-windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:570b2b7dd754b690ff4a64d39ed6d8456999dbaa4ba2d2e032210b709fe888f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6184470548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1564d1a7061940dfd4f5ce6afb7fa0de74b9bb6db451a87c126735837ec3b04e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:38:53 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:38:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:38:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 20:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:56:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:56:10 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:56:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7183023bfc47b156833d099ec072e30552b6c3ae1148546c1b24fc88268d0e`  
		Last Modified: Wed, 15 Apr 2020 21:15:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5212dfec30fa94bd24d14a73aabe8b15d5892016055570da9e77f17b2789630`  
		Last Modified: Wed, 15 Apr 2020 21:15:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7c44b34050d9488b7ee9bab70c9c1f02cd97a56b385eb92d557dced23b245`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815b3fb9a5a74fc20aca81e434e7a6b2ab796275e60167058e42e5de653b8573`  
		Last Modified: Wed, 15 Apr 2020 21:16:41 GMT  
		Size: 456.4 MB (456395041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39f6d69d951d73c0273b6ad4d4f039892b653b4c4fd84773a5a8e83d880f6f`  
		Last Modified: Wed, 15 Apr 2020 21:15:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c83426ac577cfb863e9ad1ba79db0f511ed2af0c08a074b3311b5fce18517b5`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c282651ff846b3e9e55ac002cdc5b350c0771a240df7207a395c33e657a7d3`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a8a6d04d41e01dfbc02408b77bb1e0beb9ae615083fa9c04f3db3672ac6a1c02
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366414904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6829e0b0f6f84c9eca04b29189804a8c3f45c3341769abb07317d0f32bda029`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:56:25 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:56:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:56:27 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 21:10:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 21:10:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 21:10:49 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 21:10:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca88a48aaf0aa4dc4e47de49d9add2a7264dc292b980d6b3e635dcc46397f5`  
		Last Modified: Wed, 15 Apr 2020 21:17:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263290359bdaf92a5a3f2b21f333480b16c9a81fb5a8d6d0dc0215d55f763c30`  
		Last Modified: Wed, 15 Apr 2020 21:17:02 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb70be986bd93dea1f2cdeaefaffd711bb178452f30bf3f7c24a3070f0dd09a`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9249f6f6826ce0cabd70ecae3280744020a3efed1ec39974482fb3583699c79c`  
		Last Modified: Wed, 15 Apr 2020 21:17:24 GMT  
		Size: 95.7 MB (95699676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8784409f54b9047ea60e92f33a738d30d7c85d7fc71d720176c58eaa2b01`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e02c9261106941464a0c822d6761fed8c12987ca0b8e559798fefb5a79d965`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f27b03d944457cc29673c483eb6a2f76fd68ab4ead87ccc564c8b0fb83cd88`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:92ecd6251e6a3b58406a7c415b651f6d2c899b2d9b89314ba0d48a3b4b89cf2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a8a6d04d41e01dfbc02408b77bb1e0beb9ae615083fa9c04f3db3672ac6a1c02
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366414904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6829e0b0f6f84c9eca04b29189804a8c3f45c3341769abb07317d0f32bda029`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:56:25 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:56:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:56:27 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 21:10:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 21:10:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 21:10:49 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 21:10:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca88a48aaf0aa4dc4e47de49d9add2a7264dc292b980d6b3e635dcc46397f5`  
		Last Modified: Wed, 15 Apr 2020 21:17:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263290359bdaf92a5a3f2b21f333480b16c9a81fb5a8d6d0dc0215d55f763c30`  
		Last Modified: Wed, 15 Apr 2020 21:17:02 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb70be986bd93dea1f2cdeaefaffd711bb178452f30bf3f7c24a3070f0dd09a`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9249f6f6826ce0cabd70ecae3280744020a3efed1ec39974482fb3583699c79c`  
		Last Modified: Wed, 15 Apr 2020 21:17:24 GMT  
		Size: 95.7 MB (95699676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8784409f54b9047ea60e92f33a738d30d7c85d7fc71d720176c58eaa2b01`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e02c9261106941464a0c822d6761fed8c12987ca0b8e559798fefb5a79d965`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f27b03d944457cc29673c483eb6a2f76fd68ab4ead87ccc564c8b0fb83cd88`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:a191a8e0f644b4ac41ed08daf87fe807896701b96fc09c6880ebc201c984c8a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:570b2b7dd754b690ff4a64d39ed6d8456999dbaa4ba2d2e032210b709fe888f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6184470548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1564d1a7061940dfd4f5ce6afb7fa0de74b9bb6db451a87c126735837ec3b04e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:38:53 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:38:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:38:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 20:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:56:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:56:10 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:56:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7183023bfc47b156833d099ec072e30552b6c3ae1148546c1b24fc88268d0e`  
		Last Modified: Wed, 15 Apr 2020 21:15:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5212dfec30fa94bd24d14a73aabe8b15d5892016055570da9e77f17b2789630`  
		Last Modified: Wed, 15 Apr 2020 21:15:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7c44b34050d9488b7ee9bab70c9c1f02cd97a56b385eb92d557dced23b245`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815b3fb9a5a74fc20aca81e434e7a6b2ab796275e60167058e42e5de653b8573`  
		Last Modified: Wed, 15 Apr 2020 21:16:41 GMT  
		Size: 456.4 MB (456395041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39f6d69d951d73c0273b6ad4d4f039892b653b4c4fd84773a5a8e83d880f6f`  
		Last Modified: Wed, 15 Apr 2020 21:15:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c83426ac577cfb863e9ad1ba79db0f511ed2af0c08a074b3311b5fce18517b5`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c282651ff846b3e9e55ac002cdc5b350c0771a240df7207a395c33e657a7d3`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:7c4f62da38f9e779ffbf3e0bd3bb2a6010074893a4459e0a548ef6d3e0e84c2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:89f221f5b10932104d379821e3e1e802060b97f20a75052d5cd056f9b751d091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164593985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fddee5bccba313f4c1cbdd08b9e70aa8d712a5ba7135991d9496a9fbcacd1474`
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
# Fri, 17 Apr 2020 16:53:54 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:53:54 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:54:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:54:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:54:11 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 16:54:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:54:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:54:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 16:54:14 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:54:35 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:54:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:54:36 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:54:36 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:54:36 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:54:36 GMT
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
	-	`sha256:8cdf1eb96f71308e6f5be52c3f5278ff6de496b971e1a94d6adb60fc52b2835f`  
		Last Modified: Fri, 17 Apr 2020 16:55:51 GMT  
		Size: 5.8 MB (5824593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39c254c62945d89e0d0e07c721ca9da0ee5848ace6fd9ce95f719a6b721c2be`  
		Last Modified: Fri, 17 Apr 2020 16:55:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110f77aab367a0f38f766fa5d307186a68fdd7483177e20a62c2eee431fb244d`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e0c6e877ce94a0cd7ebe568b442b5521cca34ef2a227665ce524437adb7e3a`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a88f43fe6b6071a9a9f6f8ececf15a8ada76c539c146b6c18492f4f9515793`  
		Last Modified: Fri, 17 Apr 2020 16:56:07 GMT  
		Size: 129.1 MB (129051908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0887c944645013ce04d023545d234e4ac9d423babc4705d4aa92cd59c1c3a4d2`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fb442f2202e0015e8e7e44857411f7ff8a3819170149f6eb4ee6f252be9473`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:21576cacc788c25ca4e06e525d5b5bd2d05d59bc002799e9ef52b0bce80458ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154629734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7da1fd6e5f81854c26091beeb8fcc64131412ff213fd148d30c23f3026256`
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
# Fri, 17 Apr 2020 10:51:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:51:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:52:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:52:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:52:25 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 10:52:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 10:52:31 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 10:52:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:53:01 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:53:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:53:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:53:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:53:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:53:08 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:53:09 GMT
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
	-	`sha256:359f8ab2389dda541f4ea7175f79d4588b4d6413c675ac28d92f3dc5e270bff2`  
		Last Modified: Fri, 17 Apr 2020 10:55:02 GMT  
		Size: 5.3 MB (5345170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338168077ef84b0dd691aa474a890be2fcb5675909cc4ede618fb5e2dcf0b0d5`  
		Last Modified: Fri, 17 Apr 2020 10:55:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036835a8de4a031b2f5b0cb2db030ef5f4813b34ececb319430a10be48ad259f`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058346411dc3615748a52978f2f1cc870f0386a1bf844efec790e604b1facd13`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fc00548613112d608f2ca07314032763c4e9d9f88ea1e4520dfcd1a3d6ac11`  
		Last Modified: Fri, 17 Apr 2020 10:55:27 GMT  
		Size: 122.8 MB (122844535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0b99c4162ecfbef2b02f419ca99afbce313b66d90e66d35cc164883fcb51fc`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa203ef91e47930fcf9d9262ac7123b01816e17e76d60645144f73866a2b8450`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:1c6e5703fe76550e003785ebfcadcc957764324f3fe85a225aa3116b725329b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160572665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e318ce9a859412e64d576e6faa7c7562aa06dd184456eda59837606a92ab0de`
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
# Thu, 16 Apr 2020 18:49:06 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 18:49:06 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 16 Apr 2020 18:49:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Apr 2020 18:49:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 16 Apr 2020 18:49:23 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 16 Apr 2020 18:49:29 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 16 Apr 2020 18:49:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 16 Apr 2020 18:49:30 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 16 Apr 2020 18:49:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 16 Apr 2020 18:49:30 GMT
ENV MONGO_MAJOR=4.2
# Thu, 16 Apr 2020 18:49:30 GMT
ENV MONGO_VERSION=4.2.5
# Thu, 16 Apr 2020 18:49:31 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 16 Apr 2020 18:49:48 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 16 Apr 2020 18:49:52 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 16 Apr 2020 18:49:52 GMT
VOLUME [/data/db /data/configdb]
# Thu, 16 Apr 2020 18:49:52 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Thu, 16 Apr 2020 18:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 18:49:53 GMT
EXPOSE 27017
# Thu, 16 Apr 2020 18:49:53 GMT
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
	-	`sha256:19e6e34a860b503227acfb3e159dc0b7a5c15b35be812b57f68625ef5e6d8881`  
		Last Modified: Thu, 16 Apr 2020 18:50:11 GMT  
		Size: 5.7 MB (5744726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62ba0d359bc9052f648f28cdccf1b022a7d3e83ed973559176d1cc71e3ff2f4`  
		Last Modified: Thu, 16 Apr 2020 18:50:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6aad4201de6306326277c19724581e499e991b48e2bb179d36414911b5c860`  
		Last Modified: Thu, 16 Apr 2020 18:50:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8955fd34f2c6e31809b72ccd067e6c810b20e971b2277dca55b28a81203e07b`  
		Last Modified: Thu, 16 Apr 2020 18:50:08 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad04994f473f9c6a68c6f5d199325ea2d2805a04f693226d2219788f14918ac9`  
		Last Modified: Thu, 16 Apr 2020 18:50:28 GMT  
		Size: 126.7 MB (126703742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abb86f5dce597408b95ac76d9aea1c782b1e0ce7e89ef09193dcf81e86e4593`  
		Last Modified: Thu, 16 Apr 2020 18:50:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cee8043ce690a7034411dc0c58d4559f752c73d2ea173e122c3051b2c5db2d4`  
		Last Modified: Thu, 16 Apr 2020 18:50:24 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:0e1b5e4493ff8174be20fc5145ac09979a1b67ec4808bbedd1debfc63a9688e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:89f221f5b10932104d379821e3e1e802060b97f20a75052d5cd056f9b751d091
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164593985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fddee5bccba313f4c1cbdd08b9e70aa8d712a5ba7135991d9496a9fbcacd1474`
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
# Fri, 17 Apr 2020 16:53:54 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 16:53:54 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 16:54:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 16:54:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 16:54:11 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 16:54:12 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 16:54:12 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 16:54:13 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 16:54:13 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 16:54:14 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 16:54:35 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 16:54:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 16:54:36 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 16:54:36 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:54:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 16:54:36 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 16:54:36 GMT
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
	-	`sha256:8cdf1eb96f71308e6f5be52c3f5278ff6de496b971e1a94d6adb60fc52b2835f`  
		Last Modified: Fri, 17 Apr 2020 16:55:51 GMT  
		Size: 5.8 MB (5824593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39c254c62945d89e0d0e07c721ca9da0ee5848ace6fd9ce95f719a6b721c2be`  
		Last Modified: Fri, 17 Apr 2020 16:55:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110f77aab367a0f38f766fa5d307186a68fdd7483177e20a62c2eee431fb244d`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e0c6e877ce94a0cd7ebe568b442b5521cca34ef2a227665ce524437adb7e3a`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a88f43fe6b6071a9a9f6f8ececf15a8ada76c539c146b6c18492f4f9515793`  
		Last Modified: Fri, 17 Apr 2020 16:56:07 GMT  
		Size: 129.1 MB (129051908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0887c944645013ce04d023545d234e4ac9d423babc4705d4aa92cd59c1c3a4d2`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fb442f2202e0015e8e7e44857411f7ff8a3819170149f6eb4ee6f252be9473`  
		Last Modified: Fri, 17 Apr 2020 16:55:48 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:21576cacc788c25ca4e06e525d5b5bd2d05d59bc002799e9ef52b0bce80458ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154629734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b7da1fd6e5f81854c26091beeb8fcc64131412ff213fd148d30c23f3026256`
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
# Fri, 17 Apr 2020 10:51:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 10:51:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 17 Apr 2020 10:52:22 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 10:52:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 17 Apr 2020 10:52:25 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 17 Apr 2020 10:52:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 17 Apr 2020 10:52:29 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 17 Apr 2020 10:52:30 GMT
ENV MONGO_MAJOR=4.2
# Fri, 17 Apr 2020 10:52:31 GMT
ENV MONGO_VERSION=4.2.5
# Fri, 17 Apr 2020 10:52:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 17 Apr 2020 10:53:01 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 17 Apr 2020 10:53:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 17 Apr 2020 10:53:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 17 Apr 2020 10:53:06 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 17 Apr 2020 10:53:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:53:08 GMT
EXPOSE 27017
# Fri, 17 Apr 2020 10:53:09 GMT
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
	-	`sha256:359f8ab2389dda541f4ea7175f79d4588b4d6413c675ac28d92f3dc5e270bff2`  
		Last Modified: Fri, 17 Apr 2020 10:55:02 GMT  
		Size: 5.3 MB (5345170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338168077ef84b0dd691aa474a890be2fcb5675909cc4ede618fb5e2dcf0b0d5`  
		Last Modified: Fri, 17 Apr 2020 10:55:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036835a8de4a031b2f5b0cb2db030ef5f4813b34ececb319430a10be48ad259f`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058346411dc3615748a52978f2f1cc870f0386a1bf844efec790e604b1facd13`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fc00548613112d608f2ca07314032763c4e9d9f88ea1e4520dfcd1a3d6ac11`  
		Last Modified: Fri, 17 Apr 2020 10:55:27 GMT  
		Size: 122.8 MB (122844535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0b99c4162ecfbef2b02f419ca99afbce313b66d90e66d35cc164883fcb51fc`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa203ef91e47930fcf9d9262ac7123b01816e17e76d60645144f73866a2b8450`  
		Last Modified: Fri, 17 Apr 2020 10:54:59 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:a5cd8123a14b1c250fdac0cc984f4e11c491354f5d06acf2cd4823fe13cfb733
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.5 MB (160515262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a334551bf6f630002fd7039a7fcc9147ec860a1cf1185f997588888c9cb8669`
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
# Thu, 26 Mar 2020 20:32:45 GMT
ENV MONGO_VERSION=4.2.5
# Thu, 26 Mar 2020 20:32:47 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Mar 2020 20:33:29 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Mar 2020 20:33:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Mar 2020 20:33:43 GMT
VOLUME [/data/db /data/configdb]
# Thu, 26 Mar 2020 20:33:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Thu, 26 Mar 2020 20:33:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Mar 2020 20:33:44 GMT
EXPOSE 27017
# Thu, 26 Mar 2020 20:33:45 GMT
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
	-	`sha256:b0bc568f169f0973f95718b30983404f77d9ccf078535b5633160695c9e97c9f`  
		Last Modified: Thu, 26 Mar 2020 20:33:57 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb351a08b77478c6f6ebf863c6aa1da86c8564e6e6a8823fdbf4d08c4ffcdfe`  
		Last Modified: Thu, 26 Mar 2020 20:34:31 GMT  
		Size: 126.7 MB (126703840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2432dfcb365082baa859e0d9f787bc5ec2a80685c3a29a3e50ea483782305291`  
		Last Modified: Thu, 26 Mar 2020 20:33:57 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754b24d21421c7d527eb400c331af9683edc0050b894e1b1ccfc0df8fd5e3150`  
		Last Modified: Thu, 26 Mar 2020 20:34:28 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:570b2b7dd754b690ff4a64d39ed6d8456999dbaa4ba2d2e032210b709fe888f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6184470548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1564d1a7061940dfd4f5ce6afb7fa0de74b9bb6db451a87c126735837ec3b04e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:38:53 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:38:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:38:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 20:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:56:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:56:10 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:56:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7183023bfc47b156833d099ec072e30552b6c3ae1148546c1b24fc88268d0e`  
		Last Modified: Wed, 15 Apr 2020 21:15:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5212dfec30fa94bd24d14a73aabe8b15d5892016055570da9e77f17b2789630`  
		Last Modified: Wed, 15 Apr 2020 21:15:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7c44b34050d9488b7ee9bab70c9c1f02cd97a56b385eb92d557dced23b245`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815b3fb9a5a74fc20aca81e434e7a6b2ab796275e60167058e42e5de653b8573`  
		Last Modified: Wed, 15 Apr 2020 21:16:41 GMT  
		Size: 456.4 MB (456395041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39f6d69d951d73c0273b6ad4d4f039892b653b4c4fd84773a5a8e83d880f6f`  
		Last Modified: Wed, 15 Apr 2020 21:15:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c83426ac577cfb863e9ad1ba79db0f511ed2af0c08a074b3311b5fce18517b5`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c282651ff846b3e9e55ac002cdc5b350c0771a240df7207a395c33e657a7d3`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a8a6d04d41e01dfbc02408b77bb1e0beb9ae615083fa9c04f3db3672ac6a1c02
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366414904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6829e0b0f6f84c9eca04b29189804a8c3f45c3341769abb07317d0f32bda029`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:56:25 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:56:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:56:27 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 21:10:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 21:10:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 21:10:49 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 21:10:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca88a48aaf0aa4dc4e47de49d9add2a7264dc292b980d6b3e635dcc46397f5`  
		Last Modified: Wed, 15 Apr 2020 21:17:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263290359bdaf92a5a3f2b21f333480b16c9a81fb5a8d6d0dc0215d55f763c30`  
		Last Modified: Wed, 15 Apr 2020 21:17:02 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb70be986bd93dea1f2cdeaefaffd711bb178452f30bf3f7c24a3070f0dd09a`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9249f6f6826ce0cabd70ecae3280744020a3efed1ec39974482fb3583699c79c`  
		Last Modified: Wed, 15 Apr 2020 21:17:24 GMT  
		Size: 95.7 MB (95699676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8784409f54b9047ea60e92f33a738d30d7c85d7fc71d720176c58eaa2b01`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e02c9261106941464a0c822d6761fed8c12987ca0b8e559798fefb5a79d965`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f27b03d944457cc29673c483eb6a2f76fd68ab4ead87ccc564c8b0fb83cd88`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:b06d8c9a3afb253955f2edddb5d9fbcb1330de371673b403651bf5aec0998c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64
	-	windows version 10.0.17763.1158; amd64

### `mongo:windowsservercore` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:570b2b7dd754b690ff4a64d39ed6d8456999dbaa4ba2d2e032210b709fe888f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6184470548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1564d1a7061940dfd4f5ce6afb7fa0de74b9bb6db451a87c126735837ec3b04e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:38:53 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:38:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:38:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 20:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:56:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:56:10 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:56:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7183023bfc47b156833d099ec072e30552b6c3ae1148546c1b24fc88268d0e`  
		Last Modified: Wed, 15 Apr 2020 21:15:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5212dfec30fa94bd24d14a73aabe8b15d5892016055570da9e77f17b2789630`  
		Last Modified: Wed, 15 Apr 2020 21:15:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7c44b34050d9488b7ee9bab70c9c1f02cd97a56b385eb92d557dced23b245`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815b3fb9a5a74fc20aca81e434e7a6b2ab796275e60167058e42e5de653b8573`  
		Last Modified: Wed, 15 Apr 2020 21:16:41 GMT  
		Size: 456.4 MB (456395041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39f6d69d951d73c0273b6ad4d4f039892b653b4c4fd84773a5a8e83d880f6f`  
		Last Modified: Wed, 15 Apr 2020 21:15:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c83426ac577cfb863e9ad1ba79db0f511ed2af0c08a074b3311b5fce18517b5`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c282651ff846b3e9e55ac002cdc5b350c0771a240df7207a395c33e657a7d3`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a8a6d04d41e01dfbc02408b77bb1e0beb9ae615083fa9c04f3db3672ac6a1c02
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366414904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6829e0b0f6f84c9eca04b29189804a8c3f45c3341769abb07317d0f32bda029`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:56:25 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:56:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:56:27 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 21:10:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 21:10:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 21:10:49 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 21:10:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca88a48aaf0aa4dc4e47de49d9add2a7264dc292b980d6b3e635dcc46397f5`  
		Last Modified: Wed, 15 Apr 2020 21:17:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263290359bdaf92a5a3f2b21f333480b16c9a81fb5a8d6d0dc0215d55f763c30`  
		Last Modified: Wed, 15 Apr 2020 21:17:02 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb70be986bd93dea1f2cdeaefaffd711bb178452f30bf3f7c24a3070f0dd09a`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9249f6f6826ce0cabd70ecae3280744020a3efed1ec39974482fb3583699c79c`  
		Last Modified: Wed, 15 Apr 2020 21:17:24 GMT  
		Size: 95.7 MB (95699676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8784409f54b9047ea60e92f33a738d30d7c85d7fc71d720176c58eaa2b01`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e02c9261106941464a0c822d6761fed8c12987ca0b8e559798fefb5a79d965`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f27b03d944457cc29673c483eb6a2f76fd68ab4ead87ccc564c8b0fb83cd88`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:92ecd6251e6a3b58406a7c415b651f6d2c899b2d9b89314ba0d48a3b4b89cf2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull mongo@sha256:a8a6d04d41e01dfbc02408b77bb1e0beb9ae615083fa9c04f3db3672ac6a1c02
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2366414904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6829e0b0f6f84c9eca04b29189804a8c3f45c3341769abb07317d0f32bda029`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:56:25 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:56:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:56:27 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 21:10:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 21:10:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 21:10:49 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 21:10:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ca88a48aaf0aa4dc4e47de49d9add2a7264dc292b980d6b3e635dcc46397f5`  
		Last Modified: Wed, 15 Apr 2020 21:17:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263290359bdaf92a5a3f2b21f333480b16c9a81fb5a8d6d0dc0215d55f763c30`  
		Last Modified: Wed, 15 Apr 2020 21:17:02 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb70be986bd93dea1f2cdeaefaffd711bb178452f30bf3f7c24a3070f0dd09a`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9249f6f6826ce0cabd70ecae3280744020a3efed1ec39974482fb3583699c79c`  
		Last Modified: Wed, 15 Apr 2020 21:17:24 GMT  
		Size: 95.7 MB (95699676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffa8784409f54b9047ea60e92f33a738d30d7c85d7fc71d720176c58eaa2b01`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e02c9261106941464a0c822d6761fed8c12987ca0b8e559798fefb5a79d965`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f27b03d944457cc29673c483eb6a2f76fd68ab4ead87ccc564c8b0fb83cd88`  
		Last Modified: Wed, 15 Apr 2020 21:16:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:a191a8e0f644b4ac41ed08daf87fe807896701b96fc09c6880ebc201c984c8a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3630; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.3630; amd64

```console
$ docker pull mongo@sha256:570b2b7dd754b690ff4a64d39ed6d8456999dbaa4ba2d2e032210b709fe888f3
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6184470548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1564d1a7061940dfd4f5ce6afb7fa0de74b9bb6db451a87c126735837ec3b04e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 20:38:53 GMT
ENV MONGO_VERSION=4.2.5
# Wed, 15 Apr 2020 20:38:54 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.5-signed.msi
# Wed, 15 Apr 2020 20:38:55 GMT
ENV MONGO_DOWNLOAD_SHA256=cc46897ad51f617d1946ad1b8f2eb50d215cab1b4b2fe21fd55f6022c862c333
# Wed, 15 Apr 2020 20:56:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 20:56:09 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 15 Apr 2020 20:56:10 GMT
EXPOSE 27017
# Wed, 15 Apr 2020 20:56:11 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7183023bfc47b156833d099ec072e30552b6c3ae1148546c1b24fc88268d0e`  
		Last Modified: Wed, 15 Apr 2020 21:15:32 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5212dfec30fa94bd24d14a73aabe8b15d5892016055570da9e77f17b2789630`  
		Last Modified: Wed, 15 Apr 2020 21:15:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7c44b34050d9488b7ee9bab70c9c1f02cd97a56b385eb92d557dced23b245`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815b3fb9a5a74fc20aca81e434e7a6b2ab796275e60167058e42e5de653b8573`  
		Last Modified: Wed, 15 Apr 2020 21:16:41 GMT  
		Size: 456.4 MB (456395041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39f6d69d951d73c0273b6ad4d4f039892b653b4c4fd84773a5a8e83d880f6f`  
		Last Modified: Wed, 15 Apr 2020 21:15:30 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c83426ac577cfb863e9ad1ba79db0f511ed2af0c08a074b3311b5fce18517b5`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c282651ff846b3e9e55ac002cdc5b350c0771a240df7207a395c33e657a7d3`  
		Last Modified: Wed, 15 Apr 2020 21:15:29 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
