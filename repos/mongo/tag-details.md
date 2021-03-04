<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6.22`](#mongo3622)
-	[`mongo:3.6.22-windowsservercore`](#mongo3622-windowsservercore)
-	[`mongo:3.6.22-windowsservercore-1809`](#mongo3622-windowsservercore-1809)
-	[`mongo:3.6.22-windowsservercore-ltsc2016`](#mongo3622-windowsservercore-ltsc2016)
-	[`mongo:3.6.22-xenial`](#mongo3622-xenial)
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
-	[`mongo:4.0.23`](#mongo4023)
-	[`mongo:4.0.23-windowsservercore`](#mongo4023-windowsservercore)
-	[`mongo:4.0.23-windowsservercore-1809`](#mongo4023-windowsservercore-1809)
-	[`mongo:4.0.23-windowsservercore-ltsc2016`](#mongo4023-windowsservercore-ltsc2016)
-	[`mongo:4.0.23-xenial`](#mongo4023-xenial)
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
-	[`mongo:4.4.4`](#mongo444)
-	[`mongo:4.4.4-bionic`](#mongo444-bionic)
-	[`mongo:4.4.4-windowsservercore`](#mongo444-windowsservercore)
-	[`mongo:4.4.4-windowsservercore-1809`](#mongo444-windowsservercore-1809)
-	[`mongo:4.4.4-windowsservercore-ltsc2016`](#mongo444-windowsservercore-ltsc2016)
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
$ docker pull mongo@sha256:0220f93bacbf85c7d144ff897a1fe52355988cdf95f6b4a1874c32512dbb2d73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:559ba7ae917a2bc61e5a6f9db0e5cf7fee2d7476e38b0510a5ddf49857dd478d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168105515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38f112c708c7e021e6df678f70692f0f4bd12de810acea548afa2abfc907397`
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
# Wed, 10 Feb 2021 09:11:16 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 09:11:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 09:11:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 09:11:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 09:11:39 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:04 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:05 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:05 GMT
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
	-	`sha256:3673227c8d34012a3c301269f7f2f782c18ae0a1ead22c66f1617397df875f1f`  
		Last Modified: Wed, 10 Feb 2021 09:12:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb718560867dbef31755a4d609d12ba22ad40d40cbb61a96e9c2658bfdb9a69`  
		Last Modified: Wed, 10 Feb 2021 09:12:34 GMT  
		Size: 117.9 MB (117906979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687b7b215c21101dc39efff6804dfa08314f303b42391545e1a991df50b5d7a`  
		Last Modified: Wed, 10 Feb 2021 09:12:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858fb3568c68462a2b52be8da34c6abf8e235fa3b1da73395c372e53c22841b7`  
		Last Modified: Wed, 17 Feb 2021 00:18:15 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fbcdabb433ce5f42098fa74ce3e0ab104b32fdf00447e1e96dd5ad5249d0dda4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156577394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4d5ca53001b36c9c5a3e2c1fe3a4f3aa142ff97581a0772941efce1704b8b3`
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
# Wed, 10 Feb 2021 08:33:11 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 08:33:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 08:33:40 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 08:33:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 08:33:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:13:48 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:13:49 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:13:50 GMT
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
	-	`sha256:c2ec90551bf89c56f5b5017c497344fae7b8874179b6dbe0fc6c5892be6ea96b`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958fca2389d98e21e32b47cbd26961891e8579360598579a047eecc6f69198e5`  
		Last Modified: Wed, 10 Feb 2021 08:34:55 GMT  
		Size: 112.0 MB (112001769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bb85ddaa62dacf54a35d6285fafd99e714650243c5896ffbfbb9e6b225eee0`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05092918a6c364dc00fb0bed16c13acafb3608c565418b331b6842de2c0c9e6`  
		Last Modified: Wed, 17 Feb 2021 00:15:33 GMT  
		Size: 4.4 KB (4421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:5a430f61c497202b18ae7a0e97ed317227d829bcfe5c18bf45e7dfbbd23ae5c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6024838479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b630f6f7a4be1f38f0d1f94f84df2e4d087cd0deb897033d1900d7469ea8ad2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:28:52 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:31:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:31:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:31:40 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:31:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61b717d1f9a706845ae430543ed5dde5939411c1867026f3875e0c5b264b75`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44993eed1414d8abf5ef7dbdee0fb1c20d72acc6958254e9456618ed6e1f3a`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fc2a767f2d33f887ac80e2ebff9d37d0341a4f872777e9ece9d345c512d36`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4cf3c5b28ec9311e59e9bf4e8af64f72f31ce074452c9fda1a6ca259be80a`  
		Last Modified: Tue, 09 Feb 2021 20:53:35 GMT  
		Size: 229.8 MB (229815881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1873f15584ed0aa62a01cb048f25eeff3906fb4ee7ea167b86074e0a1f87b`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aceb808b01ed0a97d8f149068b0163e126c3c410dfcfb54fbb942377b6f2c50`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483a081e03ada01f5caf09d30a966989f429ad56833271c977a2e3cd50ddcdf`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:0220f93bacbf85c7d144ff897a1fe52355988cdf95f6b4a1874c32512dbb2d73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:559ba7ae917a2bc61e5a6f9db0e5cf7fee2d7476e38b0510a5ddf49857dd478d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168105515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38f112c708c7e021e6df678f70692f0f4bd12de810acea548afa2abfc907397`
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
# Wed, 10 Feb 2021 09:11:16 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 09:11:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 09:11:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 09:11:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 09:11:39 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:04 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:05 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:05 GMT
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
	-	`sha256:3673227c8d34012a3c301269f7f2f782c18ae0a1ead22c66f1617397df875f1f`  
		Last Modified: Wed, 10 Feb 2021 09:12:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb718560867dbef31755a4d609d12ba22ad40d40cbb61a96e9c2658bfdb9a69`  
		Last Modified: Wed, 10 Feb 2021 09:12:34 GMT  
		Size: 117.9 MB (117906979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687b7b215c21101dc39efff6804dfa08314f303b42391545e1a991df50b5d7a`  
		Last Modified: Wed, 10 Feb 2021 09:12:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858fb3568c68462a2b52be8da34c6abf8e235fa3b1da73395c372e53c22841b7`  
		Last Modified: Wed, 17 Feb 2021 00:18:15 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fbcdabb433ce5f42098fa74ce3e0ab104b32fdf00447e1e96dd5ad5249d0dda4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156577394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4d5ca53001b36c9c5a3e2c1fe3a4f3aa142ff97581a0772941efce1704b8b3`
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
# Wed, 10 Feb 2021 08:33:11 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 08:33:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 08:33:40 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 08:33:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 08:33:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:13:48 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:13:49 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:13:50 GMT
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
	-	`sha256:c2ec90551bf89c56f5b5017c497344fae7b8874179b6dbe0fc6c5892be6ea96b`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958fca2389d98e21e32b47cbd26961891e8579360598579a047eecc6f69198e5`  
		Last Modified: Wed, 10 Feb 2021 08:34:55 GMT  
		Size: 112.0 MB (112001769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bb85ddaa62dacf54a35d6285fafd99e714650243c5896ffbfbb9e6b225eee0`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05092918a6c364dc00fb0bed16c13acafb3608c565418b331b6842de2c0c9e6`  
		Last Modified: Wed, 17 Feb 2021 00:15:33 GMT  
		Size: 4.4 KB (4421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:5a430f61c497202b18ae7a0e97ed317227d829bcfe5c18bf45e7dfbbd23ae5c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6024838479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b630f6f7a4be1f38f0d1f94f84df2e4d087cd0deb897033d1900d7469ea8ad2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:28:52 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:31:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:31:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:31:40 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:31:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61b717d1f9a706845ae430543ed5dde5939411c1867026f3875e0c5b264b75`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44993eed1414d8abf5ef7dbdee0fb1c20d72acc6958254e9456618ed6e1f3a`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fc2a767f2d33f887ac80e2ebff9d37d0341a4f872777e9ece9d345c512d36`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4cf3c5b28ec9311e59e9bf4e8af64f72f31ce074452c9fda1a6ca259be80a`  
		Last Modified: Tue, 09 Feb 2021 20:53:35 GMT  
		Size: 229.8 MB (229815881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1873f15584ed0aa62a01cb048f25eeff3906fb4ee7ea167b86074e0a1f87b`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aceb808b01ed0a97d8f149068b0163e126c3c410dfcfb54fbb942377b6f2c50`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483a081e03ada01f5caf09d30a966989f429ad56833271c977a2e3cd50ddcdf`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.22`

```console
$ docker pull mongo@sha256:0220f93bacbf85c7d144ff897a1fe52355988cdf95f6b4a1874c32512dbb2d73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:3.6.22` - linux; amd64

```console
$ docker pull mongo@sha256:559ba7ae917a2bc61e5a6f9db0e5cf7fee2d7476e38b0510a5ddf49857dd478d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168105515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38f112c708c7e021e6df678f70692f0f4bd12de810acea548afa2abfc907397`
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
# Wed, 10 Feb 2021 09:11:16 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 09:11:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 09:11:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 09:11:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 09:11:39 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:04 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:05 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:05 GMT
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
	-	`sha256:3673227c8d34012a3c301269f7f2f782c18ae0a1ead22c66f1617397df875f1f`  
		Last Modified: Wed, 10 Feb 2021 09:12:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb718560867dbef31755a4d609d12ba22ad40d40cbb61a96e9c2658bfdb9a69`  
		Last Modified: Wed, 10 Feb 2021 09:12:34 GMT  
		Size: 117.9 MB (117906979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687b7b215c21101dc39efff6804dfa08314f303b42391545e1a991df50b5d7a`  
		Last Modified: Wed, 10 Feb 2021 09:12:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858fb3568c68462a2b52be8da34c6abf8e235fa3b1da73395c372e53c22841b7`  
		Last Modified: Wed, 17 Feb 2021 00:18:15 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.22` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fbcdabb433ce5f42098fa74ce3e0ab104b32fdf00447e1e96dd5ad5249d0dda4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156577394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4d5ca53001b36c9c5a3e2c1fe3a4f3aa142ff97581a0772941efce1704b8b3`
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
# Wed, 10 Feb 2021 08:33:11 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 08:33:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 08:33:40 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 08:33:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 08:33:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:13:48 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:13:49 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:13:50 GMT
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
	-	`sha256:c2ec90551bf89c56f5b5017c497344fae7b8874179b6dbe0fc6c5892be6ea96b`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958fca2389d98e21e32b47cbd26961891e8579360598579a047eecc6f69198e5`  
		Last Modified: Wed, 10 Feb 2021 08:34:55 GMT  
		Size: 112.0 MB (112001769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bb85ddaa62dacf54a35d6285fafd99e714650243c5896ffbfbb9e6b225eee0`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05092918a6c364dc00fb0bed16c13acafb3608c565418b331b6842de2c0c9e6`  
		Last Modified: Wed, 17 Feb 2021 00:15:33 GMT  
		Size: 4.4 KB (4421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.22` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.22` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:5a430f61c497202b18ae7a0e97ed317227d829bcfe5c18bf45e7dfbbd23ae5c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6024838479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b630f6f7a4be1f38f0d1f94f84df2e4d087cd0deb897033d1900d7469ea8ad2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:28:52 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:31:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:31:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:31:40 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:31:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61b717d1f9a706845ae430543ed5dde5939411c1867026f3875e0c5b264b75`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44993eed1414d8abf5ef7dbdee0fb1c20d72acc6958254e9456618ed6e1f3a`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fc2a767f2d33f887ac80e2ebff9d37d0341a4f872777e9ece9d345c512d36`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4cf3c5b28ec9311e59e9bf4e8af64f72f31ce074452c9fda1a6ca259be80a`  
		Last Modified: Tue, 09 Feb 2021 20:53:35 GMT  
		Size: 229.8 MB (229815881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1873f15584ed0aa62a01cb048f25eeff3906fb4ee7ea167b86074e0a1f87b`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aceb808b01ed0a97d8f149068b0163e126c3c410dfcfb54fbb942377b6f2c50`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483a081e03ada01f5caf09d30a966989f429ad56833271c977a2e3cd50ddcdf`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.22-windowsservercore`

```console
$ docker pull mongo@sha256:0a9aa2c38fcfd0c84118eec7a526c5b6b5209a147259e7863ca31b41f23cc741
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:3.6.22-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.22-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:5a430f61c497202b18ae7a0e97ed317227d829bcfe5c18bf45e7dfbbd23ae5c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6024838479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b630f6f7a4be1f38f0d1f94f84df2e4d087cd0deb897033d1900d7469ea8ad2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:28:52 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:31:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:31:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:31:40 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:31:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61b717d1f9a706845ae430543ed5dde5939411c1867026f3875e0c5b264b75`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44993eed1414d8abf5ef7dbdee0fb1c20d72acc6958254e9456618ed6e1f3a`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fc2a767f2d33f887ac80e2ebff9d37d0341a4f872777e9ece9d345c512d36`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4cf3c5b28ec9311e59e9bf4e8af64f72f31ce074452c9fda1a6ca259be80a`  
		Last Modified: Tue, 09 Feb 2021 20:53:35 GMT  
		Size: 229.8 MB (229815881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1873f15584ed0aa62a01cb048f25eeff3906fb4ee7ea167b86074e0a1f87b`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aceb808b01ed0a97d8f149068b0163e126c3c410dfcfb54fbb942377b6f2c50`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483a081e03ada01f5caf09d30a966989f429ad56833271c977a2e3cd50ddcdf`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.22-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0a360392b4faabc3289e601cbfde43584d571f0fabd8ea711760dba99532db13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:3.6.22-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.22-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:f36443d1b6e2caab2e607931dc4787fec3b76156bd19a8febda6714a642823fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:3.6.22-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:5a430f61c497202b18ae7a0e97ed317227d829bcfe5c18bf45e7dfbbd23ae5c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6024838479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b630f6f7a4be1f38f0d1f94f84df2e4d087cd0deb897033d1900d7469ea8ad2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:28:52 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:31:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:31:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:31:40 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:31:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61b717d1f9a706845ae430543ed5dde5939411c1867026f3875e0c5b264b75`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44993eed1414d8abf5ef7dbdee0fb1c20d72acc6958254e9456618ed6e1f3a`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fc2a767f2d33f887ac80e2ebff9d37d0341a4f872777e9ece9d345c512d36`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4cf3c5b28ec9311e59e9bf4e8af64f72f31ce074452c9fda1a6ca259be80a`  
		Last Modified: Tue, 09 Feb 2021 20:53:35 GMT  
		Size: 229.8 MB (229815881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1873f15584ed0aa62a01cb048f25eeff3906fb4ee7ea167b86074e0a1f87b`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aceb808b01ed0a97d8f149068b0163e126c3c410dfcfb54fbb942377b6f2c50`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483a081e03ada01f5caf09d30a966989f429ad56833271c977a2e3cd50ddcdf`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.22-xenial`

```console
$ docker pull mongo@sha256:0a514a1da4da907230f62b9feac783d7cfe601ea51cba33398402f171c359256
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.22-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:559ba7ae917a2bc61e5a6f9db0e5cf7fee2d7476e38b0510a5ddf49857dd478d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168105515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38f112c708c7e021e6df678f70692f0f4bd12de810acea548afa2abfc907397`
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
# Wed, 10 Feb 2021 09:11:16 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 09:11:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 09:11:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 09:11:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 09:11:39 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:04 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:05 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:05 GMT
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
	-	`sha256:3673227c8d34012a3c301269f7f2f782c18ae0a1ead22c66f1617397df875f1f`  
		Last Modified: Wed, 10 Feb 2021 09:12:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb718560867dbef31755a4d609d12ba22ad40d40cbb61a96e9c2658bfdb9a69`  
		Last Modified: Wed, 10 Feb 2021 09:12:34 GMT  
		Size: 117.9 MB (117906979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687b7b215c21101dc39efff6804dfa08314f303b42391545e1a991df50b5d7a`  
		Last Modified: Wed, 10 Feb 2021 09:12:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858fb3568c68462a2b52be8da34c6abf8e235fa3b1da73395c372e53c22841b7`  
		Last Modified: Wed, 17 Feb 2021 00:18:15 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.22-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fbcdabb433ce5f42098fa74ce3e0ab104b32fdf00447e1e96dd5ad5249d0dda4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156577394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4d5ca53001b36c9c5a3e2c1fe3a4f3aa142ff97581a0772941efce1704b8b3`
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
# Wed, 10 Feb 2021 08:33:11 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 08:33:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 08:33:40 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 08:33:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 08:33:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:13:48 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:13:49 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:13:50 GMT
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
	-	`sha256:c2ec90551bf89c56f5b5017c497344fae7b8874179b6dbe0fc6c5892be6ea96b`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958fca2389d98e21e32b47cbd26961891e8579360598579a047eecc6f69198e5`  
		Last Modified: Wed, 10 Feb 2021 08:34:55 GMT  
		Size: 112.0 MB (112001769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bb85ddaa62dacf54a35d6285fafd99e714650243c5896ffbfbb9e6b225eee0`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05092918a6c364dc00fb0bed16c13acafb3608c565418b331b6842de2c0c9e6`  
		Last Modified: Wed, 17 Feb 2021 00:15:33 GMT  
		Size: 4.4 KB (4421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:0a9aa2c38fcfd0c84118eec7a526c5b6b5209a147259e7863ca31b41f23cc741
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:5a430f61c497202b18ae7a0e97ed317227d829bcfe5c18bf45e7dfbbd23ae5c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6024838479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b630f6f7a4be1f38f0d1f94f84df2e4d087cd0deb897033d1900d7469ea8ad2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:28:52 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:31:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:31:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:31:40 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:31:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61b717d1f9a706845ae430543ed5dde5939411c1867026f3875e0c5b264b75`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44993eed1414d8abf5ef7dbdee0fb1c20d72acc6958254e9456618ed6e1f3a`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fc2a767f2d33f887ac80e2ebff9d37d0341a4f872777e9ece9d345c512d36`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4cf3c5b28ec9311e59e9bf4e8af64f72f31ce074452c9fda1a6ca259be80a`  
		Last Modified: Tue, 09 Feb 2021 20:53:35 GMT  
		Size: 229.8 MB (229815881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1873f15584ed0aa62a01cb048f25eeff3906fb4ee7ea167b86074e0a1f87b`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aceb808b01ed0a97d8f149068b0163e126c3c410dfcfb54fbb942377b6f2c50`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483a081e03ada01f5caf09d30a966989f429ad56833271c977a2e3cd50ddcdf`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0a360392b4faabc3289e601cbfde43584d571f0fabd8ea711760dba99532db13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:f36443d1b6e2caab2e607931dc4787fec3b76156bd19a8febda6714a642823fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:5a430f61c497202b18ae7a0e97ed317227d829bcfe5c18bf45e7dfbbd23ae5c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6024838479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b630f6f7a4be1f38f0d1f94f84df2e4d087cd0deb897033d1900d7469ea8ad2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:28:52 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:31:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:31:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:31:40 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:31:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61b717d1f9a706845ae430543ed5dde5939411c1867026f3875e0c5b264b75`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44993eed1414d8abf5ef7dbdee0fb1c20d72acc6958254e9456618ed6e1f3a`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fc2a767f2d33f887ac80e2ebff9d37d0341a4f872777e9ece9d345c512d36`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4cf3c5b28ec9311e59e9bf4e8af64f72f31ce074452c9fda1a6ca259be80a`  
		Last Modified: Tue, 09 Feb 2021 20:53:35 GMT  
		Size: 229.8 MB (229815881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1873f15584ed0aa62a01cb048f25eeff3906fb4ee7ea167b86074e0a1f87b`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aceb808b01ed0a97d8f149068b0163e126c3c410dfcfb54fbb942377b6f2c50`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483a081e03ada01f5caf09d30a966989f429ad56833271c977a2e3cd50ddcdf`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:0a514a1da4da907230f62b9feac783d7cfe601ea51cba33398402f171c359256
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:559ba7ae917a2bc61e5a6f9db0e5cf7fee2d7476e38b0510a5ddf49857dd478d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168105515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38f112c708c7e021e6df678f70692f0f4bd12de810acea548afa2abfc907397`
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
# Wed, 10 Feb 2021 09:11:16 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 09:11:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 09:11:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 09:11:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 09:11:39 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:04 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:05 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:05 GMT
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
	-	`sha256:3673227c8d34012a3c301269f7f2f782c18ae0a1ead22c66f1617397df875f1f`  
		Last Modified: Wed, 10 Feb 2021 09:12:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb718560867dbef31755a4d609d12ba22ad40d40cbb61a96e9c2658bfdb9a69`  
		Last Modified: Wed, 10 Feb 2021 09:12:34 GMT  
		Size: 117.9 MB (117906979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687b7b215c21101dc39efff6804dfa08314f303b42391545e1a991df50b5d7a`  
		Last Modified: Wed, 10 Feb 2021 09:12:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858fb3568c68462a2b52be8da34c6abf8e235fa3b1da73395c372e53c22841b7`  
		Last Modified: Wed, 17 Feb 2021 00:18:15 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fbcdabb433ce5f42098fa74ce3e0ab104b32fdf00447e1e96dd5ad5249d0dda4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156577394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4d5ca53001b36c9c5a3e2c1fe3a4f3aa142ff97581a0772941efce1704b8b3`
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
# Wed, 10 Feb 2021 08:33:11 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 08:33:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 08:33:40 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 08:33:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 08:33:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:13:48 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:13:49 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:13:50 GMT
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
	-	`sha256:c2ec90551bf89c56f5b5017c497344fae7b8874179b6dbe0fc6c5892be6ea96b`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958fca2389d98e21e32b47cbd26961891e8579360598579a047eecc6f69198e5`  
		Last Modified: Wed, 10 Feb 2021 08:34:55 GMT  
		Size: 112.0 MB (112001769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bb85ddaa62dacf54a35d6285fafd99e714650243c5896ffbfbb9e6b225eee0`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05092918a6c364dc00fb0bed16c13acafb3608c565418b331b6842de2c0c9e6`  
		Last Modified: Wed, 17 Feb 2021 00:15:33 GMT  
		Size: 4.4 KB (4421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:0a9aa2c38fcfd0c84118eec7a526c5b6b5209a147259e7863ca31b41f23cc741
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:3-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:5a430f61c497202b18ae7a0e97ed317227d829bcfe5c18bf45e7dfbbd23ae5c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6024838479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b630f6f7a4be1f38f0d1f94f84df2e4d087cd0deb897033d1900d7469ea8ad2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:28:52 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:31:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:31:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:31:40 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:31:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61b717d1f9a706845ae430543ed5dde5939411c1867026f3875e0c5b264b75`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44993eed1414d8abf5ef7dbdee0fb1c20d72acc6958254e9456618ed6e1f3a`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fc2a767f2d33f887ac80e2ebff9d37d0341a4f872777e9ece9d345c512d36`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4cf3c5b28ec9311e59e9bf4e8af64f72f31ce074452c9fda1a6ca259be80a`  
		Last Modified: Tue, 09 Feb 2021 20:53:35 GMT  
		Size: 229.8 MB (229815881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1873f15584ed0aa62a01cb048f25eeff3906fb4ee7ea167b86074e0a1f87b`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aceb808b01ed0a97d8f149068b0163e126c3c410dfcfb54fbb942377b6f2c50`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483a081e03ada01f5caf09d30a966989f429ad56833271c977a2e3cd50ddcdf`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0a360392b4faabc3289e601cbfde43584d571f0fabd8ea711760dba99532db13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:bdb716f867395960020da5d1738ba4bf1880fef7fbc386523af3729059e2bf76
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2668399020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679f5b34401ac83f1baff684a794d7d84555b238608f57c4c127a9f7d619027c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:26:38 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:26:39 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:26:40 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:28:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:28:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:28:41 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:28:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b157fcbe53b82633afc538ba4cdeb067ebf7f28177b3a9683c3d1e7ce9d57`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:043851a001bdd94df595c6168464bab0f64c1c8f065731d9a59b30050d462ff8`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688f25c5301f14748dd161d8a9cf3194ee728546e6f21f035099be0882edf92`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8918272371828c901e18b12b840dfe6c1deeba7bd1eb395fb4b4b48762ac5bc5`  
		Last Modified: Tue, 09 Feb 2021 20:48:54 GMT  
		Size: 229.1 MB (229122627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15ed306e4ceb60ca3e8f86891d04899daf2311cbfefc61c19f0ad2f88548e9c`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afe71f1bf221506fc9466f7ccf5d81c5de5dbcf6762c676aef0758acb9c9f17`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c902c703823609a713c38a9c384a7dd1eeaa35f8d46b6cdd85b21cd13b5ac15f`  
		Last Modified: Tue, 09 Feb 2021 20:48:06 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:f36443d1b6e2caab2e607931dc4787fec3b76156bd19a8febda6714a642823fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:5a430f61c497202b18ae7a0e97ed317227d829bcfe5c18bf45e7dfbbd23ae5c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6024838479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b630f6f7a4be1f38f0d1f94f84df2e4d087cd0deb897033d1900d7469ea8ad2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_VERSION=3.6.22
# Tue, 09 Feb 2021 20:28:51 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.22-signed.msi
# Tue, 09 Feb 2021 20:28:52 GMT
ENV MONGO_DOWNLOAD_SHA256=6a6df36f18828416d73e81533a10308eba1112a8d1c1849d05714c0e0c326d21
# Tue, 09 Feb 2021 20:31:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:31:39 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:31:40 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:31:40 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b61b717d1f9a706845ae430543ed5dde5939411c1867026f3875e0c5b264b75`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44993eed1414d8abf5ef7dbdee0fb1c20d72acc6958254e9456618ed6e1f3a`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293fc2a767f2d33f887ac80e2ebff9d37d0341a4f872777e9ece9d345c512d36`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a4cf3c5b28ec9311e59e9bf4e8af64f72f31ce074452c9fda1a6ca259be80a`  
		Last Modified: Tue, 09 Feb 2021 20:53:35 GMT  
		Size: 229.8 MB (229815881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f1873f15584ed0aa62a01cb048f25eeff3906fb4ee7ea167b86074e0a1f87b`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aceb808b01ed0a97d8f149068b0163e126c3c410dfcfb54fbb942377b6f2c50`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0483a081e03ada01f5caf09d30a966989f429ad56833271c977a2e3cd50ddcdf`  
		Last Modified: Tue, 09 Feb 2021 20:49:09 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:0a514a1da4da907230f62b9feac783d7cfe601ea51cba33398402f171c359256
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:559ba7ae917a2bc61e5a6f9db0e5cf7fee2d7476e38b0510a5ddf49857dd478d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168105515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b38f112c708c7e021e6df678f70692f0f4bd12de810acea548afa2abfc907397`
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
# Wed, 10 Feb 2021 09:11:16 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 09:11:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 09:11:38 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 09:11:39 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 09:11:39 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:04 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:05 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:05 GMT
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
	-	`sha256:3673227c8d34012a3c301269f7f2f782c18ae0a1ead22c66f1617397df875f1f`  
		Last Modified: Wed, 10 Feb 2021 09:12:15 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb718560867dbef31755a4d609d12ba22ad40d40cbb61a96e9c2658bfdb9a69`  
		Last Modified: Wed, 10 Feb 2021 09:12:34 GMT  
		Size: 117.9 MB (117906979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687b7b215c21101dc39efff6804dfa08314f303b42391545e1a991df50b5d7a`  
		Last Modified: Wed, 10 Feb 2021 09:12:16 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858fb3568c68462a2b52be8da34c6abf8e235fa3b1da73395c372e53c22841b7`  
		Last Modified: Wed, 17 Feb 2021 00:18:15 GMT  
		Size: 4.4 KB (4416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fbcdabb433ce5f42098fa74ce3e0ab104b32fdf00447e1e96dd5ad5249d0dda4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156577394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4d5ca53001b36c9c5a3e2c1fe3a4f3aa142ff97581a0772941efce1704b8b3`
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
# Wed, 10 Feb 2021 08:33:11 GMT
ENV MONGO_VERSION=3.6.22
# Wed, 10 Feb 2021 08:33:13 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 10 Feb 2021 08:33:40 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 10 Feb 2021 08:33:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 10 Feb 2021 08:33:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:13:48 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:13:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:13:49 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:13:50 GMT
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
	-	`sha256:c2ec90551bf89c56f5b5017c497344fae7b8874179b6dbe0fc6c5892be6ea96b`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958fca2389d98e21e32b47cbd26961891e8579360598579a047eecc6f69198e5`  
		Last Modified: Wed, 10 Feb 2021 08:34:55 GMT  
		Size: 112.0 MB (112001769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bb85ddaa62dacf54a35d6285fafd99e714650243c5896ffbfbb9e6b225eee0`  
		Last Modified: Wed, 10 Feb 2021 08:34:32 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05092918a6c364dc00fb0bed16c13acafb3608c565418b331b6842de2c0c9e6`  
		Last Modified: Wed, 17 Feb 2021 00:15:33 GMT  
		Size: 4.4 KB (4421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:9de54e2d0703904e5005a5c8f04cd56d83475edd8c8f441c7f3ca0c71c40c6e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:5f9f9576c14a6f2e8c0c37450ad2225bddc42f63206f47fcae55c07d3ec5a6f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175098371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8264a857eba49a59ffba446beaa10e6f3a5c5b775c78b656aee476c8dc5c426`
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
# Wed, 17 Feb 2021 00:17:20 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:17:44 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:17:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:17:45 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:45 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:46 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:46 GMT
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
	-	`sha256:ebe4a7cd312628ff7eacb3958534f8f2b9b0a257b60e5aba2f8aec2ed6efc194`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343b2aa1fbbf575c12309d7070a089d6078ef3feb189972deb66c4f00bbd3aae`  
		Last Modified: Wed, 17 Feb 2021 00:18:54 GMT  
		Size: 139.6 MB (139561770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059fcf556d9315fb2f0bf2d895ca3053f7ca80418cb072b14f4d28b37af7579c`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c03e6ca912dc9f44b28670dcd8550b4eefbf73e1ec98f8c6d9407437496fbb`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:148115913437e8cc80492ac8227d74f452df88a85f5b3c944df3333daca8a435
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167513450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdc664d8cc1ec10ee0bc6511cead7c8ed640c7668062b2b325013a8165a1dab`
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
# Wed, 17 Feb 2021 00:14:15 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:14:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:14:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:14:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:14:58 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:14:58 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:15:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:15:00 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:15:01 GMT
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
	-	`sha256:b8e66fb30288214eb4c3f674fa3eb920eb41b117dd6ebf701bb22c8e85a8a728`  
		Last Modified: Wed, 17 Feb 2021 00:15:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaf34239126e893b75ad3585d7101f72624fd924a7f9fa711edd4aef1c7361`  
		Last Modified: Wed, 17 Feb 2021 00:16:29 GMT  
		Size: 135.7 MB (135742747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc1d5f5c39bc895a9ef14486c88ea33744321b894ba89b91c87284db75d3b7`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac81acd76c1faf85f7439ff1fe66aa7f03c84f1fe98ab9b143dcd2186af9e82`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:cdf3e3a8fca1c8eebd9cfbca2966b1e03123febbcf6e93e2c88d043594d186a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169033417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baed376d89d8d4c06a45ca93bd64872fed74a308e9fc4754ced821089bdac9e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:27 GMT
ADD file:20133497018a85bea4420c8f220dd76e39b9bb25c81a331c204d7ea02d984d7d in / 
# Thu, 04 Mar 2021 02:47:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:31 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:35:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 03:35:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:35:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 03:35:57 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 03:36:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 03:36:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 03:36:10 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 03:36:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 03:36:12 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 03:36:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 03:36:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 03:36:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 03:36:36 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 03:36:36 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 03:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 03:36:36 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 03:36:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e2e05228c9769d80c0b892ff4534a82c87ffa32b4d87105d6715d02dc13b73dd`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 25.4 MB (25380798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0697554175a1fb68cbf41f1990c4b35faab0569426e5f2bc7a8931cd581b85`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c776b6e8daba94835d2c0f86fb70da1005080f579b01d72ec542c138ce380d89`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd7545e09b022408db3ed3946b9e288e773c4872e5f2677367154a873397582`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0f57759a1811b0968b2d78f0d1cd4df3c94f877527ca8d1bd95f3f763b6271`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 2.7 MB (2707952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388c8556d6c330b583a5497cffb24f1c5ede4006cd663e3be38d6b1affe29ae`  
		Last Modified: Thu, 04 Mar 2021 03:36:57 GMT  
		Size: 5.7 MB (5747242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa17efe813310ff75b305c4adceb589f19a9e36c06b9c23938a7391379897f5`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ad0db5b17d4bd1d1635be0a4ed2cba7cf1920bd3db16c4109ddf3de49a523b`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd835e634633cd70eb29b0c4e871e9b3128314f1723920b5f547230fcecedf4`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46b6820f0b0e29a4c81b31b7a59a14f241b10c3de1ff56a437d7b411fbfc53`  
		Last Modified: Thu, 04 Mar 2021 03:37:11 GMT  
		Size: 135.2 MB (135188104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82bcaf445b47eeae3d6ea2e9960e6af68d4dd6d69869d94f3652e1abf9fb7d6`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f76478d141e7e3350e47a0726491ffb3f1d6dcaadc85de60bf47d336f8ca701`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:463b14d54fb2845102072be485889ca1b0cbde511b52c08384a967cbd5ea5675
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:a6c64f0117f2b1854fd8cc37d3d0da23529e3d95f10d162d87db15efa3057035
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156142137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c108f33354ee2235420edb7f40d27abacfc2fae57dd611af19ed5326d1c9b6`
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
# Mon, 22 Feb 2021 23:19:56 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:19:57 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Feb 2021 23:20:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Feb 2021 23:20:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Feb 2021 23:20:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Feb 2021 23:20:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:20:33 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:33 GMT
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
	-	`sha256:e103cf56feaac54588520455772f56ecec1130f98b655d09a1022836c4024262`  
		Last Modified: Mon, 22 Feb 2021 23:21:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdc8c250229899be82a8ff7702fba0e5ce1206f922778009868a412906a4a39`  
		Last Modified: Mon, 22 Feb 2021 23:21:29 GMT  
		Size: 105.9 MB (105944167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cadc426ed7f2bb4af24335c5d75bea8d341858126ffd38f9244ea18051c205f`  
		Last Modified: Mon, 22 Feb 2021 23:21:11 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b915ce5921f8be1e499efba626b6381c84a6793c6ceed11dd08e44bf63d7132`  
		Last Modified: Mon, 22 Feb 2021 23:21:10 GMT  
		Size: 4.4 KB (4423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:6c986d8f3b15147e2686b5f18528568358e75082ea27b40bb6f334dfe98566ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144899547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb0426b61f02d274933d51e25066f6f0e0e40ba5afecb42143518c71e5f8e97c`
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
# Mon, 22 Feb 2021 23:05:19 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:05:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Feb 2021 23:05:57 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Feb 2021 23:06:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Feb 2021 23:06:02 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Feb 2021 23:06:03 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:06:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:06:05 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:06:06 GMT
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
	-	`sha256:9103de8f97f155d692d8eaab28a53556bf64a67e2418e2ba9f2cdc5170ef26ff`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab59aaf4bed13a057afb7cb133fa7bf397a727e2574817fe15b0e9749181067`  
		Last Modified: Mon, 22 Feb 2021 23:07:13 GMT  
		Size: 100.3 MB (100324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e49b7d41138eb4b8c3b79e491262204490abb78ea370d8468372074dcf82b36`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8f1df5c32704f2de74431ded913d8f63333a1a9e4db669a59132a1be3d3fd1`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:3432d516c817351978ee2b7cf310fc136a6b77a65a46a6cc3a0c46809d1a9f7e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674485107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:598a1e947ae6da2eb6e5bcb026f0fa03fb0fb85f0c018c6076ce2ebe86370f64`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:15:36 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:15:37 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:15:38 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:17:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:17:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:17:43 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:17:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7e4348dffe8c0aeab8fef00827c09bd768058da1788669465a2cfca45d536c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784f12f422a7bb83e92e2a08268d4e4c1515cb4984df8af595537c7e81fef4c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be372049315197e0d98e4548964d67f87f9d71f7fd2a579b922d6ee4ed186121`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251196694383f58bfdf4135282dd2495348a73d659e350bb187d5ee7233ecd77`  
		Last Modified: Mon, 22 Feb 2021 23:23:37 GMT  
		Size: 235.2 MB (235208405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0e1f02f3de7f62c130b93ac9d3971063230bf03a542ffe6a1b97fe9009f35`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57d6ce2ff5fbf53e010b187e3bc977297b3c8f54c8dcd113ffc8cccd0116fc8`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bf66368e59c8bcad38c9cb5f367b5a21206fadaf425a213646edc3add7054`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:802a473dccfd0937bd71059b6bd21b9990e8df87a15c0b0e4190e68578692dc6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6030930632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb70d7a01406d482faf8ffc57a5cf880e16fc12fcf7869dd8c1276d8c3514409`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:18:03 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:18:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:18:05 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:20:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:20:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:20:58 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:59 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cc54dd5608f00189c2daa7b1de41edc1bc5eabb2c6786b995590897a8b0860`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530b06b0304f622ee88efb9cb8743f0d159b849c3443a93642ea5946fb2e73a3`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16564f4738b901477bfd4793a456a3e0ebe5003c30cb229a5d42e2139c05c9be`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b0f74b17f0ec369dfbace74cd42a56c2f49097d50caf7f5943667b0556893`  
		Last Modified: Mon, 22 Feb 2021 23:24:36 GMT  
		Size: 235.9 MB (235907773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bae7d7730cd475edb00e68b798d2ddc9e4e7736bd80d645e8e42ce600a8c25`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30c850711d5af3ab7db6ca76318c0caef248dd01aa6ae4af304201eb27a6951`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1955878305d020007ebb45a2f9dfbc79268db21f53ce6197ca450ca0669e956`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.23`

```console
$ docker pull mongo@sha256:463b14d54fb2845102072be485889ca1b0cbde511b52c08384a967cbd5ea5675
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.0.23` - linux; amd64

```console
$ docker pull mongo@sha256:a6c64f0117f2b1854fd8cc37d3d0da23529e3d95f10d162d87db15efa3057035
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156142137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c108f33354ee2235420edb7f40d27abacfc2fae57dd611af19ed5326d1c9b6`
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
# Mon, 22 Feb 2021 23:19:56 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:19:57 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Feb 2021 23:20:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Feb 2021 23:20:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Feb 2021 23:20:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Feb 2021 23:20:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:20:33 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:33 GMT
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
	-	`sha256:e103cf56feaac54588520455772f56ecec1130f98b655d09a1022836c4024262`  
		Last Modified: Mon, 22 Feb 2021 23:21:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdc8c250229899be82a8ff7702fba0e5ce1206f922778009868a412906a4a39`  
		Last Modified: Mon, 22 Feb 2021 23:21:29 GMT  
		Size: 105.9 MB (105944167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cadc426ed7f2bb4af24335c5d75bea8d341858126ffd38f9244ea18051c205f`  
		Last Modified: Mon, 22 Feb 2021 23:21:11 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b915ce5921f8be1e499efba626b6381c84a6793c6ceed11dd08e44bf63d7132`  
		Last Modified: Mon, 22 Feb 2021 23:21:10 GMT  
		Size: 4.4 KB (4423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.23` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:6c986d8f3b15147e2686b5f18528568358e75082ea27b40bb6f334dfe98566ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144899547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb0426b61f02d274933d51e25066f6f0e0e40ba5afecb42143518c71e5f8e97c`
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
# Mon, 22 Feb 2021 23:05:19 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:05:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Feb 2021 23:05:57 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Feb 2021 23:06:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Feb 2021 23:06:02 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Feb 2021 23:06:03 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:06:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:06:05 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:06:06 GMT
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
	-	`sha256:9103de8f97f155d692d8eaab28a53556bf64a67e2418e2ba9f2cdc5170ef26ff`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab59aaf4bed13a057afb7cb133fa7bf397a727e2574817fe15b0e9749181067`  
		Last Modified: Mon, 22 Feb 2021 23:07:13 GMT  
		Size: 100.3 MB (100324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e49b7d41138eb4b8c3b79e491262204490abb78ea370d8468372074dcf82b36`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8f1df5c32704f2de74431ded913d8f63333a1a9e4db669a59132a1be3d3fd1`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.23` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:3432d516c817351978ee2b7cf310fc136a6b77a65a46a6cc3a0c46809d1a9f7e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674485107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:598a1e947ae6da2eb6e5bcb026f0fa03fb0fb85f0c018c6076ce2ebe86370f64`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:15:36 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:15:37 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:15:38 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:17:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:17:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:17:43 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:17:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7e4348dffe8c0aeab8fef00827c09bd768058da1788669465a2cfca45d536c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784f12f422a7bb83e92e2a08268d4e4c1515cb4984df8af595537c7e81fef4c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be372049315197e0d98e4548964d67f87f9d71f7fd2a579b922d6ee4ed186121`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251196694383f58bfdf4135282dd2495348a73d659e350bb187d5ee7233ecd77`  
		Last Modified: Mon, 22 Feb 2021 23:23:37 GMT  
		Size: 235.2 MB (235208405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0e1f02f3de7f62c130b93ac9d3971063230bf03a542ffe6a1b97fe9009f35`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57d6ce2ff5fbf53e010b187e3bc977297b3c8f54c8dcd113ffc8cccd0116fc8`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bf66368e59c8bcad38c9cb5f367b5a21206fadaf425a213646edc3add7054`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.23` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:802a473dccfd0937bd71059b6bd21b9990e8df87a15c0b0e4190e68578692dc6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6030930632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb70d7a01406d482faf8ffc57a5cf880e16fc12fcf7869dd8c1276d8c3514409`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:18:03 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:18:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:18:05 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:20:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:20:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:20:58 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:59 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cc54dd5608f00189c2daa7b1de41edc1bc5eabb2c6786b995590897a8b0860`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530b06b0304f622ee88efb9cb8743f0d159b849c3443a93642ea5946fb2e73a3`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16564f4738b901477bfd4793a456a3e0ebe5003c30cb229a5d42e2139c05c9be`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b0f74b17f0ec369dfbace74cd42a56c2f49097d50caf7f5943667b0556893`  
		Last Modified: Mon, 22 Feb 2021 23:24:36 GMT  
		Size: 235.9 MB (235907773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bae7d7730cd475edb00e68b798d2ddc9e4e7736bd80d645e8e42ce600a8c25`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30c850711d5af3ab7db6ca76318c0caef248dd01aa6ae4af304201eb27a6951`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1955878305d020007ebb45a2f9dfbc79268db21f53ce6197ca450ca0669e956`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.23-windowsservercore`

```console
$ docker pull mongo@sha256:986844ec56a5af90c2509661da8f50c6c1d4b58506f1fff4f1620519f32f04c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.0.23-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:3432d516c817351978ee2b7cf310fc136a6b77a65a46a6cc3a0c46809d1a9f7e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674485107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:598a1e947ae6da2eb6e5bcb026f0fa03fb0fb85f0c018c6076ce2ebe86370f64`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:15:36 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:15:37 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:15:38 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:17:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:17:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:17:43 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:17:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7e4348dffe8c0aeab8fef00827c09bd768058da1788669465a2cfca45d536c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784f12f422a7bb83e92e2a08268d4e4c1515cb4984df8af595537c7e81fef4c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be372049315197e0d98e4548964d67f87f9d71f7fd2a579b922d6ee4ed186121`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251196694383f58bfdf4135282dd2495348a73d659e350bb187d5ee7233ecd77`  
		Last Modified: Mon, 22 Feb 2021 23:23:37 GMT  
		Size: 235.2 MB (235208405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0e1f02f3de7f62c130b93ac9d3971063230bf03a542ffe6a1b97fe9009f35`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57d6ce2ff5fbf53e010b187e3bc977297b3c8f54c8dcd113ffc8cccd0116fc8`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bf66368e59c8bcad38c9cb5f367b5a21206fadaf425a213646edc3add7054`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.23-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:802a473dccfd0937bd71059b6bd21b9990e8df87a15c0b0e4190e68578692dc6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6030930632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb70d7a01406d482faf8ffc57a5cf880e16fc12fcf7869dd8c1276d8c3514409`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:18:03 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:18:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:18:05 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:20:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:20:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:20:58 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:59 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cc54dd5608f00189c2daa7b1de41edc1bc5eabb2c6786b995590897a8b0860`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530b06b0304f622ee88efb9cb8743f0d159b849c3443a93642ea5946fb2e73a3`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16564f4738b901477bfd4793a456a3e0ebe5003c30cb229a5d42e2139c05c9be`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b0f74b17f0ec369dfbace74cd42a56c2f49097d50caf7f5943667b0556893`  
		Last Modified: Mon, 22 Feb 2021 23:24:36 GMT  
		Size: 235.9 MB (235907773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bae7d7730cd475edb00e68b798d2ddc9e4e7736bd80d645e8e42ce600a8c25`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30c850711d5af3ab7db6ca76318c0caef248dd01aa6ae4af304201eb27a6951`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1955878305d020007ebb45a2f9dfbc79268db21f53ce6197ca450ca0669e956`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.23-windowsservercore-1809`

```console
$ docker pull mongo@sha256:59b07cc243a1755ba596677e1c318ebd67ec63dc423f8f1df9fcbf4429dfe6f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:4.0.23-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:3432d516c817351978ee2b7cf310fc136a6b77a65a46a6cc3a0c46809d1a9f7e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674485107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:598a1e947ae6da2eb6e5bcb026f0fa03fb0fb85f0c018c6076ce2ebe86370f64`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:15:36 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:15:37 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:15:38 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:17:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:17:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:17:43 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:17:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7e4348dffe8c0aeab8fef00827c09bd768058da1788669465a2cfca45d536c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784f12f422a7bb83e92e2a08268d4e4c1515cb4984df8af595537c7e81fef4c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be372049315197e0d98e4548964d67f87f9d71f7fd2a579b922d6ee4ed186121`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251196694383f58bfdf4135282dd2495348a73d659e350bb187d5ee7233ecd77`  
		Last Modified: Mon, 22 Feb 2021 23:23:37 GMT  
		Size: 235.2 MB (235208405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0e1f02f3de7f62c130b93ac9d3971063230bf03a542ffe6a1b97fe9009f35`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57d6ce2ff5fbf53e010b187e3bc977297b3c8f54c8dcd113ffc8cccd0116fc8`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bf66368e59c8bcad38c9cb5f367b5a21206fadaf425a213646edc3add7054`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.23-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:8c1aeb4197811040056ac455f5176fdc10b0e1afaade27ea3d20d5c0df324a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.0.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:802a473dccfd0937bd71059b6bd21b9990e8df87a15c0b0e4190e68578692dc6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6030930632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb70d7a01406d482faf8ffc57a5cf880e16fc12fcf7869dd8c1276d8c3514409`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:18:03 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:18:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:18:05 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:20:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:20:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:20:58 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:59 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cc54dd5608f00189c2daa7b1de41edc1bc5eabb2c6786b995590897a8b0860`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530b06b0304f622ee88efb9cb8743f0d159b849c3443a93642ea5946fb2e73a3`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16564f4738b901477bfd4793a456a3e0ebe5003c30cb229a5d42e2139c05c9be`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b0f74b17f0ec369dfbace74cd42a56c2f49097d50caf7f5943667b0556893`  
		Last Modified: Mon, 22 Feb 2021 23:24:36 GMT  
		Size: 235.9 MB (235907773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bae7d7730cd475edb00e68b798d2ddc9e4e7736bd80d645e8e42ce600a8c25`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30c850711d5af3ab7db6ca76318c0caef248dd01aa6ae4af304201eb27a6951`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1955878305d020007ebb45a2f9dfbc79268db21f53ce6197ca450ca0669e956`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.23-xenial`

```console
$ docker pull mongo@sha256:17908be4707c47b48c2d29f8e43c85aca526ce2b9f15e3db7c5e1c4724715b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.23-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:a6c64f0117f2b1854fd8cc37d3d0da23529e3d95f10d162d87db15efa3057035
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156142137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c108f33354ee2235420edb7f40d27abacfc2fae57dd611af19ed5326d1c9b6`
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
# Mon, 22 Feb 2021 23:19:56 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:19:57 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Feb 2021 23:20:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Feb 2021 23:20:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Feb 2021 23:20:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Feb 2021 23:20:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:20:33 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:33 GMT
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
	-	`sha256:e103cf56feaac54588520455772f56ecec1130f98b655d09a1022836c4024262`  
		Last Modified: Mon, 22 Feb 2021 23:21:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdc8c250229899be82a8ff7702fba0e5ce1206f922778009868a412906a4a39`  
		Last Modified: Mon, 22 Feb 2021 23:21:29 GMT  
		Size: 105.9 MB (105944167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cadc426ed7f2bb4af24335c5d75bea8d341858126ffd38f9244ea18051c205f`  
		Last Modified: Mon, 22 Feb 2021 23:21:11 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b915ce5921f8be1e499efba626b6381c84a6793c6ceed11dd08e44bf63d7132`  
		Last Modified: Mon, 22 Feb 2021 23:21:10 GMT  
		Size: 4.4 KB (4423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.23-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:6c986d8f3b15147e2686b5f18528568358e75082ea27b40bb6f334dfe98566ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144899547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb0426b61f02d274933d51e25066f6f0e0e40ba5afecb42143518c71e5f8e97c`
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
# Mon, 22 Feb 2021 23:05:19 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:05:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Feb 2021 23:05:57 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Feb 2021 23:06:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Feb 2021 23:06:02 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Feb 2021 23:06:03 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:06:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:06:05 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:06:06 GMT
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
	-	`sha256:9103de8f97f155d692d8eaab28a53556bf64a67e2418e2ba9f2cdc5170ef26ff`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab59aaf4bed13a057afb7cb133fa7bf397a727e2574817fe15b0e9749181067`  
		Last Modified: Mon, 22 Feb 2021 23:07:13 GMT  
		Size: 100.3 MB (100324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e49b7d41138eb4b8c3b79e491262204490abb78ea370d8468372074dcf82b36`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8f1df5c32704f2de74431ded913d8f63333a1a9e4db669a59132a1be3d3fd1`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:986844ec56a5af90c2509661da8f50c6c1d4b58506f1fff4f1620519f32f04c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:3432d516c817351978ee2b7cf310fc136a6b77a65a46a6cc3a0c46809d1a9f7e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674485107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:598a1e947ae6da2eb6e5bcb026f0fa03fb0fb85f0c018c6076ce2ebe86370f64`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:15:36 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:15:37 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:15:38 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:17:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:17:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:17:43 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:17:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7e4348dffe8c0aeab8fef00827c09bd768058da1788669465a2cfca45d536c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784f12f422a7bb83e92e2a08268d4e4c1515cb4984df8af595537c7e81fef4c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be372049315197e0d98e4548964d67f87f9d71f7fd2a579b922d6ee4ed186121`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251196694383f58bfdf4135282dd2495348a73d659e350bb187d5ee7233ecd77`  
		Last Modified: Mon, 22 Feb 2021 23:23:37 GMT  
		Size: 235.2 MB (235208405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0e1f02f3de7f62c130b93ac9d3971063230bf03a542ffe6a1b97fe9009f35`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57d6ce2ff5fbf53e010b187e3bc977297b3c8f54c8dcd113ffc8cccd0116fc8`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bf66368e59c8bcad38c9cb5f367b5a21206fadaf425a213646edc3add7054`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:802a473dccfd0937bd71059b6bd21b9990e8df87a15c0b0e4190e68578692dc6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6030930632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb70d7a01406d482faf8ffc57a5cf880e16fc12fcf7869dd8c1276d8c3514409`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:18:03 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:18:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:18:05 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:20:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:20:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:20:58 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:59 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cc54dd5608f00189c2daa7b1de41edc1bc5eabb2c6786b995590897a8b0860`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530b06b0304f622ee88efb9cb8743f0d159b849c3443a93642ea5946fb2e73a3`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16564f4738b901477bfd4793a456a3e0ebe5003c30cb229a5d42e2139c05c9be`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b0f74b17f0ec369dfbace74cd42a56c2f49097d50caf7f5943667b0556893`  
		Last Modified: Mon, 22 Feb 2021 23:24:36 GMT  
		Size: 235.9 MB (235907773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bae7d7730cd475edb00e68b798d2ddc9e4e7736bd80d645e8e42ce600a8c25`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30c850711d5af3ab7db6ca76318c0caef248dd01aa6ae4af304201eb27a6951`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1955878305d020007ebb45a2f9dfbc79268db21f53ce6197ca450ca0669e956`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:59b07cc243a1755ba596677e1c318ebd67ec63dc423f8f1df9fcbf4429dfe6f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:3432d516c817351978ee2b7cf310fc136a6b77a65a46a6cc3a0c46809d1a9f7e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2674485107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:598a1e947ae6da2eb6e5bcb026f0fa03fb0fb85f0c018c6076ce2ebe86370f64`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:15:36 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:15:37 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:15:38 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:17:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:17:41 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:17:43 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:17:45 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7e4348dffe8c0aeab8fef00827c09bd768058da1788669465a2cfca45d536c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5784f12f422a7bb83e92e2a08268d4e4c1515cb4984df8af595537c7e81fef4c`  
		Last Modified: Mon, 22 Feb 2021 23:22:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be372049315197e0d98e4548964d67f87f9d71f7fd2a579b922d6ee4ed186121`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251196694383f58bfdf4135282dd2495348a73d659e350bb187d5ee7233ecd77`  
		Last Modified: Mon, 22 Feb 2021 23:23:37 GMT  
		Size: 235.2 MB (235208405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0e1f02f3de7f62c130b93ac9d3971063230bf03a542ffe6a1b97fe9009f35`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57d6ce2ff5fbf53e010b187e3bc977297b3c8f54c8dcd113ffc8cccd0116fc8`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974bf66368e59c8bcad38c9cb5f367b5a21206fadaf425a213646edc3add7054`  
		Last Modified: Mon, 22 Feb 2021 23:22:49 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:8c1aeb4197811040056ac455f5176fdc10b0e1afaade27ea3d20d5c0df324a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:802a473dccfd0937bd71059b6bd21b9990e8df87a15c0b0e4190e68578692dc6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6030930632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb70d7a01406d482faf8ffc57a5cf880e16fc12fcf7869dd8c1276d8c3514409`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Feb 2021 23:18:03 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:18:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Mon, 22 Feb 2021 23:18:05 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Mon, 22 Feb 2021 23:20:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Feb 2021 23:20:57 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Feb 2021 23:20:58 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:59 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cc54dd5608f00189c2daa7b1de41edc1bc5eabb2c6786b995590897a8b0860`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530b06b0304f622ee88efb9cb8743f0d159b849c3443a93642ea5946fb2e73a3`  
		Last Modified: Mon, 22 Feb 2021 23:23:51 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16564f4738b901477bfd4793a456a3e0ebe5003c30cb229a5d42e2139c05c9be`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84b0f74b17f0ec369dfbace74cd42a56c2f49097d50caf7f5943667b0556893`  
		Last Modified: Mon, 22 Feb 2021 23:24:36 GMT  
		Size: 235.9 MB (235907773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bae7d7730cd475edb00e68b798d2ddc9e4e7736bd80d645e8e42ce600a8c25`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30c850711d5af3ab7db6ca76318c0caef248dd01aa6ae4af304201eb27a6951`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1955878305d020007ebb45a2f9dfbc79268db21f53ce6197ca450ca0669e956`  
		Last Modified: Mon, 22 Feb 2021 23:23:48 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:17908be4707c47b48c2d29f8e43c85aca526ce2b9f15e3db7c5e1c4724715b7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:a6c64f0117f2b1854fd8cc37d3d0da23529e3d95f10d162d87db15efa3057035
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156142137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c108f33354ee2235420edb7f40d27abacfc2fae57dd611af19ed5326d1c9b6`
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
# Mon, 22 Feb 2021 23:19:56 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:19:57 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Feb 2021 23:20:30 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Feb 2021 23:20:32 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Feb 2021 23:20:32 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Feb 2021 23:20:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:20:33 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:20:33 GMT
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
	-	`sha256:e103cf56feaac54588520455772f56ecec1130f98b655d09a1022836c4024262`  
		Last Modified: Mon, 22 Feb 2021 23:21:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdc8c250229899be82a8ff7702fba0e5ce1206f922778009868a412906a4a39`  
		Last Modified: Mon, 22 Feb 2021 23:21:29 GMT  
		Size: 105.9 MB (105944167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cadc426ed7f2bb4af24335c5d75bea8d341858126ffd38f9244ea18051c205f`  
		Last Modified: Mon, 22 Feb 2021 23:21:11 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b915ce5921f8be1e499efba626b6381c84a6793c6ceed11dd08e44bf63d7132`  
		Last Modified: Mon, 22 Feb 2021 23:21:10 GMT  
		Size: 4.4 KB (4423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:6c986d8f3b15147e2686b5f18528568358e75082ea27b40bb6f334dfe98566ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144899547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb0426b61f02d274933d51e25066f6f0e0e40ba5afecb42143518c71e5f8e97c`
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
# Mon, 22 Feb 2021 23:05:19 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Feb 2021 23:05:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Feb 2021 23:05:57 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Feb 2021 23:06:01 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Feb 2021 23:06:02 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Feb 2021 23:06:03 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Feb 2021 23:06:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Feb 2021 23:06:05 GMT
EXPOSE 27017
# Mon, 22 Feb 2021 23:06:06 GMT
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
	-	`sha256:9103de8f97f155d692d8eaab28a53556bf64a67e2418e2ba9f2cdc5170ef26ff`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab59aaf4bed13a057afb7cb133fa7bf397a727e2574817fe15b0e9749181067`  
		Last Modified: Mon, 22 Feb 2021 23:07:13 GMT  
		Size: 100.3 MB (100324488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e49b7d41138eb4b8c3b79e491262204490abb78ea370d8468372074dcf82b36`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8f1df5c32704f2de74431ded913d8f63333a1a9e4db669a59132a1be3d3fd1`  
		Last Modified: Mon, 22 Feb 2021 23:06:50 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:a3a427cfb72524b6734ed08bd9f231b685e7047ad0b68dda15456fe2399cd810
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:3897109ec7975e2e66b1fda9c23ea57e3a6e5fb9c42431dfe76306b14a6561df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165092710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d93f84193018e16e5556ea3c0fe4d94e74d86f8d77d30df72f66152d84dca75`
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
# Mon, 25 Jan 2021 21:22:43 GMT
ENV MONGO_VERSION=4.2.12
# Mon, 25 Jan 2021 21:22:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 25 Jan 2021 21:23:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 25 Jan 2021 21:23:07 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 25 Jan 2021 21:23:07 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:15 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:15 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:15 GMT
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
	-	`sha256:259d5efad6ab4b42b841d666eddcb53d137aa8ef53b686c6c88a405d93b65573`  
		Last Modified: Mon, 25 Jan 2021 21:23:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745974bc412b7633b1290d46c29cdfb0675c5b65c36e74130b3b93f223509c22`  
		Last Modified: Mon, 25 Jan 2021 21:24:12 GMT  
		Size: 129.6 MB (129556096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69a5971e7f450ab2317d1b7a4c013d8bd80f42023511b30c6b73174c9011d74`  
		Last Modified: Mon, 25 Jan 2021 21:23:53 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c52c8d23db23f2559a563b8095f487b72540cbd4f62c9ab8a1ac80e8d9a5963`  
		Last Modified: Wed, 17 Feb 2021 00:18:25 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7627d4ced4a6ccc64764cb981b385158185e7e83bd8b2a5291bef2b0feaae048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155071395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f8fc1c697fa4229fea87065e09720ebf79749546d335a1130b65cc38f906a4`
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
# Wed, 17 Feb 2021 00:14:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:14:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:14:07 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:14:08 GMT
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
	-	`sha256:f9197d5d54019383967d6cac03e2ea5ec050a431fe996603badf7f60e44ed8ef`  
		Last Modified: Wed, 17 Feb 2021 00:15:49 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cd6084b972d634cc951ce015f81b8d9dcf607ff469eca68add9b371f2cc6083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2729696598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286b8a1bd32d93129f2c880b31455c3e7698a3410f79080818a9bea4ed87b67b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:36:48 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:38:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:38:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:38:52 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:38:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7877e2093132135d0736339977fab38165007cd5a915c3845360152dca9ef9c4`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0fd646dc9583d9de3bc0368a258c5ca4fc34c347516e1faed2bcf0e5fb5df2`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fa05efbb9d013622ad63a8e483b43df09c5ee738f99e73bcc57eaf5290f8a3`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d15a871c49181eb8884904ffc139e5d4889ef074a838e9f94b84bb229d5dfa`  
		Last Modified: Tue, 09 Feb 2021 21:09:03 GMT  
		Size: 290.4 MB (290420013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d16a7ee3b2395d0dfa6f59e6e9874c3b9e84e7c3785029aa4a473ec4a123a20`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e49c653c2c64cc3f43a9f218195b5164deaba8f4c0027d39176ffe8e314067`  
		Last Modified: Tue, 09 Feb 2021 21:03:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaa63d20892b0a6024db1589b775e5a5b285651b446800aa6d6662550088bcb`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:a545c92ec61392ca47d093fd296ab3f608594b03deec2a24073ca0cd1277b6ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6086150287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788a9b87dc607fbd579944881426492e960624d9e12173b0c027e60b38bd898f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:38:59 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:39:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:39:01 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:41:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:41:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:42:00 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:42:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39600dd254ee2f8c385ac8abe438b3026ecfbc59fd4cede8baf9e49755ccf42f`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037dc38ff67e44e8539b98a2697a944c4b5dc84f47cbd6fcb2d889bf63f22458`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9629bcb0abfe902504f9af494c22f945caa0d508c4abdfcca98d2782137ca419`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77845301e844a5b2137f771aea4bbe82fdb2c4b773a6ed0fb9222a0545d7c05`  
		Last Modified: Tue, 09 Feb 2021 21:14:43 GMT  
		Size: 291.1 MB (291127624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b761c8dba0c8256e4ce171503a9859d22b806ab2d93cde37f5961457bd2a0e`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfefda86e4fa28b33f2d2cef255bfe31abc0ca3456b2dec7076e47376f397b6c`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ec9b75afd6d4e065c60a77490aa3477653a68de0876a26dc38c405b2ec9668`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.12`

```console
$ docker pull mongo@sha256:a3a427cfb72524b6734ed08bd9f231b685e7047ad0b68dda15456fe2399cd810
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.2.12` - linux; amd64

```console
$ docker pull mongo@sha256:3897109ec7975e2e66b1fda9c23ea57e3a6e5fb9c42431dfe76306b14a6561df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165092710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d93f84193018e16e5556ea3c0fe4d94e74d86f8d77d30df72f66152d84dca75`
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
# Mon, 25 Jan 2021 21:22:43 GMT
ENV MONGO_VERSION=4.2.12
# Mon, 25 Jan 2021 21:22:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 25 Jan 2021 21:23:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 25 Jan 2021 21:23:07 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 25 Jan 2021 21:23:07 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:15 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:15 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:15 GMT
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
	-	`sha256:259d5efad6ab4b42b841d666eddcb53d137aa8ef53b686c6c88a405d93b65573`  
		Last Modified: Mon, 25 Jan 2021 21:23:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745974bc412b7633b1290d46c29cdfb0675c5b65c36e74130b3b93f223509c22`  
		Last Modified: Mon, 25 Jan 2021 21:24:12 GMT  
		Size: 129.6 MB (129556096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69a5971e7f450ab2317d1b7a4c013d8bd80f42023511b30c6b73174c9011d74`  
		Last Modified: Mon, 25 Jan 2021 21:23:53 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c52c8d23db23f2559a563b8095f487b72540cbd4f62c9ab8a1ac80e8d9a5963`  
		Last Modified: Wed, 17 Feb 2021 00:18:25 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.12` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7627d4ced4a6ccc64764cb981b385158185e7e83bd8b2a5291bef2b0feaae048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155071395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f8fc1c697fa4229fea87065e09720ebf79749546d335a1130b65cc38f906a4`
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
# Wed, 17 Feb 2021 00:14:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:14:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:14:07 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:14:08 GMT
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
	-	`sha256:f9197d5d54019383967d6cac03e2ea5ec050a431fe996603badf7f60e44ed8ef`  
		Last Modified: Wed, 17 Feb 2021 00:15:49 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.12` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cd6084b972d634cc951ce015f81b8d9dcf607ff469eca68add9b371f2cc6083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2729696598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286b8a1bd32d93129f2c880b31455c3e7698a3410f79080818a9bea4ed87b67b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:36:48 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:38:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:38:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:38:52 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:38:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7877e2093132135d0736339977fab38165007cd5a915c3845360152dca9ef9c4`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0fd646dc9583d9de3bc0368a258c5ca4fc34c347516e1faed2bcf0e5fb5df2`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fa05efbb9d013622ad63a8e483b43df09c5ee738f99e73bcc57eaf5290f8a3`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d15a871c49181eb8884904ffc139e5d4889ef074a838e9f94b84bb229d5dfa`  
		Last Modified: Tue, 09 Feb 2021 21:09:03 GMT  
		Size: 290.4 MB (290420013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d16a7ee3b2395d0dfa6f59e6e9874c3b9e84e7c3785029aa4a473ec4a123a20`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e49c653c2c64cc3f43a9f218195b5164deaba8f4c0027d39176ffe8e314067`  
		Last Modified: Tue, 09 Feb 2021 21:03:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaa63d20892b0a6024db1589b775e5a5b285651b446800aa6d6662550088bcb`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.12` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:a545c92ec61392ca47d093fd296ab3f608594b03deec2a24073ca0cd1277b6ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6086150287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788a9b87dc607fbd579944881426492e960624d9e12173b0c027e60b38bd898f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:38:59 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:39:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:39:01 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:41:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:41:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:42:00 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:42:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39600dd254ee2f8c385ac8abe438b3026ecfbc59fd4cede8baf9e49755ccf42f`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037dc38ff67e44e8539b98a2697a944c4b5dc84f47cbd6fcb2d889bf63f22458`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9629bcb0abfe902504f9af494c22f945caa0d508c4abdfcca98d2782137ca419`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77845301e844a5b2137f771aea4bbe82fdb2c4b773a6ed0fb9222a0545d7c05`  
		Last Modified: Tue, 09 Feb 2021 21:14:43 GMT  
		Size: 291.1 MB (291127624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b761c8dba0c8256e4ce171503a9859d22b806ab2d93cde37f5961457bd2a0e`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfefda86e4fa28b33f2d2cef255bfe31abc0ca3456b2dec7076e47376f397b6c`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ec9b75afd6d4e065c60a77490aa3477653a68de0876a26dc38c405b2ec9668`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.12-bionic`

```console
$ docker pull mongo@sha256:f20522ee939f0aecb4b6d0bcaa668ae9c224ccf46d7bba1b5bf1a2ea3099603b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2.12-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:3897109ec7975e2e66b1fda9c23ea57e3a6e5fb9c42431dfe76306b14a6561df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165092710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d93f84193018e16e5556ea3c0fe4d94e74d86f8d77d30df72f66152d84dca75`
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
# Mon, 25 Jan 2021 21:22:43 GMT
ENV MONGO_VERSION=4.2.12
# Mon, 25 Jan 2021 21:22:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 25 Jan 2021 21:23:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 25 Jan 2021 21:23:07 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 25 Jan 2021 21:23:07 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:15 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:15 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:15 GMT
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
	-	`sha256:259d5efad6ab4b42b841d666eddcb53d137aa8ef53b686c6c88a405d93b65573`  
		Last Modified: Mon, 25 Jan 2021 21:23:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745974bc412b7633b1290d46c29cdfb0675c5b65c36e74130b3b93f223509c22`  
		Last Modified: Mon, 25 Jan 2021 21:24:12 GMT  
		Size: 129.6 MB (129556096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69a5971e7f450ab2317d1b7a4c013d8bd80f42023511b30c6b73174c9011d74`  
		Last Modified: Mon, 25 Jan 2021 21:23:53 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c52c8d23db23f2559a563b8095f487b72540cbd4f62c9ab8a1ac80e8d9a5963`  
		Last Modified: Wed, 17 Feb 2021 00:18:25 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.12-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7627d4ced4a6ccc64764cb981b385158185e7e83bd8b2a5291bef2b0feaae048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155071395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f8fc1c697fa4229fea87065e09720ebf79749546d335a1130b65cc38f906a4`
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
# Wed, 17 Feb 2021 00:14:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:14:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:14:07 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:14:08 GMT
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
	-	`sha256:f9197d5d54019383967d6cac03e2ea5ec050a431fe996603badf7f60e44ed8ef`  
		Last Modified: Wed, 17 Feb 2021 00:15:49 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.12-windowsservercore`

```console
$ docker pull mongo@sha256:8084195d680e5281961ddc041b227898c0d4139f4bb6bc2df748274975c0f188
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.2.12-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cd6084b972d634cc951ce015f81b8d9dcf607ff469eca68add9b371f2cc6083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2729696598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286b8a1bd32d93129f2c880b31455c3e7698a3410f79080818a9bea4ed87b67b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:36:48 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:38:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:38:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:38:52 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:38:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7877e2093132135d0736339977fab38165007cd5a915c3845360152dca9ef9c4`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0fd646dc9583d9de3bc0368a258c5ca4fc34c347516e1faed2bcf0e5fb5df2`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fa05efbb9d013622ad63a8e483b43df09c5ee738f99e73bcc57eaf5290f8a3`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d15a871c49181eb8884904ffc139e5d4889ef074a838e9f94b84bb229d5dfa`  
		Last Modified: Tue, 09 Feb 2021 21:09:03 GMT  
		Size: 290.4 MB (290420013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d16a7ee3b2395d0dfa6f59e6e9874c3b9e84e7c3785029aa4a473ec4a123a20`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e49c653c2c64cc3f43a9f218195b5164deaba8f4c0027d39176ffe8e314067`  
		Last Modified: Tue, 09 Feb 2021 21:03:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaa63d20892b0a6024db1589b775e5a5b285651b446800aa6d6662550088bcb`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.12-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:a545c92ec61392ca47d093fd296ab3f608594b03deec2a24073ca0cd1277b6ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6086150287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788a9b87dc607fbd579944881426492e960624d9e12173b0c027e60b38bd898f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:38:59 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:39:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:39:01 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:41:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:41:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:42:00 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:42:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39600dd254ee2f8c385ac8abe438b3026ecfbc59fd4cede8baf9e49755ccf42f`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037dc38ff67e44e8539b98a2697a944c4b5dc84f47cbd6fcb2d889bf63f22458`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9629bcb0abfe902504f9af494c22f945caa0d508c4abdfcca98d2782137ca419`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77845301e844a5b2137f771aea4bbe82fdb2c4b773a6ed0fb9222a0545d7c05`  
		Last Modified: Tue, 09 Feb 2021 21:14:43 GMT  
		Size: 291.1 MB (291127624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b761c8dba0c8256e4ce171503a9859d22b806ab2d93cde37f5961457bd2a0e`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfefda86e4fa28b33f2d2cef255bfe31abc0ca3456b2dec7076e47376f397b6c`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ec9b75afd6d4e065c60a77490aa3477653a68de0876a26dc38c405b2ec9668`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.12-windowsservercore-1809`

```console
$ docker pull mongo@sha256:e2f6f5efebc83753060a5cba706cbeaa06e6286dfbef2f2fe90553be06ac9ec6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:4.2.12-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cd6084b972d634cc951ce015f81b8d9dcf607ff469eca68add9b371f2cc6083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2729696598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286b8a1bd32d93129f2c880b31455c3e7698a3410f79080818a9bea4ed87b67b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:36:48 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:38:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:38:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:38:52 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:38:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7877e2093132135d0736339977fab38165007cd5a915c3845360152dca9ef9c4`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0fd646dc9583d9de3bc0368a258c5ca4fc34c347516e1faed2bcf0e5fb5df2`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fa05efbb9d013622ad63a8e483b43df09c5ee738f99e73bcc57eaf5290f8a3`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d15a871c49181eb8884904ffc139e5d4889ef074a838e9f94b84bb229d5dfa`  
		Last Modified: Tue, 09 Feb 2021 21:09:03 GMT  
		Size: 290.4 MB (290420013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d16a7ee3b2395d0dfa6f59e6e9874c3b9e84e7c3785029aa4a473ec4a123a20`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e49c653c2c64cc3f43a9f218195b5164deaba8f4c0027d39176ffe8e314067`  
		Last Modified: Tue, 09 Feb 2021 21:03:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaa63d20892b0a6024db1589b775e5a5b285651b446800aa6d6662550088bcb`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.12-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:04b13ac89331c678ff2811805e9f40b2a5b766761d14c773b56fe78f0e777589
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.2.12-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:a545c92ec61392ca47d093fd296ab3f608594b03deec2a24073ca0cd1277b6ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6086150287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788a9b87dc607fbd579944881426492e960624d9e12173b0c027e60b38bd898f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:38:59 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:39:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:39:01 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:41:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:41:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:42:00 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:42:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39600dd254ee2f8c385ac8abe438b3026ecfbc59fd4cede8baf9e49755ccf42f`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037dc38ff67e44e8539b98a2697a944c4b5dc84f47cbd6fcb2d889bf63f22458`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9629bcb0abfe902504f9af494c22f945caa0d508c4abdfcca98d2782137ca419`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77845301e844a5b2137f771aea4bbe82fdb2c4b773a6ed0fb9222a0545d7c05`  
		Last Modified: Tue, 09 Feb 2021 21:14:43 GMT  
		Size: 291.1 MB (291127624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b761c8dba0c8256e4ce171503a9859d22b806ab2d93cde37f5961457bd2a0e`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfefda86e4fa28b33f2d2cef255bfe31abc0ca3456b2dec7076e47376f397b6c`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ec9b75afd6d4e065c60a77490aa3477653a68de0876a26dc38c405b2ec9668`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:f20522ee939f0aecb4b6d0bcaa668ae9c224ccf46d7bba1b5bf1a2ea3099603b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:3897109ec7975e2e66b1fda9c23ea57e3a6e5fb9c42431dfe76306b14a6561df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165092710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d93f84193018e16e5556ea3c0fe4d94e74d86f8d77d30df72f66152d84dca75`
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
# Mon, 25 Jan 2021 21:22:43 GMT
ENV MONGO_VERSION=4.2.12
# Mon, 25 Jan 2021 21:22:44 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 25 Jan 2021 21:23:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 25 Jan 2021 21:23:07 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 25 Jan 2021 21:23:07 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:15 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:15 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:15 GMT
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
	-	`sha256:259d5efad6ab4b42b841d666eddcb53d137aa8ef53b686c6c88a405d93b65573`  
		Last Modified: Mon, 25 Jan 2021 21:23:54 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745974bc412b7633b1290d46c29cdfb0675c5b65c36e74130b3b93f223509c22`  
		Last Modified: Mon, 25 Jan 2021 21:24:12 GMT  
		Size: 129.6 MB (129556096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69a5971e7f450ab2317d1b7a4c013d8bd80f42023511b30c6b73174c9011d74`  
		Last Modified: Mon, 25 Jan 2021 21:23:53 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c52c8d23db23f2559a563b8095f487b72540cbd4f62c9ab8a1ac80e8d9a5963`  
		Last Modified: Wed, 17 Feb 2021 00:18:25 GMT  
		Size: 4.4 KB (4419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:7627d4ced4a6ccc64764cb981b385158185e7e83bd8b2a5291bef2b0feaae048
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155071395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f8fc1c697fa4229fea87065e09720ebf79749546d335a1130b65cc38f906a4`
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
# Wed, 17 Feb 2021 00:14:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:14:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:14:07 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:14:08 GMT
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
	-	`sha256:f9197d5d54019383967d6cac03e2ea5ec050a431fe996603badf7f60e44ed8ef`  
		Last Modified: Wed, 17 Feb 2021 00:15:49 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:8084195d680e5281961ddc041b227898c0d4139f4bb6bc2df748274975c0f188
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cd6084b972d634cc951ce015f81b8d9dcf607ff469eca68add9b371f2cc6083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2729696598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286b8a1bd32d93129f2c880b31455c3e7698a3410f79080818a9bea4ed87b67b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:36:48 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:38:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:38:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:38:52 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:38:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7877e2093132135d0736339977fab38165007cd5a915c3845360152dca9ef9c4`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0fd646dc9583d9de3bc0368a258c5ca4fc34c347516e1faed2bcf0e5fb5df2`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fa05efbb9d013622ad63a8e483b43df09c5ee738f99e73bcc57eaf5290f8a3`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d15a871c49181eb8884904ffc139e5d4889ef074a838e9f94b84bb229d5dfa`  
		Last Modified: Tue, 09 Feb 2021 21:09:03 GMT  
		Size: 290.4 MB (290420013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d16a7ee3b2395d0dfa6f59e6e9874c3b9e84e7c3785029aa4a473ec4a123a20`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e49c653c2c64cc3f43a9f218195b5164deaba8f4c0027d39176ffe8e314067`  
		Last Modified: Tue, 09 Feb 2021 21:03:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaa63d20892b0a6024db1589b775e5a5b285651b446800aa6d6662550088bcb`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:a545c92ec61392ca47d093fd296ab3f608594b03deec2a24073ca0cd1277b6ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6086150287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788a9b87dc607fbd579944881426492e960624d9e12173b0c027e60b38bd898f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:38:59 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:39:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:39:01 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:41:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:41:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:42:00 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:42:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39600dd254ee2f8c385ac8abe438b3026ecfbc59fd4cede8baf9e49755ccf42f`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037dc38ff67e44e8539b98a2697a944c4b5dc84f47cbd6fcb2d889bf63f22458`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9629bcb0abfe902504f9af494c22f945caa0d508c4abdfcca98d2782137ca419`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77845301e844a5b2137f771aea4bbe82fdb2c4b773a6ed0fb9222a0545d7c05`  
		Last Modified: Tue, 09 Feb 2021 21:14:43 GMT  
		Size: 291.1 MB (291127624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b761c8dba0c8256e4ce171503a9859d22b806ab2d93cde37f5961457bd2a0e`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfefda86e4fa28b33f2d2cef255bfe31abc0ca3456b2dec7076e47376f397b6c`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ec9b75afd6d4e065c60a77490aa3477653a68de0876a26dc38c405b2ec9668`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:e2f6f5efebc83753060a5cba706cbeaa06e6286dfbef2f2fe90553be06ac9ec6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cd6084b972d634cc951ce015f81b8d9dcf607ff469eca68add9b371f2cc6083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2729696598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:286b8a1bd32d93129f2c880b31455c3e7698a3410f79080818a9bea4ed87b67b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:36:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:36:48 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:38:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:38:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:38:52 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:38:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7877e2093132135d0736339977fab38165007cd5a915c3845360152dca9ef9c4`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0fd646dc9583d9de3bc0368a258c5ca4fc34c347516e1faed2bcf0e5fb5df2`  
		Last Modified: Tue, 09 Feb 2021 21:03:23 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fa05efbb9d013622ad63a8e483b43df09c5ee738f99e73bcc57eaf5290f8a3`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d15a871c49181eb8884904ffc139e5d4889ef074a838e9f94b84bb229d5dfa`  
		Last Modified: Tue, 09 Feb 2021 21:09:03 GMT  
		Size: 290.4 MB (290420013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d16a7ee3b2395d0dfa6f59e6e9874c3b9e84e7c3785029aa4a473ec4a123a20`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e49c653c2c64cc3f43a9f218195b5164deaba8f4c0027d39176ffe8e314067`  
		Last Modified: Tue, 09 Feb 2021 21:03:20 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aaa63d20892b0a6024db1589b775e5a5b285651b446800aa6d6662550088bcb`  
		Last Modified: Tue, 09 Feb 2021 21:03:21 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:04b13ac89331c678ff2811805e9f40b2a5b766761d14c773b56fe78f0e777589
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:a545c92ec61392ca47d093fd296ab3f608594b03deec2a24073ca0cd1277b6ba
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6086150287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:788a9b87dc607fbd579944881426492e960624d9e12173b0c027e60b38bd898f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 09 Feb 2021 20:38:59 GMT
ENV MONGO_VERSION=4.2.12
# Tue, 09 Feb 2021 20:39:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.12-signed.msi
# Tue, 09 Feb 2021 20:39:01 GMT
ENV MONGO_DOWNLOAD_SHA256=68f45719faf62cc9274c2f86373cef1ab84442fcb1f60bd61af2cb8d955f5458
# Tue, 09 Feb 2021 20:41:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 09 Feb 2021 20:41:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 09 Feb 2021 20:42:00 GMT
EXPOSE 27017
# Tue, 09 Feb 2021 20:42:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39600dd254ee2f8c385ac8abe438b3026ecfbc59fd4cede8baf9e49755ccf42f`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037dc38ff67e44e8539b98a2697a944c4b5dc84f47cbd6fcb2d889bf63f22458`  
		Last Modified: Tue, 09 Feb 2021 21:09:18 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9629bcb0abfe902504f9af494c22f945caa0d508c4abdfcca98d2782137ca419`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77845301e844a5b2137f771aea4bbe82fdb2c4b773a6ed0fb9222a0545d7c05`  
		Last Modified: Tue, 09 Feb 2021 21:14:43 GMT  
		Size: 291.1 MB (291127624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b761c8dba0c8256e4ce171503a9859d22b806ab2d93cde37f5961457bd2a0e`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfefda86e4fa28b33f2d2cef255bfe31abc0ca3456b2dec7076e47376f397b6c`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ec9b75afd6d4e065c60a77490aa3477653a68de0876a26dc38c405b2ec9668`  
		Last Modified: Tue, 09 Feb 2021 21:09:16 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4`

```console
$ docker pull mongo@sha256:9de54e2d0703904e5005a5c8f04cd56d83475edd8c8f441c7f3ca0c71c40c6e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.4` - linux; amd64

```console
$ docker pull mongo@sha256:5f9f9576c14a6f2e8c0c37450ad2225bddc42f63206f47fcae55c07d3ec5a6f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175098371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8264a857eba49a59ffba446beaa10e6f3a5c5b775c78b656aee476c8dc5c426`
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
# Wed, 17 Feb 2021 00:17:20 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:17:44 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:17:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:17:45 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:45 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:46 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:46 GMT
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
	-	`sha256:ebe4a7cd312628ff7eacb3958534f8f2b9b0a257b60e5aba2f8aec2ed6efc194`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343b2aa1fbbf575c12309d7070a089d6078ef3feb189972deb66c4f00bbd3aae`  
		Last Modified: Wed, 17 Feb 2021 00:18:54 GMT  
		Size: 139.6 MB (139561770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059fcf556d9315fb2f0bf2d895ca3053f7ca80418cb072b14f4d28b37af7579c`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c03e6ca912dc9f44b28670dcd8550b4eefbf73e1ec98f8c6d9407437496fbb`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:148115913437e8cc80492ac8227d74f452df88a85f5b3c944df3333daca8a435
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167513450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdc664d8cc1ec10ee0bc6511cead7c8ed640c7668062b2b325013a8165a1dab`
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
# Wed, 17 Feb 2021 00:14:15 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:14:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:14:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:14:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:14:58 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:14:58 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:15:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:15:00 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:15:01 GMT
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
	-	`sha256:b8e66fb30288214eb4c3f674fa3eb920eb41b117dd6ebf701bb22c8e85a8a728`  
		Last Modified: Wed, 17 Feb 2021 00:15:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaf34239126e893b75ad3585d7101f72624fd924a7f9fa711edd4aef1c7361`  
		Last Modified: Wed, 17 Feb 2021 00:16:29 GMT  
		Size: 135.7 MB (135742747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc1d5f5c39bc895a9ef14486c88ea33744321b894ba89b91c87284db75d3b7`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac81acd76c1faf85f7439ff1fe66aa7f03c84f1fe98ab9b143dcd2186af9e82`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; s390x

```console
$ docker pull mongo@sha256:cdf3e3a8fca1c8eebd9cfbca2966b1e03123febbcf6e93e2c88d043594d186a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169033417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baed376d89d8d4c06a45ca93bd64872fed74a308e9fc4754ced821089bdac9e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:27 GMT
ADD file:20133497018a85bea4420c8f220dd76e39b9bb25c81a331c204d7ea02d984d7d in / 
# Thu, 04 Mar 2021 02:47:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:31 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:35:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 03:35:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:35:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 03:35:57 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 03:36:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 03:36:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 03:36:10 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 03:36:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 03:36:12 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 03:36:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 03:36:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 03:36:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 03:36:36 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 03:36:36 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 03:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 03:36:36 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 03:36:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e2e05228c9769d80c0b892ff4534a82c87ffa32b4d87105d6715d02dc13b73dd`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 25.4 MB (25380798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0697554175a1fb68cbf41f1990c4b35faab0569426e5f2bc7a8931cd581b85`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c776b6e8daba94835d2c0f86fb70da1005080f579b01d72ec542c138ce380d89`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd7545e09b022408db3ed3946b9e288e773c4872e5f2677367154a873397582`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0f57759a1811b0968b2d78f0d1cd4df3c94f877527ca8d1bd95f3f763b6271`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 2.7 MB (2707952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388c8556d6c330b583a5497cffb24f1c5ede4006cd663e3be38d6b1affe29ae`  
		Last Modified: Thu, 04 Mar 2021 03:36:57 GMT  
		Size: 5.7 MB (5747242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa17efe813310ff75b305c4adceb589f19a9e36c06b9c23938a7391379897f5`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ad0db5b17d4bd1d1635be0a4ed2cba7cf1920bd3db16c4109ddf3de49a523b`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd835e634633cd70eb29b0c4e871e9b3128314f1723920b5f547230fcecedf4`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46b6820f0b0e29a4c81b31b7a59a14f241b10c3de1ff56a437d7b411fbfc53`  
		Last Modified: Thu, 04 Mar 2021 03:37:11 GMT  
		Size: 135.2 MB (135188104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82bcaf445b47eeae3d6ea2e9960e6af68d4dd6d69869d94f3652e1abf9fb7d6`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f76478d141e7e3350e47a0726491ffb3f1d6dcaadc85de60bf47d336f8ca701`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4`

```console
$ docker pull mongo@sha256:9de54e2d0703904e5005a5c8f04cd56d83475edd8c8f441c7f3ca0c71c40c6e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.4.4` - linux; amd64

```console
$ docker pull mongo@sha256:5f9f9576c14a6f2e8c0c37450ad2225bddc42f63206f47fcae55c07d3ec5a6f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175098371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8264a857eba49a59ffba446beaa10e6f3a5c5b775c78b656aee476c8dc5c426`
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
# Wed, 17 Feb 2021 00:17:20 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:17:44 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:17:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:17:45 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:45 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:46 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:46 GMT
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
	-	`sha256:ebe4a7cd312628ff7eacb3958534f8f2b9b0a257b60e5aba2f8aec2ed6efc194`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343b2aa1fbbf575c12309d7070a089d6078ef3feb189972deb66c4f00bbd3aae`  
		Last Modified: Wed, 17 Feb 2021 00:18:54 GMT  
		Size: 139.6 MB (139561770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059fcf556d9315fb2f0bf2d895ca3053f7ca80418cb072b14f4d28b37af7579c`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c03e6ca912dc9f44b28670dcd8550b4eefbf73e1ec98f8c6d9407437496fbb`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:148115913437e8cc80492ac8227d74f452df88a85f5b3c944df3333daca8a435
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167513450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdc664d8cc1ec10ee0bc6511cead7c8ed640c7668062b2b325013a8165a1dab`
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
# Wed, 17 Feb 2021 00:14:15 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:14:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:14:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:14:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:14:58 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:14:58 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:15:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:15:00 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:15:01 GMT
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
	-	`sha256:b8e66fb30288214eb4c3f674fa3eb920eb41b117dd6ebf701bb22c8e85a8a728`  
		Last Modified: Wed, 17 Feb 2021 00:15:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaf34239126e893b75ad3585d7101f72624fd924a7f9fa711edd4aef1c7361`  
		Last Modified: Wed, 17 Feb 2021 00:16:29 GMT  
		Size: 135.7 MB (135742747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc1d5f5c39bc895a9ef14486c88ea33744321b894ba89b91c87284db75d3b7`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac81acd76c1faf85f7439ff1fe66aa7f03c84f1fe98ab9b143dcd2186af9e82`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4` - linux; s390x

```console
$ docker pull mongo@sha256:cdf3e3a8fca1c8eebd9cfbca2966b1e03123febbcf6e93e2c88d043594d186a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169033417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baed376d89d8d4c06a45ca93bd64872fed74a308e9fc4754ced821089bdac9e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:27 GMT
ADD file:20133497018a85bea4420c8f220dd76e39b9bb25c81a331c204d7ea02d984d7d in / 
# Thu, 04 Mar 2021 02:47:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:31 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:35:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 03:35:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:35:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 03:35:57 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 03:36:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 03:36:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 03:36:10 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 03:36:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 03:36:12 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 03:36:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 03:36:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 03:36:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 03:36:36 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 03:36:36 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 03:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 03:36:36 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 03:36:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e2e05228c9769d80c0b892ff4534a82c87ffa32b4d87105d6715d02dc13b73dd`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 25.4 MB (25380798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0697554175a1fb68cbf41f1990c4b35faab0569426e5f2bc7a8931cd581b85`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c776b6e8daba94835d2c0f86fb70da1005080f579b01d72ec542c138ce380d89`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd7545e09b022408db3ed3946b9e288e773c4872e5f2677367154a873397582`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0f57759a1811b0968b2d78f0d1cd4df3c94f877527ca8d1bd95f3f763b6271`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 2.7 MB (2707952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388c8556d6c330b583a5497cffb24f1c5ede4006cd663e3be38d6b1affe29ae`  
		Last Modified: Thu, 04 Mar 2021 03:36:57 GMT  
		Size: 5.7 MB (5747242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa17efe813310ff75b305c4adceb589f19a9e36c06b9c23938a7391379897f5`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ad0db5b17d4bd1d1635be0a4ed2cba7cf1920bd3db16c4109ddf3de49a523b`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd835e634633cd70eb29b0c4e871e9b3128314f1723920b5f547230fcecedf4`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46b6820f0b0e29a4c81b31b7a59a14f241b10c3de1ff56a437d7b411fbfc53`  
		Last Modified: Thu, 04 Mar 2021 03:37:11 GMT  
		Size: 135.2 MB (135188104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82bcaf445b47eeae3d6ea2e9960e6af68d4dd6d69869d94f3652e1abf9fb7d6`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f76478d141e7e3350e47a0726491ffb3f1d6dcaadc85de60bf47d336f8ca701`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4-bionic`

```console
$ docker pull mongo@sha256:dd0e689272b9a96c5a38053366056bd18497d63a54fe6a243fb8922b90d7b7bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:5f9f9576c14a6f2e8c0c37450ad2225bddc42f63206f47fcae55c07d3ec5a6f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175098371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8264a857eba49a59ffba446beaa10e6f3a5c5b775c78b656aee476c8dc5c426`
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
# Wed, 17 Feb 2021 00:17:20 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:17:44 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:17:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:17:45 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:45 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:46 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:46 GMT
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
	-	`sha256:ebe4a7cd312628ff7eacb3958534f8f2b9b0a257b60e5aba2f8aec2ed6efc194`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343b2aa1fbbf575c12309d7070a089d6078ef3feb189972deb66c4f00bbd3aae`  
		Last Modified: Wed, 17 Feb 2021 00:18:54 GMT  
		Size: 139.6 MB (139561770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059fcf556d9315fb2f0bf2d895ca3053f7ca80418cb072b14f4d28b37af7579c`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c03e6ca912dc9f44b28670dcd8550b4eefbf73e1ec98f8c6d9407437496fbb`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:148115913437e8cc80492ac8227d74f452df88a85f5b3c944df3333daca8a435
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167513450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdc664d8cc1ec10ee0bc6511cead7c8ed640c7668062b2b325013a8165a1dab`
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
# Wed, 17 Feb 2021 00:14:15 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:14:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:14:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:14:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:14:58 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:14:58 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:15:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:15:00 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:15:01 GMT
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
	-	`sha256:b8e66fb30288214eb4c3f674fa3eb920eb41b117dd6ebf701bb22c8e85a8a728`  
		Last Modified: Wed, 17 Feb 2021 00:15:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaf34239126e893b75ad3585d7101f72624fd924a7f9fa711edd4aef1c7361`  
		Last Modified: Wed, 17 Feb 2021 00:16:29 GMT  
		Size: 135.7 MB (135742747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc1d5f5c39bc895a9ef14486c88ea33744321b894ba89b91c87284db75d3b7`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac81acd76c1faf85f7439ff1fe66aa7f03c84f1fe98ab9b143dcd2186af9e82`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:cdf3e3a8fca1c8eebd9cfbca2966b1e03123febbcf6e93e2c88d043594d186a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169033417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baed376d89d8d4c06a45ca93bd64872fed74a308e9fc4754ced821089bdac9e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:27 GMT
ADD file:20133497018a85bea4420c8f220dd76e39b9bb25c81a331c204d7ea02d984d7d in / 
# Thu, 04 Mar 2021 02:47:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:31 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:35:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 03:35:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:35:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 03:35:57 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 03:36:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 03:36:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 03:36:10 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 03:36:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 03:36:12 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 03:36:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 03:36:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 03:36:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 03:36:36 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 03:36:36 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 03:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 03:36:36 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 03:36:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e2e05228c9769d80c0b892ff4534a82c87ffa32b4d87105d6715d02dc13b73dd`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 25.4 MB (25380798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0697554175a1fb68cbf41f1990c4b35faab0569426e5f2bc7a8931cd581b85`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c776b6e8daba94835d2c0f86fb70da1005080f579b01d72ec542c138ce380d89`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd7545e09b022408db3ed3946b9e288e773c4872e5f2677367154a873397582`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0f57759a1811b0968b2d78f0d1cd4df3c94f877527ca8d1bd95f3f763b6271`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 2.7 MB (2707952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388c8556d6c330b583a5497cffb24f1c5ede4006cd663e3be38d6b1affe29ae`  
		Last Modified: Thu, 04 Mar 2021 03:36:57 GMT  
		Size: 5.7 MB (5747242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa17efe813310ff75b305c4adceb589f19a9e36c06b9c23938a7391379897f5`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ad0db5b17d4bd1d1635be0a4ed2cba7cf1920bd3db16c4109ddf3de49a523b`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd835e634633cd70eb29b0c4e871e9b3128314f1723920b5f547230fcecedf4`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46b6820f0b0e29a4c81b31b7a59a14f241b10c3de1ff56a437d7b411fbfc53`  
		Last Modified: Thu, 04 Mar 2021 03:37:11 GMT  
		Size: 135.2 MB (135188104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82bcaf445b47eeae3d6ea2e9960e6af68d4dd6d69869d94f3652e1abf9fb7d6`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f76478d141e7e3350e47a0726491ffb3f1d6dcaadc85de60bf47d336f8ca701`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4-windowsservercore`

```console
$ docker pull mongo@sha256:deb97f68bab1b34bd243bb314ad20664eaa2a4ce5a44ba32772d62b78037f9c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.4.4-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0e286e9a040887ff8a6db51a1fe8a86acfbc038920a9feeae38279735ff348f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:4.4.4-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:5fc68047e5e1b96aa1d123c1998be572034a26b329694b3fca7b98aeee426b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.4.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-bionic`

```console
$ docker pull mongo@sha256:dd0e689272b9a96c5a38053366056bd18497d63a54fe6a243fb8922b90d7b7bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:5f9f9576c14a6f2e8c0c37450ad2225bddc42f63206f47fcae55c07d3ec5a6f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175098371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8264a857eba49a59ffba446beaa10e6f3a5c5b775c78b656aee476c8dc5c426`
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
# Wed, 17 Feb 2021 00:17:20 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:17:44 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:17:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:17:45 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:45 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:46 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:46 GMT
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
	-	`sha256:ebe4a7cd312628ff7eacb3958534f8f2b9b0a257b60e5aba2f8aec2ed6efc194`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343b2aa1fbbf575c12309d7070a089d6078ef3feb189972deb66c4f00bbd3aae`  
		Last Modified: Wed, 17 Feb 2021 00:18:54 GMT  
		Size: 139.6 MB (139561770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059fcf556d9315fb2f0bf2d895ca3053f7ca80418cb072b14f4d28b37af7579c`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c03e6ca912dc9f44b28670dcd8550b4eefbf73e1ec98f8c6d9407437496fbb`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:148115913437e8cc80492ac8227d74f452df88a85f5b3c944df3333daca8a435
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167513450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdc664d8cc1ec10ee0bc6511cead7c8ed640c7668062b2b325013a8165a1dab`
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
# Wed, 17 Feb 2021 00:14:15 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:14:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:14:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:14:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:14:58 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:14:58 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:15:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:15:00 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:15:01 GMT
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
	-	`sha256:b8e66fb30288214eb4c3f674fa3eb920eb41b117dd6ebf701bb22c8e85a8a728`  
		Last Modified: Wed, 17 Feb 2021 00:15:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaf34239126e893b75ad3585d7101f72624fd924a7f9fa711edd4aef1c7361`  
		Last Modified: Wed, 17 Feb 2021 00:16:29 GMT  
		Size: 135.7 MB (135742747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc1d5f5c39bc895a9ef14486c88ea33744321b894ba89b91c87284db75d3b7`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac81acd76c1faf85f7439ff1fe66aa7f03c84f1fe98ab9b143dcd2186af9e82`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:cdf3e3a8fca1c8eebd9cfbca2966b1e03123febbcf6e93e2c88d043594d186a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169033417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baed376d89d8d4c06a45ca93bd64872fed74a308e9fc4754ced821089bdac9e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:27 GMT
ADD file:20133497018a85bea4420c8f220dd76e39b9bb25c81a331c204d7ea02d984d7d in / 
# Thu, 04 Mar 2021 02:47:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:31 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:35:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 03:35:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:35:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 03:35:57 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 03:36:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 03:36:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 03:36:10 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 03:36:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 03:36:12 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 03:36:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 03:36:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 03:36:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 03:36:36 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 03:36:36 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 03:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 03:36:36 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 03:36:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e2e05228c9769d80c0b892ff4534a82c87ffa32b4d87105d6715d02dc13b73dd`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 25.4 MB (25380798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0697554175a1fb68cbf41f1990c4b35faab0569426e5f2bc7a8931cd581b85`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c776b6e8daba94835d2c0f86fb70da1005080f579b01d72ec542c138ce380d89`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd7545e09b022408db3ed3946b9e288e773c4872e5f2677367154a873397582`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0f57759a1811b0968b2d78f0d1cd4df3c94f877527ca8d1bd95f3f763b6271`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 2.7 MB (2707952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388c8556d6c330b583a5497cffb24f1c5ede4006cd663e3be38d6b1affe29ae`  
		Last Modified: Thu, 04 Mar 2021 03:36:57 GMT  
		Size: 5.7 MB (5747242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa17efe813310ff75b305c4adceb589f19a9e36c06b9c23938a7391379897f5`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ad0db5b17d4bd1d1635be0a4ed2cba7cf1920bd3db16c4109ddf3de49a523b`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd835e634633cd70eb29b0c4e871e9b3128314f1723920b5f547230fcecedf4`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46b6820f0b0e29a4c81b31b7a59a14f241b10c3de1ff56a437d7b411fbfc53`  
		Last Modified: Thu, 04 Mar 2021 03:37:11 GMT  
		Size: 135.2 MB (135188104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82bcaf445b47eeae3d6ea2e9960e6af68d4dd6d69869d94f3652e1abf9fb7d6`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f76478d141e7e3350e47a0726491ffb3f1d6dcaadc85de60bf47d336f8ca701`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore`

```console
$ docker pull mongo@sha256:deb97f68bab1b34bd243bb314ad20664eaa2a4ce5a44ba32772d62b78037f9c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.4-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0e286e9a040887ff8a6db51a1fe8a86acfbc038920a9feeae38279735ff348f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:4.4-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:5fc68047e5e1b96aa1d123c1998be572034a26b329694b3fca7b98aeee426b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:4.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:dd0e689272b9a96c5a38053366056bd18497d63a54fe6a243fb8922b90d7b7bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:5f9f9576c14a6f2e8c0c37450ad2225bddc42f63206f47fcae55c07d3ec5a6f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175098371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8264a857eba49a59ffba446beaa10e6f3a5c5b775c78b656aee476c8dc5c426`
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
# Wed, 17 Feb 2021 00:17:20 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:17:44 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:17:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:17:45 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:45 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:46 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:46 GMT
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
	-	`sha256:ebe4a7cd312628ff7eacb3958534f8f2b9b0a257b60e5aba2f8aec2ed6efc194`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343b2aa1fbbf575c12309d7070a089d6078ef3feb189972deb66c4f00bbd3aae`  
		Last Modified: Wed, 17 Feb 2021 00:18:54 GMT  
		Size: 139.6 MB (139561770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059fcf556d9315fb2f0bf2d895ca3053f7ca80418cb072b14f4d28b37af7579c`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c03e6ca912dc9f44b28670dcd8550b4eefbf73e1ec98f8c6d9407437496fbb`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:148115913437e8cc80492ac8227d74f452df88a85f5b3c944df3333daca8a435
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167513450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdc664d8cc1ec10ee0bc6511cead7c8ed640c7668062b2b325013a8165a1dab`
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
# Wed, 17 Feb 2021 00:14:15 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:14:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:14:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:14:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:14:58 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:14:58 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:15:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:15:00 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:15:01 GMT
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
	-	`sha256:b8e66fb30288214eb4c3f674fa3eb920eb41b117dd6ebf701bb22c8e85a8a728`  
		Last Modified: Wed, 17 Feb 2021 00:15:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaf34239126e893b75ad3585d7101f72624fd924a7f9fa711edd4aef1c7361`  
		Last Modified: Wed, 17 Feb 2021 00:16:29 GMT  
		Size: 135.7 MB (135742747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc1d5f5c39bc895a9ef14486c88ea33744321b894ba89b91c87284db75d3b7`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac81acd76c1faf85f7439ff1fe66aa7f03c84f1fe98ab9b143dcd2186af9e82`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:cdf3e3a8fca1c8eebd9cfbca2966b1e03123febbcf6e93e2c88d043594d186a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169033417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baed376d89d8d4c06a45ca93bd64872fed74a308e9fc4754ced821089bdac9e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:27 GMT
ADD file:20133497018a85bea4420c8f220dd76e39b9bb25c81a331c204d7ea02d984d7d in / 
# Thu, 04 Mar 2021 02:47:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:31 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:35:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 03:35:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:35:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 03:35:57 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 03:36:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 03:36:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 03:36:10 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 03:36:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 03:36:12 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 03:36:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 03:36:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 03:36:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 03:36:36 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 03:36:36 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 03:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 03:36:36 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 03:36:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e2e05228c9769d80c0b892ff4534a82c87ffa32b4d87105d6715d02dc13b73dd`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 25.4 MB (25380798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0697554175a1fb68cbf41f1990c4b35faab0569426e5f2bc7a8931cd581b85`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c776b6e8daba94835d2c0f86fb70da1005080f579b01d72ec542c138ce380d89`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd7545e09b022408db3ed3946b9e288e773c4872e5f2677367154a873397582`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0f57759a1811b0968b2d78f0d1cd4df3c94f877527ca8d1bd95f3f763b6271`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 2.7 MB (2707952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388c8556d6c330b583a5497cffb24f1c5ede4006cd663e3be38d6b1affe29ae`  
		Last Modified: Thu, 04 Mar 2021 03:36:57 GMT  
		Size: 5.7 MB (5747242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa17efe813310ff75b305c4adceb589f19a9e36c06b9c23938a7391379897f5`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ad0db5b17d4bd1d1635be0a4ed2cba7cf1920bd3db16c4109ddf3de49a523b`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd835e634633cd70eb29b0c4e871e9b3128314f1723920b5f547230fcecedf4`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46b6820f0b0e29a4c81b31b7a59a14f241b10c3de1ff56a437d7b411fbfc53`  
		Last Modified: Thu, 04 Mar 2021 03:37:11 GMT  
		Size: 135.2 MB (135188104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82bcaf445b47eeae3d6ea2e9960e6af68d4dd6d69869d94f3652e1abf9fb7d6`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f76478d141e7e3350e47a0726491ffb3f1d6dcaadc85de60bf47d336f8ca701`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:deb97f68bab1b34bd243bb314ad20664eaa2a4ce5a44ba32772d62b78037f9c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:4-windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0e286e9a040887ff8a6db51a1fe8a86acfbc038920a9feeae38279735ff348f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:5fc68047e5e1b96aa1d123c1998be572034a26b329694b3fca7b98aeee426b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:dd0e689272b9a96c5a38053366056bd18497d63a54fe6a243fb8922b90d7b7bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:5f9f9576c14a6f2e8c0c37450ad2225bddc42f63206f47fcae55c07d3ec5a6f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175098371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8264a857eba49a59ffba446beaa10e6f3a5c5b775c78b656aee476c8dc5c426`
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
# Wed, 17 Feb 2021 00:17:20 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:17:44 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:17:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:17:45 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:45 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:46 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:46 GMT
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
	-	`sha256:ebe4a7cd312628ff7eacb3958534f8f2b9b0a257b60e5aba2f8aec2ed6efc194`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343b2aa1fbbf575c12309d7070a089d6078ef3feb189972deb66c4f00bbd3aae`  
		Last Modified: Wed, 17 Feb 2021 00:18:54 GMT  
		Size: 139.6 MB (139561770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059fcf556d9315fb2f0bf2d895ca3053f7ca80418cb072b14f4d28b37af7579c`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c03e6ca912dc9f44b28670dcd8550b4eefbf73e1ec98f8c6d9407437496fbb`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:148115913437e8cc80492ac8227d74f452df88a85f5b3c944df3333daca8a435
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167513450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdc664d8cc1ec10ee0bc6511cead7c8ed640c7668062b2b325013a8165a1dab`
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
# Wed, 17 Feb 2021 00:14:15 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:14:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:14:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:14:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:14:58 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:14:58 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:15:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:15:00 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:15:01 GMT
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
	-	`sha256:b8e66fb30288214eb4c3f674fa3eb920eb41b117dd6ebf701bb22c8e85a8a728`  
		Last Modified: Wed, 17 Feb 2021 00:15:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaf34239126e893b75ad3585d7101f72624fd924a7f9fa711edd4aef1c7361`  
		Last Modified: Wed, 17 Feb 2021 00:16:29 GMT  
		Size: 135.7 MB (135742747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc1d5f5c39bc895a9ef14486c88ea33744321b894ba89b91c87284db75d3b7`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac81acd76c1faf85f7439ff1fe66aa7f03c84f1fe98ab9b143dcd2186af9e82`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:cdf3e3a8fca1c8eebd9cfbca2966b1e03123febbcf6e93e2c88d043594d186a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169033417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baed376d89d8d4c06a45ca93bd64872fed74a308e9fc4754ced821089bdac9e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:27 GMT
ADD file:20133497018a85bea4420c8f220dd76e39b9bb25c81a331c204d7ea02d984d7d in / 
# Thu, 04 Mar 2021 02:47:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:31 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:35:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 03:35:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:35:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 03:35:57 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 03:36:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 03:36:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 03:36:10 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 03:36:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 03:36:12 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 03:36:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 03:36:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 03:36:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 03:36:36 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 03:36:36 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 03:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 03:36:36 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 03:36:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e2e05228c9769d80c0b892ff4534a82c87ffa32b4d87105d6715d02dc13b73dd`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 25.4 MB (25380798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0697554175a1fb68cbf41f1990c4b35faab0569426e5f2bc7a8931cd581b85`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c776b6e8daba94835d2c0f86fb70da1005080f579b01d72ec542c138ce380d89`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd7545e09b022408db3ed3946b9e288e773c4872e5f2677367154a873397582`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0f57759a1811b0968b2d78f0d1cd4df3c94f877527ca8d1bd95f3f763b6271`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 2.7 MB (2707952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388c8556d6c330b583a5497cffb24f1c5ede4006cd663e3be38d6b1affe29ae`  
		Last Modified: Thu, 04 Mar 2021 03:36:57 GMT  
		Size: 5.7 MB (5747242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa17efe813310ff75b305c4adceb589f19a9e36c06b9c23938a7391379897f5`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ad0db5b17d4bd1d1635be0a4ed2cba7cf1920bd3db16c4109ddf3de49a523b`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd835e634633cd70eb29b0c4e871e9b3128314f1723920b5f547230fcecedf4`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46b6820f0b0e29a4c81b31b7a59a14f241b10c3de1ff56a437d7b411fbfc53`  
		Last Modified: Thu, 04 Mar 2021 03:37:11 GMT  
		Size: 135.2 MB (135188104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82bcaf445b47eeae3d6ea2e9960e6af68d4dd6d69869d94f3652e1abf9fb7d6`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f76478d141e7e3350e47a0726491ffb3f1d6dcaadc85de60bf47d336f8ca701`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:9de54e2d0703904e5005a5c8f04cd56d83475edd8c8f441c7f3ca0c71c40c6e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:5f9f9576c14a6f2e8c0c37450ad2225bddc42f63206f47fcae55c07d3ec5a6f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175098371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8264a857eba49a59ffba446beaa10e6f3a5c5b775c78b656aee476c8dc5c426`
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
# Wed, 17 Feb 2021 00:17:20 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:17:44 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:17:45 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:17:45 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:17:45 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:17:46 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:17:46 GMT
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
	-	`sha256:ebe4a7cd312628ff7eacb3958534f8f2b9b0a257b60e5aba2f8aec2ed6efc194`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343b2aa1fbbf575c12309d7070a089d6078ef3feb189972deb66c4f00bbd3aae`  
		Last Modified: Wed, 17 Feb 2021 00:18:54 GMT  
		Size: 139.6 MB (139561770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059fcf556d9315fb2f0bf2d895ca3053f7ca80418cb072b14f4d28b37af7579c`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c03e6ca912dc9f44b28670dcd8550b4eefbf73e1ec98f8c6d9407437496fbb`  
		Last Modified: Wed, 17 Feb 2021 00:18:29 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:148115913437e8cc80492ac8227d74f452df88a85f5b3c944df3333daca8a435
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167513450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdc664d8cc1ec10ee0bc6511cead7c8ed640c7668062b2b325013a8165a1dab`
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
# Wed, 17 Feb 2021 00:14:15 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 17 Feb 2021 00:14:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 17 Feb 2021 00:14:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 17 Feb 2021 00:14:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 17 Feb 2021 00:14:58 GMT
VOLUME [/data/db /data/configdb]
# Wed, 17 Feb 2021 00:14:58 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Wed, 17 Feb 2021 00:15:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Feb 2021 00:15:00 GMT
EXPOSE 27017
# Wed, 17 Feb 2021 00:15:01 GMT
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
	-	`sha256:b8e66fb30288214eb4c3f674fa3eb920eb41b117dd6ebf701bb22c8e85a8a728`  
		Last Modified: Wed, 17 Feb 2021 00:15:59 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbaf34239126e893b75ad3585d7101f72624fd924a7f9fa711edd4aef1c7361`  
		Last Modified: Wed, 17 Feb 2021 00:16:29 GMT  
		Size: 135.7 MB (135742747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecc1d5f5c39bc895a9ef14486c88ea33744321b894ba89b91c87284db75d3b7`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac81acd76c1faf85f7439ff1fe66aa7f03c84f1fe98ab9b143dcd2186af9e82`  
		Last Modified: Wed, 17 Feb 2021 00:15:58 GMT  
		Size: 4.4 KB (4427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:cdf3e3a8fca1c8eebd9cfbca2966b1e03123febbcf6e93e2c88d043594d186a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169033417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baed376d89d8d4c06a45ca93bd64872fed74a308e9fc4754ced821089bdac9e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:47:27 GMT
ADD file:20133497018a85bea4420c8f220dd76e39b9bb25c81a331c204d7ea02d984d7d in / 
# Thu, 04 Mar 2021 02:47:29 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:47:30 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:47:31 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:47:31 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 03:35:50 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 03:35:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 03:35:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 03:35:57 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 03:36:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 03:36:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 03:36:10 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 03:36:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 03:36:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 03:36:11 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 03:36:12 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 03:36:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 03:36:31 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 03:36:36 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 03:36:36 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 03:36:36 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 03:36:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 03:36:36 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 03:36:37 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:e2e05228c9769d80c0b892ff4534a82c87ffa32b4d87105d6715d02dc13b73dd`  
		Last Modified: Mon, 01 Mar 2021 16:20:21 GMT  
		Size: 25.4 MB (25380798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0697554175a1fb68cbf41f1990c4b35faab0569426e5f2bc7a8931cd581b85`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c776b6e8daba94835d2c0f86fb70da1005080f579b01d72ec542c138ce380d89`  
		Last Modified: Thu, 04 Mar 2021 02:48:29 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd7545e09b022408db3ed3946b9e288e773c4872e5f2677367154a873397582`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0f57759a1811b0968b2d78f0d1cd4df3c94f877527ca8d1bd95f3f763b6271`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 2.7 MB (2707952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388c8556d6c330b583a5497cffb24f1c5ede4006cd663e3be38d6b1affe29ae`  
		Last Modified: Thu, 04 Mar 2021 03:36:57 GMT  
		Size: 5.7 MB (5747242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa17efe813310ff75b305c4adceb589f19a9e36c06b9c23938a7391379897f5`  
		Last Modified: Thu, 04 Mar 2021 03:36:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ad0db5b17d4bd1d1635be0a4ed2cba7cf1920bd3db16c4109ddf3de49a523b`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd835e634633cd70eb29b0c4e871e9b3128314f1723920b5f547230fcecedf4`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46b6820f0b0e29a4c81b31b7a59a14f241b10c3de1ff56a437d7b411fbfc53`  
		Last Modified: Thu, 04 Mar 2021 03:37:11 GMT  
		Size: 135.2 MB (135188104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82bcaf445b47eeae3d6ea2e9960e6af68d4dd6d69869d94f3652e1abf9fb7d6`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f76478d141e7e3350e47a0726491ffb3f1d6dcaadc85de60bf47d336f8ca701`  
		Last Modified: Thu, 04 Mar 2021 03:36:54 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:deb97f68bab1b34bd243bb314ad20664eaa2a4ce5a44ba32772d62b78037f9c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `mongo:windowsservercore` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:0e286e9a040887ff8a6db51a1fe8a86acfbc038920a9feeae38279735ff348f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1757; amd64

```console
$ docker pull mongo@sha256:7cdcc0eaad2054954a075fddc6cb411bf59947a187da8a5420d968ffc5a2669e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2679545750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39525f6db8351191aeb032f85d522c13a2562fd1964c1e3e49eab0c7925eaac8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:15:44 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:15:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:15:46 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:17:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:17:56 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:17:57 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:17:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db31180c577df72a9e777d749dacf99b5ecdce0c9bd9d36df11ac8d72bf3773`  
		Last Modified: Tue, 16 Feb 2021 23:22:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752b82972789fb70767bf1869cc48eed4ce5391808635cba762e02b2e18a3687`  
		Last Modified: Tue, 16 Feb 2021 23:22:21 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe010fb60f271aa127d31d04f0f836e92fae8dee7015b4321561a4bf0a367728`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9891f2e75b4221526d6dc82d8b2a55d9930d50ef08f918c904dc070e63729b26`  
		Last Modified: Tue, 16 Feb 2021 23:23:02 GMT  
		Size: 240.3 MB (240269074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598fb862351f0dfa456e89f92213200554d754611024a7a52feadd1aede10ea`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71c78704ab3eeed7485eff12a27749357ec7bc07964bd4b0e2d63396abbe88b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e373efc55de47a9f55060b4d0cf71eb63829800a23fff2e439100cddb2015b`  
		Last Modified: Tue, 16 Feb 2021 23:22:19 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:5fc68047e5e1b96aa1d123c1998be572034a26b329694b3fca7b98aeee426b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4225; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.4225; amd64

```console
$ docker pull mongo@sha256:4c615ee6ad2e49ea7e03ff18ecf8c91887774886bc2ad3231059ed60eb3b30bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6035965692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde2ddfbfff449dd7a3f5664eda531970945e7a8af5ec043e9ec218f83fcb4b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Tue, 16 Feb 2021 23:18:11 GMT
ENV MONGO_VERSION=4.4.4
# Tue, 16 Feb 2021 23:18:12 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Tue, 16 Feb 2021 23:18:13 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Tue, 16 Feb 2021 23:20:53 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Tue, 16 Feb 2021 23:20:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Feb 2021 23:20:56 GMT
EXPOSE 27017
# Tue, 16 Feb 2021 23:20:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1320340b1f82449ea2e4632b13724fecbb20b7032b686e1056f38f89cd5dcbf`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a1ea4f45daf70ca785bd0ef00c60eedb8747ee01deaa9b1d1e7cc6a858e40a`  
		Last Modified: Tue, 16 Feb 2021 23:23:24 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2afc0181b2607ff45d01f5ee393e5e0fd515568d8b37d8b80aa91a1054f688`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092f4eb963297bd6e1820ff7ed0d2878c8eda3262f985e9bd5e6605bc77947`  
		Last Modified: Tue, 16 Feb 2021 23:24:06 GMT  
		Size: 240.9 MB (240942834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f320ee577215bd0d1d605d7bbeeec252c4692a32e6f5bbca34e18e81b346b2`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6a0f59bda4b0e20eee324ee6efeca8f8c0387158741c0dbbbccda9873ce6a3`  
		Last Modified: Tue, 16 Feb 2021 23:23:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a09803bcc7824e67c94aac6a17d65b520560fb1440ffdce6345088c1bb22423`  
		Last Modified: Tue, 16 Feb 2021 23:23:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
