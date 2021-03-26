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
-	[`mongo:4.0.23`](#mongo4023)
-	[`mongo:4.0.23-windowsservercore`](#mongo4023-windowsservercore)
-	[`mongo:4.0.23-windowsservercore-1809`](#mongo4023-windowsservercore-1809)
-	[`mongo:4.0.23-windowsservercore-ltsc2016`](#mongo4023-windowsservercore-ltsc2016)
-	[`mongo:4.0.23-xenial`](#mongo4023-xenial)
-	[`mongo:4.2`](#mongo42)
-	[`mongo:4.2-bionic`](#mongo42-bionic)
-	[`mongo:4.2-windowsservercore`](#mongo42-windowsservercore)
-	[`mongo:4.2-windowsservercore-1809`](#mongo42-windowsservercore-1809)
-	[`mongo:4.2-windowsservercore-ltsc2016`](#mongo42-windowsservercore-ltsc2016)
-	[`mongo:4.2.13`](#mongo4213)
-	[`mongo:4.2.13-bionic`](#mongo4213-bionic)
-	[`mongo:4.2.13-windowsservercore`](#mongo4213-windowsservercore)
-	[`mongo:4.2.13-windowsservercore-1809`](#mongo4213-windowsservercore-1809)
-	[`mongo:4.2.13-windowsservercore-ltsc2016`](#mongo4213-windowsservercore-ltsc2016)
-	[`mongo:4.4`](#mongo44)
-	[`mongo:4.4-bionic`](#mongo44-bionic)
-	[`mongo:4.4-windowsservercore`](#mongo44-windowsservercore)
-	[`mongo:4.4-windowsservercore-1809`](#mongo44-windowsservercore-1809)
-	[`mongo:4.4-windowsservercore-ltsc2016`](#mongo44-windowsservercore-ltsc2016)
-	[`mongo:4.4.4`](#mongo444)
-	[`mongo:4.4.4-bionic`](#mongo444-bionic)
-	[`mongo:4.4.4-windowsservercore`](#mongo444-windowsservercore)
-	[`mongo:4.4.4-windowsservercore-1809`](#mongo444-windowsservercore-1809)
-	[`mongo:4.4.4-windowsservercore-ltsc2016`](#mongo444-windowsservercore-ltsc2016)
-	[`mongo:bionic`](#mongobionic)
-	[`mongo:latest`](#mongolatest)
-	[`mongo:windowsservercore`](#mongowindowsservercore)
-	[`mongo:windowsservercore-1809`](#mongowindowsservercore-1809)
-	[`mongo:windowsservercore-ltsc2016`](#mongowindowsservercore-ltsc2016)

## `mongo:3`

```console
$ docker pull mongo@sha256:b79495efbae684fbda5d03f37b56c8d15368448c16ecc535c0267ced6a8b9f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:8febed4c87baf95786587ad2447817330b0cae3c02c147783bb30ab6fe731894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6075da9d551ef7d97e29775dcb03ec32226215bfa717cb326ddff5ccffb56a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:00:30 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 26 Mar 2021 12:00:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_MAJOR=3.6
# Fri, 26 Mar 2021 12:00:35 GMT
ENV MONGO_VERSION=3.6.23
# Fri, 26 Mar 2021 12:00:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:03 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:06 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:07 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da17adcdc02155bd69d9074497e6e2ffc5b7609dcdaefb81bf8c514e63689027`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a7cfbb0a119f0188e96ef9b49c63202bbb3c8f944ceb0a1186cbdb31221dff`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0624b9494b00f365e76e7318938ee308ef477a8b9ad653bf954cf6c791526f`  
		Last Modified: Fri, 26 Mar 2021 12:06:22 GMT  
		Size: 119.4 MB (119408001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fe06b9f8d979969819b4fbd3d893ae9747ea813ccf8bf4136451424bd5bfe4`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7541bd7b951e5a0d33629df6e8fdc2ab801111ee7a4d12a0eb019fb0f97e98`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c206a1d258a0c69a65ba30c312699d1d40d427cfaee393868da6f684e6a68972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.0 MB (157955361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31951dc525ae227bfc43b0b137ea273f7e9d19b61d890d2160d05c7c14b99890`
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
# Mon, 22 Mar 2021 19:40:32 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:40:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:04 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:05 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:07 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:07 GMT
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
	-	`sha256:4323fbd86340c57754c90058655613ba9aff6e054d6205519d5c6f65ed8d1d5e`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b780180bdd00bedf065b80a3dedda8d180d28660f90ddbfeae0c863b4ce090b`  
		Last Modified: Mon, 22 Mar 2021 19:43:00 GMT  
		Size: 113.4 MB (113379732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810e7643ed985ded5e60ff7e79e1e422390da8875e330da74d7e879a57e7c912`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c766c03ca1ae0eee35c4baff837a94ed0b5985665ee3baba01b7107733e1f3`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:63731590e62366f30a5d83b24987f6b71fa886f2c81eb52fd8fcee62396ef448
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692269073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7ed3b78d40c11e1b47f6c3fb27275c3289271e69f2d4946166e26ef3028972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:15:23 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:15:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:17:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:17:38 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:17:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7125fbbf1426092fe6933ef492b330859c33df4c223e56391f89b42b16e045ee`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8398f134d3c378d17b050bfd4b64beb85a05e2e7596864eb802d049503172f3f`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e19cf7c338f75657e10dedb236bf941729dedb6c1909f49054ee5e8650eaf2e`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55501c2e78abcdc12785db0e7045f1fc816427a651439a2d96fdba261ccd956`  
		Last Modified: Mon, 22 Mar 2021 19:29:36 GMT  
		Size: 230.7 MB (230724749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c33cf9ff3dc2f3d9ac2b6d85f2dee0698cbdc41b74d1aca2001b752c823a297`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f2da1ce568bdb909af7b2eddec2c8405ed83a8e8ed87c3a99caf2a61c7e9d`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7c6bf198ad8a3fb8a3879796caac6cd559bc27cd0ec1667e9a1d69b173a1b`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:003d7796e5615a09631a01bb00ee2f772461eee132da5480c2dde3002018c65d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6028346497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2001dc86ca184f18a58ce56c979d40f453090a77e027c4300aaa8e600da36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:17:52 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:17:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:17:54 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:21:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:21:08 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c5392547fce8ffc9f2ca8bd53dd13325b8a9811d908d79bcf21e264003526`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f191de5d0f746b5acabb63d0e0e4c4979a356786c93070054fc532e99390d6f0`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394051376831027d2cd58c3df5b3d5ce6c1645488f18b51247fa0620f60281f`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee498fd2a3866142f4d271b5136d20fdd3be3e29e733b7d48d78a9a645132f`  
		Last Modified: Mon, 22 Mar 2021 19:34:20 GMT  
		Size: 231.4 MB (231425773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbc0ee3c51f0dd7f1f0fc9dc5ce6070073867ada02455b5414ea5f1b2afe358`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edded4e2d6084db86ea9d144b0640c355350da1b275aaaa6e0e5dac18046c4e`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e843513a6cccd3ab12a8ba4fa1f5dcc8bf5e2e2d0fe68f9a831421890ae529`  
		Last Modified: Mon, 22 Mar 2021 19:29:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:7ddbaa2f3aff5d6d10af75479604f1f1fccf47cfea95a17e9d3947c74ee11f59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:3-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:63731590e62366f30a5d83b24987f6b71fa886f2c81eb52fd8fcee62396ef448
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692269073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7ed3b78d40c11e1b47f6c3fb27275c3289271e69f2d4946166e26ef3028972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:15:23 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:15:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:17:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:17:38 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:17:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7125fbbf1426092fe6933ef492b330859c33df4c223e56391f89b42b16e045ee`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8398f134d3c378d17b050bfd4b64beb85a05e2e7596864eb802d049503172f3f`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e19cf7c338f75657e10dedb236bf941729dedb6c1909f49054ee5e8650eaf2e`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55501c2e78abcdc12785db0e7045f1fc816427a651439a2d96fdba261ccd956`  
		Last Modified: Mon, 22 Mar 2021 19:29:36 GMT  
		Size: 230.7 MB (230724749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c33cf9ff3dc2f3d9ac2b6d85f2dee0698cbdc41b74d1aca2001b752c823a297`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f2da1ce568bdb909af7b2eddec2c8405ed83a8e8ed87c3a99caf2a61c7e9d`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7c6bf198ad8a3fb8a3879796caac6cd559bc27cd0ec1667e9a1d69b173a1b`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:003d7796e5615a09631a01bb00ee2f772461eee132da5480c2dde3002018c65d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6028346497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2001dc86ca184f18a58ce56c979d40f453090a77e027c4300aaa8e600da36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:17:52 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:17:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:17:54 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:21:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:21:08 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c5392547fce8ffc9f2ca8bd53dd13325b8a9811d908d79bcf21e264003526`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f191de5d0f746b5acabb63d0e0e4c4979a356786c93070054fc532e99390d6f0`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394051376831027d2cd58c3df5b3d5ce6c1645488f18b51247fa0620f60281f`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee498fd2a3866142f4d271b5136d20fdd3be3e29e733b7d48d78a9a645132f`  
		Last Modified: Mon, 22 Mar 2021 19:34:20 GMT  
		Size: 231.4 MB (231425773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbc0ee3c51f0dd7f1f0fc9dc5ce6070073867ada02455b5414ea5f1b2afe358`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edded4e2d6084db86ea9d144b0640c355350da1b275aaaa6e0e5dac18046c4e`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e843513a6cccd3ab12a8ba4fa1f5dcc8bf5e2e2d0fe68f9a831421890ae529`  
		Last Modified: Mon, 22 Mar 2021 19:29:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:1d0a12f8d1a4886a50245fa6f59f76b128869b8838f928adcd606bb1f393116a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:63731590e62366f30a5d83b24987f6b71fa886f2c81eb52fd8fcee62396ef448
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692269073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7ed3b78d40c11e1b47f6c3fb27275c3289271e69f2d4946166e26ef3028972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:15:23 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:15:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:17:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:17:38 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:17:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7125fbbf1426092fe6933ef492b330859c33df4c223e56391f89b42b16e045ee`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8398f134d3c378d17b050bfd4b64beb85a05e2e7596864eb802d049503172f3f`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e19cf7c338f75657e10dedb236bf941729dedb6c1909f49054ee5e8650eaf2e`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55501c2e78abcdc12785db0e7045f1fc816427a651439a2d96fdba261ccd956`  
		Last Modified: Mon, 22 Mar 2021 19:29:36 GMT  
		Size: 230.7 MB (230724749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c33cf9ff3dc2f3d9ac2b6d85f2dee0698cbdc41b74d1aca2001b752c823a297`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f2da1ce568bdb909af7b2eddec2c8405ed83a8e8ed87c3a99caf2a61c7e9d`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7c6bf198ad8a3fb8a3879796caac6cd559bc27cd0ec1667e9a1d69b173a1b`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:7be90b243eb7f847c5998ed11d866d4707490ec63789c744c032ea2b90ccebfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:003d7796e5615a09631a01bb00ee2f772461eee132da5480c2dde3002018c65d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6028346497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2001dc86ca184f18a58ce56c979d40f453090a77e027c4300aaa8e600da36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:17:52 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:17:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:17:54 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:21:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:21:08 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c5392547fce8ffc9f2ca8bd53dd13325b8a9811d908d79bcf21e264003526`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f191de5d0f746b5acabb63d0e0e4c4979a356786c93070054fc532e99390d6f0`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394051376831027d2cd58c3df5b3d5ce6c1645488f18b51247fa0620f60281f`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee498fd2a3866142f4d271b5136d20fdd3be3e29e733b7d48d78a9a645132f`  
		Last Modified: Mon, 22 Mar 2021 19:34:20 GMT  
		Size: 231.4 MB (231425773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbc0ee3c51f0dd7f1f0fc9dc5ce6070073867ada02455b5414ea5f1b2afe358`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edded4e2d6084db86ea9d144b0640c355350da1b275aaaa6e0e5dac18046c4e`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e843513a6cccd3ab12a8ba4fa1f5dcc8bf5e2e2d0fe68f9a831421890ae529`  
		Last Modified: Mon, 22 Mar 2021 19:29:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:dfdd5a8c4f91124d09299d3ee4c1ac26c7bf9697dc9cf75296d39c9a8ddb1fbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:8febed4c87baf95786587ad2447817330b0cae3c02c147783bb30ab6fe731894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6075da9d551ef7d97e29775dcb03ec32226215bfa717cb326ddff5ccffb56a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:00:30 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 26 Mar 2021 12:00:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_MAJOR=3.6
# Fri, 26 Mar 2021 12:00:35 GMT
ENV MONGO_VERSION=3.6.23
# Fri, 26 Mar 2021 12:00:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:03 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:06 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:07 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da17adcdc02155bd69d9074497e6e2ffc5b7609dcdaefb81bf8c514e63689027`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a7cfbb0a119f0188e96ef9b49c63202bbb3c8f944ceb0a1186cbdb31221dff`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0624b9494b00f365e76e7318938ee308ef477a8b9ad653bf954cf6c791526f`  
		Last Modified: Fri, 26 Mar 2021 12:06:22 GMT  
		Size: 119.4 MB (119408001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fe06b9f8d979969819b4fbd3d893ae9747ea813ccf8bf4136451424bd5bfe4`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7541bd7b951e5a0d33629df6e8fdc2ab801111ee7a4d12a0eb019fb0f97e98`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c206a1d258a0c69a65ba30c312699d1d40d427cfaee393868da6f684e6a68972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.0 MB (157955361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31951dc525ae227bfc43b0b137ea273f7e9d19b61d890d2160d05c7c14b99890`
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
# Mon, 22 Mar 2021 19:40:32 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:40:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:04 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:05 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:07 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:07 GMT
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
	-	`sha256:4323fbd86340c57754c90058655613ba9aff6e054d6205519d5c6f65ed8d1d5e`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b780180bdd00bedf065b80a3dedda8d180d28660f90ddbfeae0c863b4ce090b`  
		Last Modified: Mon, 22 Mar 2021 19:43:00 GMT  
		Size: 113.4 MB (113379732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810e7643ed985ded5e60ff7e79e1e422390da8875e330da74d7e879a57e7c912`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c766c03ca1ae0eee35c4baff837a94ed0b5985665ee3baba01b7107733e1f3`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:b79495efbae684fbda5d03f37b56c8d15368448c16ecc535c0267ced6a8b9f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:8febed4c87baf95786587ad2447817330b0cae3c02c147783bb30ab6fe731894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6075da9d551ef7d97e29775dcb03ec32226215bfa717cb326ddff5ccffb56a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:00:30 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 26 Mar 2021 12:00:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_MAJOR=3.6
# Fri, 26 Mar 2021 12:00:35 GMT
ENV MONGO_VERSION=3.6.23
# Fri, 26 Mar 2021 12:00:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:03 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:06 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:07 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da17adcdc02155bd69d9074497e6e2ffc5b7609dcdaefb81bf8c514e63689027`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a7cfbb0a119f0188e96ef9b49c63202bbb3c8f944ceb0a1186cbdb31221dff`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0624b9494b00f365e76e7318938ee308ef477a8b9ad653bf954cf6c791526f`  
		Last Modified: Fri, 26 Mar 2021 12:06:22 GMT  
		Size: 119.4 MB (119408001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fe06b9f8d979969819b4fbd3d893ae9747ea813ccf8bf4136451424bd5bfe4`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7541bd7b951e5a0d33629df6e8fdc2ab801111ee7a4d12a0eb019fb0f97e98`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c206a1d258a0c69a65ba30c312699d1d40d427cfaee393868da6f684e6a68972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.0 MB (157955361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31951dc525ae227bfc43b0b137ea273f7e9d19b61d890d2160d05c7c14b99890`
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
# Mon, 22 Mar 2021 19:40:32 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:40:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:04 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:05 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:07 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:07 GMT
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
	-	`sha256:4323fbd86340c57754c90058655613ba9aff6e054d6205519d5c6f65ed8d1d5e`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b780180bdd00bedf065b80a3dedda8d180d28660f90ddbfeae0c863b4ce090b`  
		Last Modified: Mon, 22 Mar 2021 19:43:00 GMT  
		Size: 113.4 MB (113379732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810e7643ed985ded5e60ff7e79e1e422390da8875e330da74d7e879a57e7c912`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c766c03ca1ae0eee35c4baff837a94ed0b5985665ee3baba01b7107733e1f3`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:63731590e62366f30a5d83b24987f6b71fa886f2c81eb52fd8fcee62396ef448
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692269073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7ed3b78d40c11e1b47f6c3fb27275c3289271e69f2d4946166e26ef3028972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:15:23 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:15:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:17:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:17:38 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:17:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7125fbbf1426092fe6933ef492b330859c33df4c223e56391f89b42b16e045ee`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8398f134d3c378d17b050bfd4b64beb85a05e2e7596864eb802d049503172f3f`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e19cf7c338f75657e10dedb236bf941729dedb6c1909f49054ee5e8650eaf2e`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55501c2e78abcdc12785db0e7045f1fc816427a651439a2d96fdba261ccd956`  
		Last Modified: Mon, 22 Mar 2021 19:29:36 GMT  
		Size: 230.7 MB (230724749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c33cf9ff3dc2f3d9ac2b6d85f2dee0698cbdc41b74d1aca2001b752c823a297`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f2da1ce568bdb909af7b2eddec2c8405ed83a8e8ed87c3a99caf2a61c7e9d`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7c6bf198ad8a3fb8a3879796caac6cd559bc27cd0ec1667e9a1d69b173a1b`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:003d7796e5615a09631a01bb00ee2f772461eee132da5480c2dde3002018c65d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6028346497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2001dc86ca184f18a58ce56c979d40f453090a77e027c4300aaa8e600da36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:17:52 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:17:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:17:54 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:21:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:21:08 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c5392547fce8ffc9f2ca8bd53dd13325b8a9811d908d79bcf21e264003526`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f191de5d0f746b5acabb63d0e0e4c4979a356786c93070054fc532e99390d6f0`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394051376831027d2cd58c3df5b3d5ce6c1645488f18b51247fa0620f60281f`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee498fd2a3866142f4d271b5136d20fdd3be3e29e733b7d48d78a9a645132f`  
		Last Modified: Mon, 22 Mar 2021 19:34:20 GMT  
		Size: 231.4 MB (231425773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbc0ee3c51f0dd7f1f0fc9dc5ce6070073867ada02455b5414ea5f1b2afe358`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edded4e2d6084db86ea9d144b0640c355350da1b275aaaa6e0e5dac18046c4e`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e843513a6cccd3ab12a8ba4fa1f5dcc8bf5e2e2d0fe68f9a831421890ae529`  
		Last Modified: Mon, 22 Mar 2021 19:29:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:7ddbaa2f3aff5d6d10af75479604f1f1fccf47cfea95a17e9d3947c74ee11f59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:63731590e62366f30a5d83b24987f6b71fa886f2c81eb52fd8fcee62396ef448
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692269073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7ed3b78d40c11e1b47f6c3fb27275c3289271e69f2d4946166e26ef3028972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:15:23 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:15:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:17:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:17:38 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:17:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7125fbbf1426092fe6933ef492b330859c33df4c223e56391f89b42b16e045ee`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8398f134d3c378d17b050bfd4b64beb85a05e2e7596864eb802d049503172f3f`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e19cf7c338f75657e10dedb236bf941729dedb6c1909f49054ee5e8650eaf2e`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55501c2e78abcdc12785db0e7045f1fc816427a651439a2d96fdba261ccd956`  
		Last Modified: Mon, 22 Mar 2021 19:29:36 GMT  
		Size: 230.7 MB (230724749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c33cf9ff3dc2f3d9ac2b6d85f2dee0698cbdc41b74d1aca2001b752c823a297`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f2da1ce568bdb909af7b2eddec2c8405ed83a8e8ed87c3a99caf2a61c7e9d`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7c6bf198ad8a3fb8a3879796caac6cd559bc27cd0ec1667e9a1d69b173a1b`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:003d7796e5615a09631a01bb00ee2f772461eee132da5480c2dde3002018c65d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6028346497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2001dc86ca184f18a58ce56c979d40f453090a77e027c4300aaa8e600da36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:17:52 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:17:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:17:54 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:21:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:21:08 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c5392547fce8ffc9f2ca8bd53dd13325b8a9811d908d79bcf21e264003526`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f191de5d0f746b5acabb63d0e0e4c4979a356786c93070054fc532e99390d6f0`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394051376831027d2cd58c3df5b3d5ce6c1645488f18b51247fa0620f60281f`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee498fd2a3866142f4d271b5136d20fdd3be3e29e733b7d48d78a9a645132f`  
		Last Modified: Mon, 22 Mar 2021 19:34:20 GMT  
		Size: 231.4 MB (231425773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbc0ee3c51f0dd7f1f0fc9dc5ce6070073867ada02455b5414ea5f1b2afe358`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edded4e2d6084db86ea9d144b0640c355350da1b275aaaa6e0e5dac18046c4e`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e843513a6cccd3ab12a8ba4fa1f5dcc8bf5e2e2d0fe68f9a831421890ae529`  
		Last Modified: Mon, 22 Mar 2021 19:29:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:1d0a12f8d1a4886a50245fa6f59f76b128869b8838f928adcd606bb1f393116a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:63731590e62366f30a5d83b24987f6b71fa886f2c81eb52fd8fcee62396ef448
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692269073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7ed3b78d40c11e1b47f6c3fb27275c3289271e69f2d4946166e26ef3028972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:15:23 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:15:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:17:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:17:38 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:17:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7125fbbf1426092fe6933ef492b330859c33df4c223e56391f89b42b16e045ee`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8398f134d3c378d17b050bfd4b64beb85a05e2e7596864eb802d049503172f3f`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e19cf7c338f75657e10dedb236bf941729dedb6c1909f49054ee5e8650eaf2e`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55501c2e78abcdc12785db0e7045f1fc816427a651439a2d96fdba261ccd956`  
		Last Modified: Mon, 22 Mar 2021 19:29:36 GMT  
		Size: 230.7 MB (230724749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c33cf9ff3dc2f3d9ac2b6d85f2dee0698cbdc41b74d1aca2001b752c823a297`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f2da1ce568bdb909af7b2eddec2c8405ed83a8e8ed87c3a99caf2a61c7e9d`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7c6bf198ad8a3fb8a3879796caac6cd559bc27cd0ec1667e9a1d69b173a1b`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:7be90b243eb7f847c5998ed11d866d4707490ec63789c744c032ea2b90ccebfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:003d7796e5615a09631a01bb00ee2f772461eee132da5480c2dde3002018c65d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6028346497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2001dc86ca184f18a58ce56c979d40f453090a77e027c4300aaa8e600da36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:17:52 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:17:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:17:54 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:21:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:21:08 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c5392547fce8ffc9f2ca8bd53dd13325b8a9811d908d79bcf21e264003526`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f191de5d0f746b5acabb63d0e0e4c4979a356786c93070054fc532e99390d6f0`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394051376831027d2cd58c3df5b3d5ce6c1645488f18b51247fa0620f60281f`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee498fd2a3866142f4d271b5136d20fdd3be3e29e733b7d48d78a9a645132f`  
		Last Modified: Mon, 22 Mar 2021 19:34:20 GMT  
		Size: 231.4 MB (231425773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbc0ee3c51f0dd7f1f0fc9dc5ce6070073867ada02455b5414ea5f1b2afe358`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edded4e2d6084db86ea9d144b0640c355350da1b275aaaa6e0e5dac18046c4e`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e843513a6cccd3ab12a8ba4fa1f5dcc8bf5e2e2d0fe68f9a831421890ae529`  
		Last Modified: Mon, 22 Mar 2021 19:29:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:dfdd5a8c4f91124d09299d3ee4c1ac26c7bf9697dc9cf75296d39c9a8ddb1fbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:8febed4c87baf95786587ad2447817330b0cae3c02c147783bb30ab6fe731894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6075da9d551ef7d97e29775dcb03ec32226215bfa717cb326ddff5ccffb56a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:00:30 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 26 Mar 2021 12:00:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_MAJOR=3.6
# Fri, 26 Mar 2021 12:00:35 GMT
ENV MONGO_VERSION=3.6.23
# Fri, 26 Mar 2021 12:00:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:03 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:06 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:07 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da17adcdc02155bd69d9074497e6e2ffc5b7609dcdaefb81bf8c514e63689027`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a7cfbb0a119f0188e96ef9b49c63202bbb3c8f944ceb0a1186cbdb31221dff`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0624b9494b00f365e76e7318938ee308ef477a8b9ad653bf954cf6c791526f`  
		Last Modified: Fri, 26 Mar 2021 12:06:22 GMT  
		Size: 119.4 MB (119408001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fe06b9f8d979969819b4fbd3d893ae9747ea813ccf8bf4136451424bd5bfe4`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7541bd7b951e5a0d33629df6e8fdc2ab801111ee7a4d12a0eb019fb0f97e98`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c206a1d258a0c69a65ba30c312699d1d40d427cfaee393868da6f684e6a68972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.0 MB (157955361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31951dc525ae227bfc43b0b137ea273f7e9d19b61d890d2160d05c7c14b99890`
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
# Mon, 22 Mar 2021 19:40:32 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:40:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:04 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:05 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:07 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:07 GMT
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
	-	`sha256:4323fbd86340c57754c90058655613ba9aff6e054d6205519d5c6f65ed8d1d5e`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b780180bdd00bedf065b80a3dedda8d180d28660f90ddbfeae0c863b4ce090b`  
		Last Modified: Mon, 22 Mar 2021 19:43:00 GMT  
		Size: 113.4 MB (113379732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810e7643ed985ded5e60ff7e79e1e422390da8875e330da74d7e879a57e7c912`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c766c03ca1ae0eee35c4baff837a94ed0b5985665ee3baba01b7107733e1f3`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23`

```console
$ docker pull mongo@sha256:b79495efbae684fbda5d03f37b56c8d15368448c16ecc535c0267ced6a8b9f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:3.6.23` - linux; amd64

```console
$ docker pull mongo@sha256:8febed4c87baf95786587ad2447817330b0cae3c02c147783bb30ab6fe731894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6075da9d551ef7d97e29775dcb03ec32226215bfa717cb326ddff5ccffb56a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:00:30 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 26 Mar 2021 12:00:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_MAJOR=3.6
# Fri, 26 Mar 2021 12:00:35 GMT
ENV MONGO_VERSION=3.6.23
# Fri, 26 Mar 2021 12:00:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:03 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:06 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:07 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da17adcdc02155bd69d9074497e6e2ffc5b7609dcdaefb81bf8c514e63689027`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a7cfbb0a119f0188e96ef9b49c63202bbb3c8f944ceb0a1186cbdb31221dff`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0624b9494b00f365e76e7318938ee308ef477a8b9ad653bf954cf6c791526f`  
		Last Modified: Fri, 26 Mar 2021 12:06:22 GMT  
		Size: 119.4 MB (119408001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fe06b9f8d979969819b4fbd3d893ae9747ea813ccf8bf4136451424bd5bfe4`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7541bd7b951e5a0d33629df6e8fdc2ab801111ee7a4d12a0eb019fb0f97e98`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c206a1d258a0c69a65ba30c312699d1d40d427cfaee393868da6f684e6a68972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.0 MB (157955361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31951dc525ae227bfc43b0b137ea273f7e9d19b61d890d2160d05c7c14b99890`
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
# Mon, 22 Mar 2021 19:40:32 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:40:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:04 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:05 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:07 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:07 GMT
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
	-	`sha256:4323fbd86340c57754c90058655613ba9aff6e054d6205519d5c6f65ed8d1d5e`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b780180bdd00bedf065b80a3dedda8d180d28660f90ddbfeae0c863b4ce090b`  
		Last Modified: Mon, 22 Mar 2021 19:43:00 GMT  
		Size: 113.4 MB (113379732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810e7643ed985ded5e60ff7e79e1e422390da8875e330da74d7e879a57e7c912`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c766c03ca1ae0eee35c4baff837a94ed0b5985665ee3baba01b7107733e1f3`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:63731590e62366f30a5d83b24987f6b71fa886f2c81eb52fd8fcee62396ef448
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692269073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7ed3b78d40c11e1b47f6c3fb27275c3289271e69f2d4946166e26ef3028972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:15:23 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:15:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:17:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:17:38 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:17:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7125fbbf1426092fe6933ef492b330859c33df4c223e56391f89b42b16e045ee`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8398f134d3c378d17b050bfd4b64beb85a05e2e7596864eb802d049503172f3f`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e19cf7c338f75657e10dedb236bf941729dedb6c1909f49054ee5e8650eaf2e`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55501c2e78abcdc12785db0e7045f1fc816427a651439a2d96fdba261ccd956`  
		Last Modified: Mon, 22 Mar 2021 19:29:36 GMT  
		Size: 230.7 MB (230724749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c33cf9ff3dc2f3d9ac2b6d85f2dee0698cbdc41b74d1aca2001b752c823a297`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f2da1ce568bdb909af7b2eddec2c8405ed83a8e8ed87c3a99caf2a61c7e9d`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7c6bf198ad8a3fb8a3879796caac6cd559bc27cd0ec1667e9a1d69b173a1b`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:003d7796e5615a09631a01bb00ee2f772461eee132da5480c2dde3002018c65d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6028346497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2001dc86ca184f18a58ce56c979d40f453090a77e027c4300aaa8e600da36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:17:52 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:17:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:17:54 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:21:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:21:08 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c5392547fce8ffc9f2ca8bd53dd13325b8a9811d908d79bcf21e264003526`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f191de5d0f746b5acabb63d0e0e4c4979a356786c93070054fc532e99390d6f0`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394051376831027d2cd58c3df5b3d5ce6c1645488f18b51247fa0620f60281f`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee498fd2a3866142f4d271b5136d20fdd3be3e29e733b7d48d78a9a645132f`  
		Last Modified: Mon, 22 Mar 2021 19:34:20 GMT  
		Size: 231.4 MB (231425773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbc0ee3c51f0dd7f1f0fc9dc5ce6070073867ada02455b5414ea5f1b2afe358`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edded4e2d6084db86ea9d144b0640c355350da1b275aaaa6e0e5dac18046c4e`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e843513a6cccd3ab12a8ba4fa1f5dcc8bf5e2e2d0fe68f9a831421890ae529`  
		Last Modified: Mon, 22 Mar 2021 19:29:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23-windowsservercore`

```console
$ docker pull mongo@sha256:7ddbaa2f3aff5d6d10af75479604f1f1fccf47cfea95a17e9d3947c74ee11f59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:3.6.23-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:63731590e62366f30a5d83b24987f6b71fa886f2c81eb52fd8fcee62396ef448
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692269073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7ed3b78d40c11e1b47f6c3fb27275c3289271e69f2d4946166e26ef3028972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:15:23 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:15:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:17:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:17:38 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:17:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7125fbbf1426092fe6933ef492b330859c33df4c223e56391f89b42b16e045ee`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8398f134d3c378d17b050bfd4b64beb85a05e2e7596864eb802d049503172f3f`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e19cf7c338f75657e10dedb236bf941729dedb6c1909f49054ee5e8650eaf2e`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55501c2e78abcdc12785db0e7045f1fc816427a651439a2d96fdba261ccd956`  
		Last Modified: Mon, 22 Mar 2021 19:29:36 GMT  
		Size: 230.7 MB (230724749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c33cf9ff3dc2f3d9ac2b6d85f2dee0698cbdc41b74d1aca2001b752c823a297`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f2da1ce568bdb909af7b2eddec2c8405ed83a8e8ed87c3a99caf2a61c7e9d`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7c6bf198ad8a3fb8a3879796caac6cd559bc27cd0ec1667e9a1d69b173a1b`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:003d7796e5615a09631a01bb00ee2f772461eee132da5480c2dde3002018c65d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6028346497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2001dc86ca184f18a58ce56c979d40f453090a77e027c4300aaa8e600da36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:17:52 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:17:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:17:54 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:21:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:21:08 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c5392547fce8ffc9f2ca8bd53dd13325b8a9811d908d79bcf21e264003526`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f191de5d0f746b5acabb63d0e0e4c4979a356786c93070054fc532e99390d6f0`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394051376831027d2cd58c3df5b3d5ce6c1645488f18b51247fa0620f60281f`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee498fd2a3866142f4d271b5136d20fdd3be3e29e733b7d48d78a9a645132f`  
		Last Modified: Mon, 22 Mar 2021 19:34:20 GMT  
		Size: 231.4 MB (231425773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbc0ee3c51f0dd7f1f0fc9dc5ce6070073867ada02455b5414ea5f1b2afe358`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edded4e2d6084db86ea9d144b0640c355350da1b275aaaa6e0e5dac18046c4e`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e843513a6cccd3ab12a8ba4fa1f5dcc8bf5e2e2d0fe68f9a831421890ae529`  
		Last Modified: Mon, 22 Mar 2021 19:29:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23-windowsservercore-1809`

```console
$ docker pull mongo@sha256:1d0a12f8d1a4886a50245fa6f59f76b128869b8838f928adcd606bb1f393116a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:3.6.23-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:63731590e62366f30a5d83b24987f6b71fa886f2c81eb52fd8fcee62396ef448
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692269073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e7ed3b78d40c11e1b47f6c3fb27275c3289271e69f2d4946166e26ef3028972`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:15:23 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:15:24 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:15:25 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:17:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:17:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:17:38 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:17:39 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7125fbbf1426092fe6933ef492b330859c33df4c223e56391f89b42b16e045ee`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8398f134d3c378d17b050bfd4b64beb85a05e2e7596864eb802d049503172f3f`  
		Last Modified: Mon, 22 Mar 2021 19:28:52 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e19cf7c338f75657e10dedb236bf941729dedb6c1909f49054ee5e8650eaf2e`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55501c2e78abcdc12785db0e7045f1fc816427a651439a2d96fdba261ccd956`  
		Last Modified: Mon, 22 Mar 2021 19:29:36 GMT  
		Size: 230.7 MB (230724749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c33cf9ff3dc2f3d9ac2b6d85f2dee0698cbdc41b74d1aca2001b752c823a297`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f2da1ce568bdb909af7b2eddec2c8405ed83a8e8ed87c3a99caf2a61c7e9d`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e7c6bf198ad8a3fb8a3879796caac6cd559bc27cd0ec1667e9a1d69b173a1b`  
		Last Modified: Mon, 22 Mar 2021 19:28:49 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:7be90b243eb7f847c5998ed11d866d4707490ec63789c744c032ea2b90ccebfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:3.6.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:003d7796e5615a09631a01bb00ee2f772461eee132da5480c2dde3002018c65d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6028346497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a2001dc86ca184f18a58ce56c979d40f453090a77e027c4300aaa8e600da36`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:17:52 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:17:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.23-signed.msi
# Mon, 22 Mar 2021 19:17:54 GMT
ENV MONGO_DOWNLOAD_SHA256=ebc275ea0b2f69f2297e329877cb8174c69d2a5da3c41306b5b7a06aa45796e8
# Mon, 22 Mar 2021 19:21:06 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:21:08 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c5392547fce8ffc9f2ca8bd53dd13325b8a9811d908d79bcf21e264003526`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f191de5d0f746b5acabb63d0e0e4c4979a356786c93070054fc532e99390d6f0`  
		Last Modified: Mon, 22 Mar 2021 19:29:54 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1394051376831027d2cd58c3df5b3d5ce6c1645488f18b51247fa0620f60281f`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ee498fd2a3866142f4d271b5136d20fdd3be3e29e733b7d48d78a9a645132f`  
		Last Modified: Mon, 22 Mar 2021 19:34:20 GMT  
		Size: 231.4 MB (231425773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbc0ee3c51f0dd7f1f0fc9dc5ce6070073867ada02455b5414ea5f1b2afe358`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edded4e2d6084db86ea9d144b0640c355350da1b275aaaa6e0e5dac18046c4e`  
		Last Modified: Mon, 22 Mar 2021 19:29:51 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e843513a6cccd3ab12a8ba4fa1f5dcc8bf5e2e2d0fe68f9a831421890ae529`  
		Last Modified: Mon, 22 Mar 2021 19:29:52 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.23-xenial`

```console
$ docker pull mongo@sha256:dfdd5a8c4f91124d09299d3ee4c1ac26c7bf9697dc9cf75296d39c9a8ddb1fbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.23-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:8febed4c87baf95786587ad2447817330b0cae3c02c147783bb30ab6fe731894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6075da9d551ef7d97e29775dcb03ec32226215bfa717cb326ddff5ccffb56a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:00:30 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Fri, 26 Mar 2021 12:00:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:00:33 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:00:34 GMT
ENV MONGO_MAJOR=3.6
# Fri, 26 Mar 2021 12:00:35 GMT
ENV MONGO_VERSION=3.6.23
# Fri, 26 Mar 2021 12:00:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:03 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:06 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:06 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:06 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:07 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da17adcdc02155bd69d9074497e6e2ffc5b7609dcdaefb81bf8c514e63689027`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 2.0 KB (1999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a7cfbb0a119f0188e96ef9b49c63202bbb3c8f944ceb0a1186cbdb31221dff`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0624b9494b00f365e76e7318938ee308ef477a8b9ad653bf954cf6c791526f`  
		Last Modified: Fri, 26 Mar 2021 12:06:22 GMT  
		Size: 119.4 MB (119408001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fe06b9f8d979969819b4fbd3d893ae9747ea813ccf8bf4136451424bd5bfe4`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7541bd7b951e5a0d33629df6e8fdc2ab801111ee7a4d12a0eb019fb0f97e98`  
		Last Modified: Fri, 26 Mar 2021 12:05:58 GMT  
		Size: 4.4 KB (4420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.23-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c206a1d258a0c69a65ba30c312699d1d40d427cfaee393868da6f684e6a68972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.0 MB (157955361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31951dc525ae227bfc43b0b137ea273f7e9d19b61d890d2160d05c7c14b99890`
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
# Mon, 22 Mar 2021 19:40:32 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:40:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:00 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:03 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:04 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:05 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:07 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:07 GMT
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
	-	`sha256:4323fbd86340c57754c90058655613ba9aff6e054d6205519d5c6f65ed8d1d5e`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b780180bdd00bedf065b80a3dedda8d180d28660f90ddbfeae0c863b4ce090b`  
		Last Modified: Mon, 22 Mar 2021 19:43:00 GMT  
		Size: 113.4 MB (113379732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810e7643ed985ded5e60ff7e79e1e422390da8875e330da74d7e879a57e7c912`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c766c03ca1ae0eee35c4baff837a94ed0b5985665ee3baba01b7107733e1f3`  
		Last Modified: Mon, 22 Mar 2021 19:42:33 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:75a5f624bd6d14254e0d84c2833f576109672750aaf2bf01d61cb5ead44f4505
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:424cadd696e9a0dbc691a4e2680722f2a9e8ab604374b482e2a9890fdc8ab0c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175093468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03be0dc25f8732caef29f051c91ce7447f8305738032e91c23b13cba3e74e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:03:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 12:03:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:03:30 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:03:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 12:03:32 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:05:11 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:05:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:05:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:05:13 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:05:13 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:05:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8c3715616e84c33c0038ba795484161fd38d0930d82e09b68283a1a18f451`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac42b84e850eda3c7655d1937d8a023de9fa68199e383acb2262d323442219d`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724cb122c25fe9272d20cdf76c45c6aab3f447f4e6f3b0ebfdfbb46724eb2ef`  
		Last Modified: Fri, 26 Mar 2021 12:08:02 GMT  
		Size: 139.6 MB (139567497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe10b8b0c12777d4c337f611abaf127960fab70650c1f7ad27073ac9bd2521`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e025c87f29ce34b87590b9f4dcc0b3b164ddba3bb903fcb1b9e0b91b0c7a7b`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:18b9ba93b6208cd80e1a723a241269f6e1eb44bfaa6ce1dd3de9be32f717daf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167536780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58929ecfa3caf151a12d97acb343f9b94bd867df524c3cdc9f60a00f46df5496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:27:42 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 14:27:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:27:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:27:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:50 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 14:27:51 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 14:27:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:28:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:28:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:28:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:28:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:28:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:28:46 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:28:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada24af95b05b298538ab63d883be491085362960192889c5c5d07627dfc446`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877762b7148d23f4cef028d66cb3f7ab51c8fb232f674d8cb2ce546675f0803`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a783117ad78ea48199bae4e86a245b13ae202fd98202cc2d5cd9df8bb0564432`  
		Last Modified: Fri, 26 Mar 2021 14:30:33 GMT  
		Size: 135.8 MB (135778542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc369a412303d9bc7d67b498032752b974cc1cf3a1854beba31c5b7705ca819`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ff00ed0d4b2c1c9040bac960068c8cf865ddf3b3417b0b4bfa0372df05ba06`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:cbb067bdf193c627f85874531f3d5c0b692d81db482a9c0c69d026a81383afe5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169136167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651556f82f603bac974f5788631fd43b058c3c818c1c6a96cf2e2dc5c2a0a289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:31 GMT
ADD file:1c7dbc64158234b813a2eeff0c325efa0cff7c3983e93fc9f7de0004e901c2c1 in / 
# Thu, 25 Mar 2021 22:53:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:35 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 08:57:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 08:57:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:57:20 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 08:57:21 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 08:57:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 08:57:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 08:57:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 08:57:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 08:57:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 08:57:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 08:57:41 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 08:57:42 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 08:58:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 08:58:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 08:58:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 08:58:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 08:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:58:33 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 08:58:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:bf8da0ed3f9ec60019cec9fac782f04b7281f232a86e7613579e54c348b8402b`  
		Last Modified: Thu, 25 Mar 2021 22:54:27 GMT  
		Size: 25.4 MB (25381419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de72c87d1d7a4355d21e04b9ce611f427f0c84ee6705dd53a1fd990012cefdd6`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffe2f5d8eac8afe4b79981c9c93b44c985dbb7b3bb5f9af5e918c6aac415fcf`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2808460e51d63b807cb6cb00bf034b7f2643599362ad55d9df26c6bc9ffad42c`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400c3133d141345611000d1de01cfadc8b8a785e209b80afcafa9214669ffd8f`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 2.7 MB (2708345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cdf5b66f6831b7db4ee570b487453c025248b2607e441c34db29488fcc35d4`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 5.7 MB (5747339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0de8bd807c307aaa480d335670e64efb51855df37c491f9e888d1848637001`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d58b3f14f22d07c415679c463eb1f4af10f1cbf89aa20fb46aaf3e31a41c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eef524d85fb192432f8eb7fc575cef6576292d4d47939a2b3650fd72dba5c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34edb6160fb71ce9809aec003c97570df6d05e2b19a1eb3ec267806ba9586f1`  
		Last Modified: Fri, 26 Mar 2021 08:59:21 GMT  
		Size: 135.3 MB (135289747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa65663451ec46890ca56252fcc498672e68e9b5dfa0df327c68150aa50226`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8215528e5cd8c0cb268785c0f8d75cfeb8ac2b40dd7f267effa9793d6fb487c5`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:1fdc0fd04f4c1006a41c81066521c8d396a4fe9cbbb7d8df99dfba9ba670bfe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:424cadd696e9a0dbc691a4e2680722f2a9e8ab604374b482e2a9890fdc8ab0c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175093468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03be0dc25f8732caef29f051c91ce7447f8305738032e91c23b13cba3e74e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:03:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 12:03:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:03:30 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:03:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 12:03:32 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:05:11 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:05:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:05:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:05:13 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:05:13 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:05:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8c3715616e84c33c0038ba795484161fd38d0930d82e09b68283a1a18f451`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac42b84e850eda3c7655d1937d8a023de9fa68199e383acb2262d323442219d`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724cb122c25fe9272d20cdf76c45c6aab3f447f4e6f3b0ebfdfbb46724eb2ef`  
		Last Modified: Fri, 26 Mar 2021 12:08:02 GMT  
		Size: 139.6 MB (139567497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe10b8b0c12777d4c337f611abaf127960fab70650c1f7ad27073ac9bd2521`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e025c87f29ce34b87590b9f4dcc0b3b164ddba3bb903fcb1b9e0b91b0c7a7b`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:18b9ba93b6208cd80e1a723a241269f6e1eb44bfaa6ce1dd3de9be32f717daf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167536780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58929ecfa3caf151a12d97acb343f9b94bd867df524c3cdc9f60a00f46df5496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:27:42 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 14:27:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:27:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:27:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:50 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 14:27:51 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 14:27:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:28:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:28:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:28:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:28:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:28:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:28:46 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:28:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada24af95b05b298538ab63d883be491085362960192889c5c5d07627dfc446`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877762b7148d23f4cef028d66cb3f7ab51c8fb232f674d8cb2ce546675f0803`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a783117ad78ea48199bae4e86a245b13ae202fd98202cc2d5cd9df8bb0564432`  
		Last Modified: Fri, 26 Mar 2021 14:30:33 GMT  
		Size: 135.8 MB (135778542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc369a412303d9bc7d67b498032752b974cc1cf3a1854beba31c5b7705ca819`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ff00ed0d4b2c1c9040bac960068c8cf865ddf3b3417b0b4bfa0372df05ba06`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:cbb067bdf193c627f85874531f3d5c0b692d81db482a9c0c69d026a81383afe5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169136167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651556f82f603bac974f5788631fd43b058c3c818c1c6a96cf2e2dc5c2a0a289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:31 GMT
ADD file:1c7dbc64158234b813a2eeff0c325efa0cff7c3983e93fc9f7de0004e901c2c1 in / 
# Thu, 25 Mar 2021 22:53:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:35 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 08:57:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 08:57:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:57:20 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 08:57:21 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 08:57:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 08:57:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 08:57:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 08:57:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 08:57:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 08:57:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 08:57:41 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 08:57:42 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 08:58:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 08:58:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 08:58:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 08:58:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 08:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:58:33 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 08:58:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:bf8da0ed3f9ec60019cec9fac782f04b7281f232a86e7613579e54c348b8402b`  
		Last Modified: Thu, 25 Mar 2021 22:54:27 GMT  
		Size: 25.4 MB (25381419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de72c87d1d7a4355d21e04b9ce611f427f0c84ee6705dd53a1fd990012cefdd6`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffe2f5d8eac8afe4b79981c9c93b44c985dbb7b3bb5f9af5e918c6aac415fcf`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2808460e51d63b807cb6cb00bf034b7f2643599362ad55d9df26c6bc9ffad42c`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400c3133d141345611000d1de01cfadc8b8a785e209b80afcafa9214669ffd8f`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 2.7 MB (2708345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cdf5b66f6831b7db4ee570b487453c025248b2607e441c34db29488fcc35d4`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 5.7 MB (5747339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0de8bd807c307aaa480d335670e64efb51855df37c491f9e888d1848637001`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d58b3f14f22d07c415679c463eb1f4af10f1cbf89aa20fb46aaf3e31a41c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eef524d85fb192432f8eb7fc575cef6576292d4d47939a2b3650fd72dba5c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34edb6160fb71ce9809aec003c97570df6d05e2b19a1eb3ec267806ba9586f1`  
		Last Modified: Fri, 26 Mar 2021 08:59:21 GMT  
		Size: 135.3 MB (135289747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa65663451ec46890ca56252fcc498672e68e9b5dfa0df327c68150aa50226`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8215528e5cd8c0cb268785c0f8d75cfeb8ac2b40dd7f267effa9793d6fb487c5`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:015fbab5dc985d5281b38ea374ec95fe55adddab9f883b59e8b37c7c61090cba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:60acbac1cd7c075dc499da7ed7b6a9176c62fbab80a72afad59554330adc6d56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:13cc45bcbe04fd9d2f1acea62d4bc57a1a533cae59c01cfcc74bff9aa5f2a501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:007c81ff7b81d99f611b1ec664ab036838219c22b8105b556c69d847c9682280
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:06c6b5dd62a46dbac54127b06c3fdf906e22afa54510049517990fda8a54da11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156130343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0df4f86665738885bc4e9dc7b0576d90f45f34f11e9a047729c6854b6bf9a65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:01:20 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 26 Mar 2021 12:01:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:01:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:01:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:01:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:01:25 GMT
ENV MONGO_MAJOR=4.0
# Fri, 26 Mar 2021 12:01:25 GMT
ENV MONGO_VERSION=4.0.23
# Fri, 26 Mar 2021 12:01:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:49 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:51 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:52 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:52 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6581891ba73f040b5728189e295d1f1e0f36fd802abbf95c431eae3cdd3f9d47`  
		Last Modified: Fri, 26 Mar 2021 12:06:39 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17a3cabb9decc8b2aeab50a695d73d3b154e6436bc21562d2e9a5a8202669a3`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dd736a5440e879ceef968361c521d055c97a6f7b5c0a83d0e1c96448f7ef18`  
		Last Modified: Fri, 26 Mar 2021 12:06:55 GMT  
		Size: 105.9 MB (105945768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63c9587c119b63b3822d648974ed9b7a1f504d3f2e623034512ba36276d967c`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4806e4fe4ce30e1bc3b7d8c20344e14193e2d4ed70afb4047b64fc7f597b66`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 4.4 KB (4420 bytes)  
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

### `mongo:4.0` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:4fc08ddf022a5375d9fa4c0d94e8c6dc266f3c1b66955084d50d5210589384b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2696767747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f3d07aecbebe24e790d19524ad862b5f574e37e87f3082a59d42287c0863cc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:01:46 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:01:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:01:48 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:03:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:03:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:03:56 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:03:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035fbd38d8b52e01f940adb123050f0ee57ee459f568382f9ab2e161385daccc`  
		Last Modified: Wed, 10 Mar 2021 22:27:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e5caabff84d783ac1febddbbda13747e40e778a71899a540e1b82182dbc1f3`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce1afb0f0a252eb64ecf1b7bf79d8c945119ca0239b3c9d244ce747d6fbc5ee`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b6e1e12ef3e96a6db7a95b4a95acd12749e270ae732c0681cba28455133f47`  
		Last Modified: Wed, 10 Mar 2021 22:27:53 GMT  
		Size: 235.2 MB (235223440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0869747a8b49ccaa9ef00163f7d429c5b735f4b2cbf088a52b9bf9e5a0743e9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10f415b0d19985d54ed7945eca9c40343ad6dd851283e0f5c3dc4c391312e5`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7be938f74e1edf85b19d70b484a4d0c4a59d1843029996506b5db5552d4dd9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:83603f1754d1a692d10d88852407fcf458abaa727c6c5e6ea514fe94168ca216
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032830526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558fd300012714ba24dec1cb5b5bf8c12751e0ddf87616dbbad9d8bb3c4ecdaf`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:04:14 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:04:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:04:16 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:07:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:07:27 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:07:28 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:07:29 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c58ccf67935e99262254c3dfe2e9c28aca0b9661d66a60414faf28c21fd5931`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb22f888d0e51d3f0e92fcdc193db77dbf964cd5926330d40a6f6f51e101275d`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e71ce8b447156b65819454e2f150314b6ee92f7f76baf7bc1bb8aa389a0377d`  
		Last Modified: Wed, 10 Mar 2021 22:28:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45086bc178a2e2742f5a32caaef800e419a9b23a4c533fc9b79c3dac4e0f5986`  
		Last Modified: Wed, 10 Mar 2021 22:29:03 GMT  
		Size: 235.9 MB (235909789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315fb7f007e58410757d47f0971833f8d7162461a6d9ef05375f90110effd906`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52f0132f741b96fd2709a67f89be37cb6e0dd27685bc21d8fce68bc06412608`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e09528fa31b4c10649796974937ca7b3ce93a56e2d9aa80d683f25c517b8be`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:c9b80691272fbd8d1e97b966223f437fc3abdb528164d9c832804e6fe4050151
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:4fc08ddf022a5375d9fa4c0d94e8c6dc266f3c1b66955084d50d5210589384b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2696767747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f3d07aecbebe24e790d19524ad862b5f574e37e87f3082a59d42287c0863cc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:01:46 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:01:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:01:48 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:03:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:03:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:03:56 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:03:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035fbd38d8b52e01f940adb123050f0ee57ee459f568382f9ab2e161385daccc`  
		Last Modified: Wed, 10 Mar 2021 22:27:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e5caabff84d783ac1febddbbda13747e40e778a71899a540e1b82182dbc1f3`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce1afb0f0a252eb64ecf1b7bf79d8c945119ca0239b3c9d244ce747d6fbc5ee`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b6e1e12ef3e96a6db7a95b4a95acd12749e270ae732c0681cba28455133f47`  
		Last Modified: Wed, 10 Mar 2021 22:27:53 GMT  
		Size: 235.2 MB (235223440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0869747a8b49ccaa9ef00163f7d429c5b735f4b2cbf088a52b9bf9e5a0743e9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10f415b0d19985d54ed7945eca9c40343ad6dd851283e0f5c3dc4c391312e5`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7be938f74e1edf85b19d70b484a4d0c4a59d1843029996506b5db5552d4dd9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:83603f1754d1a692d10d88852407fcf458abaa727c6c5e6ea514fe94168ca216
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032830526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558fd300012714ba24dec1cb5b5bf8c12751e0ddf87616dbbad9d8bb3c4ecdaf`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:04:14 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:04:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:04:16 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:07:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:07:27 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:07:28 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:07:29 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c58ccf67935e99262254c3dfe2e9c28aca0b9661d66a60414faf28c21fd5931`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb22f888d0e51d3f0e92fcdc193db77dbf964cd5926330d40a6f6f51e101275d`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e71ce8b447156b65819454e2f150314b6ee92f7f76baf7bc1bb8aa389a0377d`  
		Last Modified: Wed, 10 Mar 2021 22:28:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45086bc178a2e2742f5a32caaef800e419a9b23a4c533fc9b79c3dac4e0f5986`  
		Last Modified: Wed, 10 Mar 2021 22:29:03 GMT  
		Size: 235.9 MB (235909789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315fb7f007e58410757d47f0971833f8d7162461a6d9ef05375f90110effd906`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52f0132f741b96fd2709a67f89be37cb6e0dd27685bc21d8fce68bc06412608`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e09528fa31b4c10649796974937ca7b3ce93a56e2d9aa80d683f25c517b8be`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:f10882173c6cdec36f50c60df70f568a94a9c3fded992e548d40d4022bad3658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:4fc08ddf022a5375d9fa4c0d94e8c6dc266f3c1b66955084d50d5210589384b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2696767747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f3d07aecbebe24e790d19524ad862b5f574e37e87f3082a59d42287c0863cc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:01:46 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:01:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:01:48 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:03:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:03:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:03:56 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:03:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035fbd38d8b52e01f940adb123050f0ee57ee459f568382f9ab2e161385daccc`  
		Last Modified: Wed, 10 Mar 2021 22:27:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e5caabff84d783ac1febddbbda13747e40e778a71899a540e1b82182dbc1f3`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce1afb0f0a252eb64ecf1b7bf79d8c945119ca0239b3c9d244ce747d6fbc5ee`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b6e1e12ef3e96a6db7a95b4a95acd12749e270ae732c0681cba28455133f47`  
		Last Modified: Wed, 10 Mar 2021 22:27:53 GMT  
		Size: 235.2 MB (235223440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0869747a8b49ccaa9ef00163f7d429c5b735f4b2cbf088a52b9bf9e5a0743e9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10f415b0d19985d54ed7945eca9c40343ad6dd851283e0f5c3dc4c391312e5`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7be938f74e1edf85b19d70b484a4d0c4a59d1843029996506b5db5552d4dd9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:ddb238e53f52fa3949339beb36fb5c2386918445e26542702b0bde1ea0dd1909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:83603f1754d1a692d10d88852407fcf458abaa727c6c5e6ea514fe94168ca216
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032830526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558fd300012714ba24dec1cb5b5bf8c12751e0ddf87616dbbad9d8bb3c4ecdaf`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:04:14 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:04:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:04:16 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:07:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:07:27 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:07:28 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:07:29 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c58ccf67935e99262254c3dfe2e9c28aca0b9661d66a60414faf28c21fd5931`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb22f888d0e51d3f0e92fcdc193db77dbf964cd5926330d40a6f6f51e101275d`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e71ce8b447156b65819454e2f150314b6ee92f7f76baf7bc1bb8aa389a0377d`  
		Last Modified: Wed, 10 Mar 2021 22:28:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45086bc178a2e2742f5a32caaef800e419a9b23a4c533fc9b79c3dac4e0f5986`  
		Last Modified: Wed, 10 Mar 2021 22:29:03 GMT  
		Size: 235.9 MB (235909789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315fb7f007e58410757d47f0971833f8d7162461a6d9ef05375f90110effd906`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52f0132f741b96fd2709a67f89be37cb6e0dd27685bc21d8fce68bc06412608`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e09528fa31b4c10649796974937ca7b3ce93a56e2d9aa80d683f25c517b8be`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:760b9af6eab2cadc037868a13ed6ec6dec79c801cc00fd7b1680f847edd052f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:06c6b5dd62a46dbac54127b06c3fdf906e22afa54510049517990fda8a54da11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156130343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0df4f86665738885bc4e9dc7b0576d90f45f34f11e9a047729c6854b6bf9a65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:01:20 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 26 Mar 2021 12:01:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:01:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:01:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:01:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:01:25 GMT
ENV MONGO_MAJOR=4.0
# Fri, 26 Mar 2021 12:01:25 GMT
ENV MONGO_VERSION=4.0.23
# Fri, 26 Mar 2021 12:01:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:49 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:51 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:52 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:52 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6581891ba73f040b5728189e295d1f1e0f36fd802abbf95c431eae3cdd3f9d47`  
		Last Modified: Fri, 26 Mar 2021 12:06:39 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17a3cabb9decc8b2aeab50a695d73d3b154e6436bc21562d2e9a5a8202669a3`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dd736a5440e879ceef968361c521d055c97a6f7b5c0a83d0e1c96448f7ef18`  
		Last Modified: Fri, 26 Mar 2021 12:06:55 GMT  
		Size: 105.9 MB (105945768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63c9587c119b63b3822d648974ed9b7a1f504d3f2e623034512ba36276d967c`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4806e4fe4ce30e1bc3b7d8c20344e14193e2d4ed70afb4047b64fc7f597b66`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 4.4 KB (4420 bytes)  
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

## `mongo:4.0.23`

```console
$ docker pull mongo@sha256:007c81ff7b81d99f611b1ec664ab036838219c22b8105b556c69d847c9682280
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.0.23` - linux; amd64

```console
$ docker pull mongo@sha256:06c6b5dd62a46dbac54127b06c3fdf906e22afa54510049517990fda8a54da11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156130343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0df4f86665738885bc4e9dc7b0576d90f45f34f11e9a047729c6854b6bf9a65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:01:20 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 26 Mar 2021 12:01:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:01:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:01:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:01:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:01:25 GMT
ENV MONGO_MAJOR=4.0
# Fri, 26 Mar 2021 12:01:25 GMT
ENV MONGO_VERSION=4.0.23
# Fri, 26 Mar 2021 12:01:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:49 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:51 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:52 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:52 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6581891ba73f040b5728189e295d1f1e0f36fd802abbf95c431eae3cdd3f9d47`  
		Last Modified: Fri, 26 Mar 2021 12:06:39 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17a3cabb9decc8b2aeab50a695d73d3b154e6436bc21562d2e9a5a8202669a3`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dd736a5440e879ceef968361c521d055c97a6f7b5c0a83d0e1c96448f7ef18`  
		Last Modified: Fri, 26 Mar 2021 12:06:55 GMT  
		Size: 105.9 MB (105945768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63c9587c119b63b3822d648974ed9b7a1f504d3f2e623034512ba36276d967c`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4806e4fe4ce30e1bc3b7d8c20344e14193e2d4ed70afb4047b64fc7f597b66`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 4.4 KB (4420 bytes)  
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

### `mongo:4.0.23` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:4fc08ddf022a5375d9fa4c0d94e8c6dc266f3c1b66955084d50d5210589384b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2696767747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f3d07aecbebe24e790d19524ad862b5f574e37e87f3082a59d42287c0863cc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:01:46 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:01:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:01:48 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:03:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:03:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:03:56 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:03:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035fbd38d8b52e01f940adb123050f0ee57ee459f568382f9ab2e161385daccc`  
		Last Modified: Wed, 10 Mar 2021 22:27:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e5caabff84d783ac1febddbbda13747e40e778a71899a540e1b82182dbc1f3`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce1afb0f0a252eb64ecf1b7bf79d8c945119ca0239b3c9d244ce747d6fbc5ee`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b6e1e12ef3e96a6db7a95b4a95acd12749e270ae732c0681cba28455133f47`  
		Last Modified: Wed, 10 Mar 2021 22:27:53 GMT  
		Size: 235.2 MB (235223440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0869747a8b49ccaa9ef00163f7d429c5b735f4b2cbf088a52b9bf9e5a0743e9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10f415b0d19985d54ed7945eca9c40343ad6dd851283e0f5c3dc4c391312e5`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7be938f74e1edf85b19d70b484a4d0c4a59d1843029996506b5db5552d4dd9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.23` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:83603f1754d1a692d10d88852407fcf458abaa727c6c5e6ea514fe94168ca216
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032830526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558fd300012714ba24dec1cb5b5bf8c12751e0ddf87616dbbad9d8bb3c4ecdaf`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:04:14 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:04:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:04:16 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:07:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:07:27 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:07:28 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:07:29 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c58ccf67935e99262254c3dfe2e9c28aca0b9661d66a60414faf28c21fd5931`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb22f888d0e51d3f0e92fcdc193db77dbf964cd5926330d40a6f6f51e101275d`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e71ce8b447156b65819454e2f150314b6ee92f7f76baf7bc1bb8aa389a0377d`  
		Last Modified: Wed, 10 Mar 2021 22:28:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45086bc178a2e2742f5a32caaef800e419a9b23a4c533fc9b79c3dac4e0f5986`  
		Last Modified: Wed, 10 Mar 2021 22:29:03 GMT  
		Size: 235.9 MB (235909789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315fb7f007e58410757d47f0971833f8d7162461a6d9ef05375f90110effd906`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52f0132f741b96fd2709a67f89be37cb6e0dd27685bc21d8fce68bc06412608`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e09528fa31b4c10649796974937ca7b3ce93a56e2d9aa80d683f25c517b8be`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.23-windowsservercore`

```console
$ docker pull mongo@sha256:c9b80691272fbd8d1e97b966223f437fc3abdb528164d9c832804e6fe4050151
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.0.23-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:4fc08ddf022a5375d9fa4c0d94e8c6dc266f3c1b66955084d50d5210589384b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2696767747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f3d07aecbebe24e790d19524ad862b5f574e37e87f3082a59d42287c0863cc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:01:46 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:01:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:01:48 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:03:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:03:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:03:56 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:03:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035fbd38d8b52e01f940adb123050f0ee57ee459f568382f9ab2e161385daccc`  
		Last Modified: Wed, 10 Mar 2021 22:27:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e5caabff84d783ac1febddbbda13747e40e778a71899a540e1b82182dbc1f3`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce1afb0f0a252eb64ecf1b7bf79d8c945119ca0239b3c9d244ce747d6fbc5ee`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b6e1e12ef3e96a6db7a95b4a95acd12749e270ae732c0681cba28455133f47`  
		Last Modified: Wed, 10 Mar 2021 22:27:53 GMT  
		Size: 235.2 MB (235223440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0869747a8b49ccaa9ef00163f7d429c5b735f4b2cbf088a52b9bf9e5a0743e9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10f415b0d19985d54ed7945eca9c40343ad6dd851283e0f5c3dc4c391312e5`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7be938f74e1edf85b19d70b484a4d0c4a59d1843029996506b5db5552d4dd9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.23-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:83603f1754d1a692d10d88852407fcf458abaa727c6c5e6ea514fe94168ca216
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032830526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558fd300012714ba24dec1cb5b5bf8c12751e0ddf87616dbbad9d8bb3c4ecdaf`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:04:14 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:04:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:04:16 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:07:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:07:27 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:07:28 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:07:29 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c58ccf67935e99262254c3dfe2e9c28aca0b9661d66a60414faf28c21fd5931`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb22f888d0e51d3f0e92fcdc193db77dbf964cd5926330d40a6f6f51e101275d`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e71ce8b447156b65819454e2f150314b6ee92f7f76baf7bc1bb8aa389a0377d`  
		Last Modified: Wed, 10 Mar 2021 22:28:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45086bc178a2e2742f5a32caaef800e419a9b23a4c533fc9b79c3dac4e0f5986`  
		Last Modified: Wed, 10 Mar 2021 22:29:03 GMT  
		Size: 235.9 MB (235909789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315fb7f007e58410757d47f0971833f8d7162461a6d9ef05375f90110effd906`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52f0132f741b96fd2709a67f89be37cb6e0dd27685bc21d8fce68bc06412608`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e09528fa31b4c10649796974937ca7b3ce93a56e2d9aa80d683f25c517b8be`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.23-windowsservercore-1809`

```console
$ docker pull mongo@sha256:f10882173c6cdec36f50c60df70f568a94a9c3fded992e548d40d4022bad3658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:4.0.23-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:4fc08ddf022a5375d9fa4c0d94e8c6dc266f3c1b66955084d50d5210589384b4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2696767747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f3d07aecbebe24e790d19524ad862b5f574e37e87f3082a59d42287c0863cc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:01:46 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:01:47 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:01:48 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:03:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:03:55 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:03:56 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:03:57 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035fbd38d8b52e01f940adb123050f0ee57ee459f568382f9ab2e161385daccc`  
		Last Modified: Wed, 10 Mar 2021 22:27:03 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e5caabff84d783ac1febddbbda13747e40e778a71899a540e1b82182dbc1f3`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce1afb0f0a252eb64ecf1b7bf79d8c945119ca0239b3c9d244ce747d6fbc5ee`  
		Last Modified: Wed, 10 Mar 2021 22:27:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b6e1e12ef3e96a6db7a95b4a95acd12749e270ae732c0681cba28455133f47`  
		Last Modified: Wed, 10 Mar 2021 22:27:53 GMT  
		Size: 235.2 MB (235223440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0869747a8b49ccaa9ef00163f7d429c5b735f4b2cbf088a52b9bf9e5a0743e9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a10f415b0d19985d54ed7945eca9c40343ad6dd851283e0f5c3dc4c391312e5`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7be938f74e1edf85b19d70b484a4d0c4a59d1843029996506b5db5552d4dd9`  
		Last Modified: Wed, 10 Mar 2021 22:27:00 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.23-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:ddb238e53f52fa3949339beb36fb5c2386918445e26542702b0bde1ea0dd1909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.0.23-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:83603f1754d1a692d10d88852407fcf458abaa727c6c5e6ea514fe94168ca216
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6032830526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:558fd300012714ba24dec1cb5b5bf8c12751e0ddf87616dbbad9d8bb3c4ecdaf`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:04:14 GMT
ENV MONGO_VERSION=4.0.23
# Wed, 10 Mar 2021 22:04:15 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.23-signed.msi
# Wed, 10 Mar 2021 22:04:16 GMT
ENV MONGO_DOWNLOAD_SHA256=32ff04b705f5a47c3974c8c5c7d859ea2fbfeb328101b2f84314e0cb6d3aea55
# Wed, 10 Mar 2021 22:07:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:07:27 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:07:28 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:07:29 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c58ccf67935e99262254c3dfe2e9c28aca0b9661d66a60414faf28c21fd5931`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb22f888d0e51d3f0e92fcdc193db77dbf964cd5926330d40a6f6f51e101275d`  
		Last Modified: Wed, 10 Mar 2021 22:28:12 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e71ce8b447156b65819454e2f150314b6ee92f7f76baf7bc1bb8aa389a0377d`  
		Last Modified: Wed, 10 Mar 2021 22:28:10 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45086bc178a2e2742f5a32caaef800e419a9b23a4c533fc9b79c3dac4e0f5986`  
		Last Modified: Wed, 10 Mar 2021 22:29:03 GMT  
		Size: 235.9 MB (235909789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315fb7f007e58410757d47f0971833f8d7162461a6d9ef05375f90110effd906`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52f0132f741b96fd2709a67f89be37cb6e0dd27685bc21d8fce68bc06412608`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e09528fa31b4c10649796974937ca7b3ce93a56e2d9aa80d683f25c517b8be`  
		Last Modified: Wed, 10 Mar 2021 22:28:09 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.23-xenial`

```console
$ docker pull mongo@sha256:760b9af6eab2cadc037868a13ed6ec6dec79c801cc00fd7b1680f847edd052f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.23-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:06c6b5dd62a46dbac54127b06c3fdf906e22afa54510049517990fda8a54da11
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156130343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0df4f86665738885bc4e9dc7b0576d90f45f34f11e9a047729c6854b6bf9a65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 11:59:24 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 11:59:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 11:59:45 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 11:59:45 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:00:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:01:20 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Fri, 26 Mar 2021 12:01:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:01:23 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:01:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:01:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:01:25 GMT
ENV MONGO_MAJOR=4.0
# Fri, 26 Mar 2021 12:01:25 GMT
ENV MONGO_VERSION=4.0.23
# Fri, 26 Mar 2021 12:01:27 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:01:49 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:01:51 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:01:51 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:01:52 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:01:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:01:52 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:01:52 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f48c36391ab27b893d30cb8749701c17aae74dba8ce49d7af701a5b1e11f222`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3f7696456b874ef2dd1f9f34a68caeb51b2354fcab687b40e6d05270f2ee48`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 2.9 MB (2906714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4dacfbe3d2ac79a7b70251ef94dd91bc4e2b0bfe77bd08df70a1945c1469af`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 1.3 MB (1305575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f630625fdedc3e1a0b430913884394118a03ac4314e123421f71ecd8126cef5c`  
		Last Modified: Fri, 26 Mar 2021 12:06:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6581891ba73f040b5728189e295d1f1e0f36fd802abbf95c431eae3cdd3f9d47`  
		Last Modified: Fri, 26 Mar 2021 12:06:39 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17a3cabb9decc8b2aeab50a695d73d3b154e6436bc21562d2e9a5a8202669a3`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dd736a5440e879ceef968361c521d055c97a6f7b5c0a83d0e1c96448f7ef18`  
		Last Modified: Fri, 26 Mar 2021 12:06:55 GMT  
		Size: 105.9 MB (105945768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63c9587c119b63b3822d648974ed9b7a1f504d3f2e623034512ba36276d967c`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4806e4fe4ce30e1bc3b7d8c20344e14193e2d4ed70afb4047b64fc7f597b66`  
		Last Modified: Fri, 26 Mar 2021 12:06:38 GMT  
		Size: 4.4 KB (4420 bytes)  
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

## `mongo:4.2`

```console
$ docker pull mongo@sha256:6b47e9e3f63c1b8e5384aedd470cb21b1c857f84ceb80f2e01bd611b596732e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:2d488b40a9c92757956a8218e99d2d7512ca85f285572a9d6499d1b0129e30f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165338616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a0c891d8e9f6ad7e547417382afe09ea2489bd0b9cf1cd863ac3bf2459a545`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:02:44 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 26 Mar 2021 12:02:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:02:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:02:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:02:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:02:47 GMT
ENV MONGO_MAJOR=4.2
# Fri, 26 Mar 2021 12:02:48 GMT
ENV MONGO_VERSION=4.2.13
# Fri, 26 Mar 2021 12:02:50 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:03:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:03:19 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:03:19 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:03:19 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:03:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:03:20 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:03:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f35d5694be470a1a7e6ddee921d7a0af615873d564b15bb30058f4a1307ca71`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c844b082d749f44f76101a3d69557c440409f125aff1510b504545695fcdde5c`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c6544f3957c7c8bd4ef17db9b875a0e753f075147873ad1baae1ffc41d56d`  
		Last Modified: Fri, 26 Mar 2021 12:07:25 GMT  
		Size: 129.8 MB (129812639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64ed3881190ea87cd2536caa391de6b2512a189d2f8323654c21fd675d873e`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827b807659b223cb1eb334ec910e3352a059ba3201bbba1cc374bc25e06d1714`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:37e6f51938653286c18fb2c9ed2f041cd9c1e9ee34caa0569190cfc793c67d31
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155378941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2c2d4a66cbbfd0b62adb391e656d34dc8f67907f412be89470ba741be2744a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:26:27 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 26 Mar 2021 14:26:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:26:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:26:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:26:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:26:35 GMT
ENV MONGO_MAJOR=4.2
# Fri, 26 Mar 2021 14:26:36 GMT
ENV MONGO_VERSION=4.2.13
# Fri, 26 Mar 2021 14:26:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:27:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:27:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:27:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:27:14 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:27:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:27:18 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:27:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd73a4f281f322b7c335b983af3e704becf170e25042e461a35917bb396a4a`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3980f9773ac88c25edb987a303eea134f480eb5011b91a2947adfd7047743`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fb162892eb9b9848756f015c4805b5500a34cef31dfdee045da4de97766925`  
		Last Modified: Fri, 26 Mar 2021 14:29:52 GMT  
		Size: 123.6 MB (123620696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe46ca5307a1298bdfd26f464dd9b72a081647cfd8e9506d5295694ac0f1673`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6cf059df426b71123e7a2c690c23bdecf4b1aad416bc09d0f86f1a758912891`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:6b3b01b217721cbc030457ed1f2da2641803730a535f2bf246b317331bb39e40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752476041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c7a216e1c8d0d3fe0f7a600984c89dea4f73c319cd44f332a92aa47153b07e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:21:31 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:21:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:21:33 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:23:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:23:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:23:51 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:23:52 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600f4a553eeb85f3a6189c85e5cf7ffb6ac69df76c572e17b72912781f7f7704`  
		Last Modified: Mon, 22 Mar 2021 19:34:51 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5176f03f404b25cce3e71601a609da870ceeba6a126a9caf51a3df6eb9e913`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4901b162524e64df5a81b5fcd74ca2aa3135e7976a543d5f318ee17268d6695`  
		Last Modified: Mon, 22 Mar 2021 19:34:48 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbdcb0f45bb89d337a5074de5df20a189ad7116928fb421d7e2003ffb6f083c`  
		Last Modified: Mon, 22 Mar 2021 19:35:49 GMT  
		Size: 290.9 MB (290931749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4c662c7db65e9fcecc8610464b842b104b66ac0a250056593ca7b82c9c5a38`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf69a37404e213cbf18fa16be134d54bc756d88374cac17868844db45b0fd7`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd28f19088183d0b3fb758f51ca187ed5fc935e9d177a0b101cd275cecd33ae8`  
		Last Modified: Mon, 22 Mar 2021 19:34:46 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:1cb33bac838bd8415ada8c00ec00bf2b761115554608c60209597d6db5455a39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088555115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cea8db6b268240a70ea150a97882ed9426a00dc7701616fbba7b24a1735a34a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:23:59 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:24:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:24:02 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:27:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:27:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:27:16 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eaa81b3a4a570431be2fe69af41fb30429cea059d798a0cb17154639d1cbf94`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371b356126c8d7b3acc71adfbd9bca79df0d778a4cf7d0c0e3373d59febe94bb`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdfeb41feece886e063a1f3fbff19116f71799474a77b7f8e82ec322e64b91`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21da404b9fb900087a2abbfe99291b231824f84e7603535a354a422929180d51`  
		Last Modified: Mon, 22 Mar 2021 19:41:43 GMT  
		Size: 291.6 MB (291634727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e2cf3619af6549d9aff1254032646d5fc1f2219efaafabb2771b8d415de926`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e001ea11a85c7d5904cb3acb12de7b6ea62a553133e301b9cbabf9cd31ab8`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e624818326147f8bb5b2370555ec81ee4887ce78cab3ea06b6cb4822bcbce4c`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:3eaf7d0b3de4e97d5e4c794e2cb43b402a1835c8ccc7b669d4a78d062a51b754
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:2d488b40a9c92757956a8218e99d2d7512ca85f285572a9d6499d1b0129e30f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165338616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a0c891d8e9f6ad7e547417382afe09ea2489bd0b9cf1cd863ac3bf2459a545`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:02:44 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 26 Mar 2021 12:02:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:02:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:02:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:02:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:02:47 GMT
ENV MONGO_MAJOR=4.2
# Fri, 26 Mar 2021 12:02:48 GMT
ENV MONGO_VERSION=4.2.13
# Fri, 26 Mar 2021 12:02:50 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:03:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:03:19 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:03:19 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:03:19 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:03:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:03:20 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:03:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f35d5694be470a1a7e6ddee921d7a0af615873d564b15bb30058f4a1307ca71`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c844b082d749f44f76101a3d69557c440409f125aff1510b504545695fcdde5c`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c6544f3957c7c8bd4ef17db9b875a0e753f075147873ad1baae1ffc41d56d`  
		Last Modified: Fri, 26 Mar 2021 12:07:25 GMT  
		Size: 129.8 MB (129812639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64ed3881190ea87cd2536caa391de6b2512a189d2f8323654c21fd675d873e`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827b807659b223cb1eb334ec910e3352a059ba3201bbba1cc374bc25e06d1714`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:37e6f51938653286c18fb2c9ed2f041cd9c1e9ee34caa0569190cfc793c67d31
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155378941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2c2d4a66cbbfd0b62adb391e656d34dc8f67907f412be89470ba741be2744a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:26:27 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 26 Mar 2021 14:26:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:26:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:26:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:26:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:26:35 GMT
ENV MONGO_MAJOR=4.2
# Fri, 26 Mar 2021 14:26:36 GMT
ENV MONGO_VERSION=4.2.13
# Fri, 26 Mar 2021 14:26:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:27:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:27:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:27:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:27:14 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:27:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:27:18 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:27:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd73a4f281f322b7c335b983af3e704becf170e25042e461a35917bb396a4a`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3980f9773ac88c25edb987a303eea134f480eb5011b91a2947adfd7047743`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fb162892eb9b9848756f015c4805b5500a34cef31dfdee045da4de97766925`  
		Last Modified: Fri, 26 Mar 2021 14:29:52 GMT  
		Size: 123.6 MB (123620696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe46ca5307a1298bdfd26f464dd9b72a081647cfd8e9506d5295694ac0f1673`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6cf059df426b71123e7a2c690c23bdecf4b1aad416bc09d0f86f1a758912891`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:f07785bdb802704b36d70adcd8b6417e694a4351e483003ecaa1e6806e489122
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:6b3b01b217721cbc030457ed1f2da2641803730a535f2bf246b317331bb39e40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752476041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c7a216e1c8d0d3fe0f7a600984c89dea4f73c319cd44f332a92aa47153b07e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:21:31 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:21:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:21:33 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:23:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:23:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:23:51 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:23:52 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600f4a553eeb85f3a6189c85e5cf7ffb6ac69df76c572e17b72912781f7f7704`  
		Last Modified: Mon, 22 Mar 2021 19:34:51 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5176f03f404b25cce3e71601a609da870ceeba6a126a9caf51a3df6eb9e913`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4901b162524e64df5a81b5fcd74ca2aa3135e7976a543d5f318ee17268d6695`  
		Last Modified: Mon, 22 Mar 2021 19:34:48 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbdcb0f45bb89d337a5074de5df20a189ad7116928fb421d7e2003ffb6f083c`  
		Last Modified: Mon, 22 Mar 2021 19:35:49 GMT  
		Size: 290.9 MB (290931749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4c662c7db65e9fcecc8610464b842b104b66ac0a250056593ca7b82c9c5a38`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf69a37404e213cbf18fa16be134d54bc756d88374cac17868844db45b0fd7`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd28f19088183d0b3fb758f51ca187ed5fc935e9d177a0b101cd275cecd33ae8`  
		Last Modified: Mon, 22 Mar 2021 19:34:46 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:1cb33bac838bd8415ada8c00ec00bf2b761115554608c60209597d6db5455a39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088555115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cea8db6b268240a70ea150a97882ed9426a00dc7701616fbba7b24a1735a34a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:23:59 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:24:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:24:02 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:27:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:27:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:27:16 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eaa81b3a4a570431be2fe69af41fb30429cea059d798a0cb17154639d1cbf94`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371b356126c8d7b3acc71adfbd9bca79df0d778a4cf7d0c0e3373d59febe94bb`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdfeb41feece886e063a1f3fbff19116f71799474a77b7f8e82ec322e64b91`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21da404b9fb900087a2abbfe99291b231824f84e7603535a354a422929180d51`  
		Last Modified: Mon, 22 Mar 2021 19:41:43 GMT  
		Size: 291.6 MB (291634727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e2cf3619af6549d9aff1254032646d5fc1f2219efaafabb2771b8d415de926`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e001ea11a85c7d5904cb3acb12de7b6ea62a553133e301b9cbabf9cd31ab8`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e624818326147f8bb5b2370555ec81ee4887ce78cab3ea06b6cb4822bcbce4c`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:5bae54912721caef62183a4849ea80e0ac1971660c8cbe95b61688a9778b4c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:6b3b01b217721cbc030457ed1f2da2641803730a535f2bf246b317331bb39e40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752476041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c7a216e1c8d0d3fe0f7a600984c89dea4f73c319cd44f332a92aa47153b07e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:21:31 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:21:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:21:33 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:23:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:23:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:23:51 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:23:52 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600f4a553eeb85f3a6189c85e5cf7ffb6ac69df76c572e17b72912781f7f7704`  
		Last Modified: Mon, 22 Mar 2021 19:34:51 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5176f03f404b25cce3e71601a609da870ceeba6a126a9caf51a3df6eb9e913`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4901b162524e64df5a81b5fcd74ca2aa3135e7976a543d5f318ee17268d6695`  
		Last Modified: Mon, 22 Mar 2021 19:34:48 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbdcb0f45bb89d337a5074de5df20a189ad7116928fb421d7e2003ffb6f083c`  
		Last Modified: Mon, 22 Mar 2021 19:35:49 GMT  
		Size: 290.9 MB (290931749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4c662c7db65e9fcecc8610464b842b104b66ac0a250056593ca7b82c9c5a38`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf69a37404e213cbf18fa16be134d54bc756d88374cac17868844db45b0fd7`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd28f19088183d0b3fb758f51ca187ed5fc935e9d177a0b101cd275cecd33ae8`  
		Last Modified: Mon, 22 Mar 2021 19:34:46 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:aeadd0cbc2d85d9be88a9a6d02054f8ee717488c079f82410c30fb1a4425a40b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:1cb33bac838bd8415ada8c00ec00bf2b761115554608c60209597d6db5455a39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088555115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cea8db6b268240a70ea150a97882ed9426a00dc7701616fbba7b24a1735a34a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:23:59 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:24:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:24:02 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:27:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:27:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:27:16 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eaa81b3a4a570431be2fe69af41fb30429cea059d798a0cb17154639d1cbf94`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371b356126c8d7b3acc71adfbd9bca79df0d778a4cf7d0c0e3373d59febe94bb`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdfeb41feece886e063a1f3fbff19116f71799474a77b7f8e82ec322e64b91`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21da404b9fb900087a2abbfe99291b231824f84e7603535a354a422929180d51`  
		Last Modified: Mon, 22 Mar 2021 19:41:43 GMT  
		Size: 291.6 MB (291634727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e2cf3619af6549d9aff1254032646d5fc1f2219efaafabb2771b8d415de926`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e001ea11a85c7d5904cb3acb12de7b6ea62a553133e301b9cbabf9cd31ab8`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e624818326147f8bb5b2370555ec81ee4887ce78cab3ea06b6cb4822bcbce4c`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.13`

```console
$ docker pull mongo@sha256:6b47e9e3f63c1b8e5384aedd470cb21b1c857f84ceb80f2e01bd611b596732e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.2.13` - linux; amd64

```console
$ docker pull mongo@sha256:2d488b40a9c92757956a8218e99d2d7512ca85f285572a9d6499d1b0129e30f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165338616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a0c891d8e9f6ad7e547417382afe09ea2489bd0b9cf1cd863ac3bf2459a545`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:02:44 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 26 Mar 2021 12:02:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:02:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:02:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:02:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:02:47 GMT
ENV MONGO_MAJOR=4.2
# Fri, 26 Mar 2021 12:02:48 GMT
ENV MONGO_VERSION=4.2.13
# Fri, 26 Mar 2021 12:02:50 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:03:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:03:19 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:03:19 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:03:19 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:03:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:03:20 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:03:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f35d5694be470a1a7e6ddee921d7a0af615873d564b15bb30058f4a1307ca71`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c844b082d749f44f76101a3d69557c440409f125aff1510b504545695fcdde5c`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c6544f3957c7c8bd4ef17db9b875a0e753f075147873ad1baae1ffc41d56d`  
		Last Modified: Fri, 26 Mar 2021 12:07:25 GMT  
		Size: 129.8 MB (129812639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64ed3881190ea87cd2536caa391de6b2512a189d2f8323654c21fd675d873e`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827b807659b223cb1eb334ec910e3352a059ba3201bbba1cc374bc25e06d1714`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.13` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:37e6f51938653286c18fb2c9ed2f041cd9c1e9ee34caa0569190cfc793c67d31
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155378941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2c2d4a66cbbfd0b62adb391e656d34dc8f67907f412be89470ba741be2744a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:26:27 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 26 Mar 2021 14:26:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:26:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:26:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:26:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:26:35 GMT
ENV MONGO_MAJOR=4.2
# Fri, 26 Mar 2021 14:26:36 GMT
ENV MONGO_VERSION=4.2.13
# Fri, 26 Mar 2021 14:26:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:27:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:27:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:27:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:27:14 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:27:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:27:18 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:27:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd73a4f281f322b7c335b983af3e704becf170e25042e461a35917bb396a4a`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3980f9773ac88c25edb987a303eea134f480eb5011b91a2947adfd7047743`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fb162892eb9b9848756f015c4805b5500a34cef31dfdee045da4de97766925`  
		Last Modified: Fri, 26 Mar 2021 14:29:52 GMT  
		Size: 123.6 MB (123620696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe46ca5307a1298bdfd26f464dd9b72a081647cfd8e9506d5295694ac0f1673`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6cf059df426b71123e7a2c690c23bdecf4b1aad416bc09d0f86f1a758912891`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.13` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:6b3b01b217721cbc030457ed1f2da2641803730a535f2bf246b317331bb39e40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752476041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c7a216e1c8d0d3fe0f7a600984c89dea4f73c319cd44f332a92aa47153b07e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:21:31 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:21:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:21:33 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:23:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:23:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:23:51 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:23:52 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600f4a553eeb85f3a6189c85e5cf7ffb6ac69df76c572e17b72912781f7f7704`  
		Last Modified: Mon, 22 Mar 2021 19:34:51 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5176f03f404b25cce3e71601a609da870ceeba6a126a9caf51a3df6eb9e913`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4901b162524e64df5a81b5fcd74ca2aa3135e7976a543d5f318ee17268d6695`  
		Last Modified: Mon, 22 Mar 2021 19:34:48 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbdcb0f45bb89d337a5074de5df20a189ad7116928fb421d7e2003ffb6f083c`  
		Last Modified: Mon, 22 Mar 2021 19:35:49 GMT  
		Size: 290.9 MB (290931749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4c662c7db65e9fcecc8610464b842b104b66ac0a250056593ca7b82c9c5a38`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf69a37404e213cbf18fa16be134d54bc756d88374cac17868844db45b0fd7`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd28f19088183d0b3fb758f51ca187ed5fc935e9d177a0b101cd275cecd33ae8`  
		Last Modified: Mon, 22 Mar 2021 19:34:46 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.13` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:1cb33bac838bd8415ada8c00ec00bf2b761115554608c60209597d6db5455a39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088555115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cea8db6b268240a70ea150a97882ed9426a00dc7701616fbba7b24a1735a34a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:23:59 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:24:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:24:02 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:27:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:27:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:27:16 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eaa81b3a4a570431be2fe69af41fb30429cea059d798a0cb17154639d1cbf94`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371b356126c8d7b3acc71adfbd9bca79df0d778a4cf7d0c0e3373d59febe94bb`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdfeb41feece886e063a1f3fbff19116f71799474a77b7f8e82ec322e64b91`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21da404b9fb900087a2abbfe99291b231824f84e7603535a354a422929180d51`  
		Last Modified: Mon, 22 Mar 2021 19:41:43 GMT  
		Size: 291.6 MB (291634727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e2cf3619af6549d9aff1254032646d5fc1f2219efaafabb2771b8d415de926`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e001ea11a85c7d5904cb3acb12de7b6ea62a553133e301b9cbabf9cd31ab8`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e624818326147f8bb5b2370555ec81ee4887ce78cab3ea06b6cb4822bcbce4c`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.13-bionic`

```console
$ docker pull mongo@sha256:3eaf7d0b3de4e97d5e4c794e2cb43b402a1835c8ccc7b669d4a78d062a51b754
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2.13-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:2d488b40a9c92757956a8218e99d2d7512ca85f285572a9d6499d1b0129e30f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165338616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a0c891d8e9f6ad7e547417382afe09ea2489bd0b9cf1cd863ac3bf2459a545`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:02:44 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 26 Mar 2021 12:02:46 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:02:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:02:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:02:47 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:02:47 GMT
ENV MONGO_MAJOR=4.2
# Fri, 26 Mar 2021 12:02:48 GMT
ENV MONGO_VERSION=4.2.13
# Fri, 26 Mar 2021 12:02:50 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:03:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:03:19 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:03:19 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:03:19 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:03:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:03:20 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:03:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f35d5694be470a1a7e6ddee921d7a0af615873d564b15bb30058f4a1307ca71`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c844b082d749f44f76101a3d69557c440409f125aff1510b504545695fcdde5c`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c6544f3957c7c8bd4ef17db9b875a0e753f075147873ad1baae1ffc41d56d`  
		Last Modified: Fri, 26 Mar 2021 12:07:25 GMT  
		Size: 129.8 MB (129812639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64ed3881190ea87cd2536caa391de6b2512a189d2f8323654c21fd675d873e`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827b807659b223cb1eb334ec910e3352a059ba3201bbba1cc374bc25e06d1714`  
		Last Modified: Fri, 26 Mar 2021 12:07:07 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.13-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:37e6f51938653286c18fb2c9ed2f041cd9c1e9ee34caa0569190cfc793c67d31
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155378941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a2c2d4a66cbbfd0b62adb391e656d34dc8f67907f412be89470ba741be2744a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:26:27 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Fri, 26 Mar 2021 14:26:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:26:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:26:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:26:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:26:35 GMT
ENV MONGO_MAJOR=4.2
# Fri, 26 Mar 2021 14:26:36 GMT
ENV MONGO_VERSION=4.2.13
# Fri, 26 Mar 2021 14:26:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:27:06 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:27:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:27:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:27:14 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:27:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:27:18 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:27:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd73a4f281f322b7c335b983af3e704becf170e25042e461a35917bb396a4a`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3980f9773ac88c25edb987a303eea134f480eb5011b91a2947adfd7047743`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fb162892eb9b9848756f015c4805b5500a34cef31dfdee045da4de97766925`  
		Last Modified: Fri, 26 Mar 2021 14:29:52 GMT  
		Size: 123.6 MB (123620696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe46ca5307a1298bdfd26f464dd9b72a081647cfd8e9506d5295694ac0f1673`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6cf059df426b71123e7a2c690c23bdecf4b1aad416bc09d0f86f1a758912891`  
		Last Modified: Fri, 26 Mar 2021 14:29:27 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.13-windowsservercore`

```console
$ docker pull mongo@sha256:f07785bdb802704b36d70adcd8b6417e694a4351e483003ecaa1e6806e489122
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.2.13-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:6b3b01b217721cbc030457ed1f2da2641803730a535f2bf246b317331bb39e40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752476041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c7a216e1c8d0d3fe0f7a600984c89dea4f73c319cd44f332a92aa47153b07e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:21:31 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:21:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:21:33 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:23:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:23:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:23:51 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:23:52 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600f4a553eeb85f3a6189c85e5cf7ffb6ac69df76c572e17b72912781f7f7704`  
		Last Modified: Mon, 22 Mar 2021 19:34:51 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5176f03f404b25cce3e71601a609da870ceeba6a126a9caf51a3df6eb9e913`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4901b162524e64df5a81b5fcd74ca2aa3135e7976a543d5f318ee17268d6695`  
		Last Modified: Mon, 22 Mar 2021 19:34:48 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbdcb0f45bb89d337a5074de5df20a189ad7116928fb421d7e2003ffb6f083c`  
		Last Modified: Mon, 22 Mar 2021 19:35:49 GMT  
		Size: 290.9 MB (290931749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4c662c7db65e9fcecc8610464b842b104b66ac0a250056593ca7b82c9c5a38`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf69a37404e213cbf18fa16be134d54bc756d88374cac17868844db45b0fd7`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd28f19088183d0b3fb758f51ca187ed5fc935e9d177a0b101cd275cecd33ae8`  
		Last Modified: Mon, 22 Mar 2021 19:34:46 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.13-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:1cb33bac838bd8415ada8c00ec00bf2b761115554608c60209597d6db5455a39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088555115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cea8db6b268240a70ea150a97882ed9426a00dc7701616fbba7b24a1735a34a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:23:59 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:24:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:24:02 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:27:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:27:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:27:16 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eaa81b3a4a570431be2fe69af41fb30429cea059d798a0cb17154639d1cbf94`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371b356126c8d7b3acc71adfbd9bca79df0d778a4cf7d0c0e3373d59febe94bb`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdfeb41feece886e063a1f3fbff19116f71799474a77b7f8e82ec322e64b91`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21da404b9fb900087a2abbfe99291b231824f84e7603535a354a422929180d51`  
		Last Modified: Mon, 22 Mar 2021 19:41:43 GMT  
		Size: 291.6 MB (291634727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e2cf3619af6549d9aff1254032646d5fc1f2219efaafabb2771b8d415de926`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e001ea11a85c7d5904cb3acb12de7b6ea62a553133e301b9cbabf9cd31ab8`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e624818326147f8bb5b2370555ec81ee4887ce78cab3ea06b6cb4822bcbce4c`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.13-windowsservercore-1809`

```console
$ docker pull mongo@sha256:5bae54912721caef62183a4849ea80e0ac1971660c8cbe95b61688a9778b4c09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:4.2.13-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:6b3b01b217721cbc030457ed1f2da2641803730a535f2bf246b317331bb39e40
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2752476041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81c7a216e1c8d0d3fe0f7a600984c89dea4f73c319cd44f332a92aa47153b07e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:21:31 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:21:32 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:21:33 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:23:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:23:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:23:51 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:23:52 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600f4a553eeb85f3a6189c85e5cf7ffb6ac69df76c572e17b72912781f7f7704`  
		Last Modified: Mon, 22 Mar 2021 19:34:51 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5176f03f404b25cce3e71601a609da870ceeba6a126a9caf51a3df6eb9e913`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4901b162524e64df5a81b5fcd74ca2aa3135e7976a543d5f318ee17268d6695`  
		Last Modified: Mon, 22 Mar 2021 19:34:48 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbdcb0f45bb89d337a5074de5df20a189ad7116928fb421d7e2003ffb6f083c`  
		Last Modified: Mon, 22 Mar 2021 19:35:49 GMT  
		Size: 290.9 MB (290931749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4c662c7db65e9fcecc8610464b842b104b66ac0a250056593ca7b82c9c5a38`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cf69a37404e213cbf18fa16be134d54bc756d88374cac17868844db45b0fd7`  
		Last Modified: Mon, 22 Mar 2021 19:34:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd28f19088183d0b3fb758f51ca187ed5fc935e9d177a0b101cd275cecd33ae8`  
		Last Modified: Mon, 22 Mar 2021 19:34:46 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.13-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:aeadd0cbc2d85d9be88a9a6d02054f8ee717488c079f82410c30fb1a4425a40b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.2.13-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:1cb33bac838bd8415ada8c00ec00bf2b761115554608c60209597d6db5455a39
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6088555115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cea8db6b268240a70ea150a97882ed9426a00dc7701616fbba7b24a1735a34a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 22 Mar 2021 19:23:59 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:24:00 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.13-signed.msi
# Mon, 22 Mar 2021 19:24:02 GMT
ENV MONGO_DOWNLOAD_SHA256=36253a0bac369179e6906144d67458c9547ae6bfa2680b2440d2538c7de25230
# Mon, 22 Mar 2021 19:27:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 22 Mar 2021 19:27:15 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 22 Mar 2021 19:27:16 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eaa81b3a4a570431be2fe69af41fb30429cea059d798a0cb17154639d1cbf94`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371b356126c8d7b3acc71adfbd9bca79df0d778a4cf7d0c0e3373d59febe94bb`  
		Last Modified: Mon, 22 Mar 2021 19:36:05 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdfeb41feece886e063a1f3fbff19116f71799474a77b7f8e82ec322e64b91`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21da404b9fb900087a2abbfe99291b231824f84e7603535a354a422929180d51`  
		Last Modified: Mon, 22 Mar 2021 19:41:43 GMT  
		Size: 291.6 MB (291634727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e2cf3619af6549d9aff1254032646d5fc1f2219efaafabb2771b8d415de926`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e001ea11a85c7d5904cb3acb12de7b6ea62a553133e301b9cbabf9cd31ab8`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e624818326147f8bb5b2370555ec81ee4887ce78cab3ea06b6cb4822bcbce4c`  
		Last Modified: Mon, 22 Mar 2021 19:36:02 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4`

```console
$ docker pull mongo@sha256:75a5f624bd6d14254e0d84c2833f576109672750aaf2bf01d61cb5ead44f4505
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.4` - linux; amd64

```console
$ docker pull mongo@sha256:424cadd696e9a0dbc691a4e2680722f2a9e8ab604374b482e2a9890fdc8ab0c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175093468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03be0dc25f8732caef29f051c91ce7447f8305738032e91c23b13cba3e74e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:03:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 12:03:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:03:30 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:03:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 12:03:32 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:05:11 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:05:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:05:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:05:13 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:05:13 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:05:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8c3715616e84c33c0038ba795484161fd38d0930d82e09b68283a1a18f451`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac42b84e850eda3c7655d1937d8a023de9fa68199e383acb2262d323442219d`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724cb122c25fe9272d20cdf76c45c6aab3f447f4e6f3b0ebfdfbb46724eb2ef`  
		Last Modified: Fri, 26 Mar 2021 12:08:02 GMT  
		Size: 139.6 MB (139567497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe10b8b0c12777d4c337f611abaf127960fab70650c1f7ad27073ac9bd2521`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e025c87f29ce34b87590b9f4dcc0b3b164ddba3bb903fcb1b9e0b91b0c7a7b`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:18b9ba93b6208cd80e1a723a241269f6e1eb44bfaa6ce1dd3de9be32f717daf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167536780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58929ecfa3caf151a12d97acb343f9b94bd867df524c3cdc9f60a00f46df5496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:27:42 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 14:27:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:27:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:27:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:50 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 14:27:51 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 14:27:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:28:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:28:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:28:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:28:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:28:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:28:46 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:28:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada24af95b05b298538ab63d883be491085362960192889c5c5d07627dfc446`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877762b7148d23f4cef028d66cb3f7ab51c8fb232f674d8cb2ce546675f0803`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a783117ad78ea48199bae4e86a245b13ae202fd98202cc2d5cd9df8bb0564432`  
		Last Modified: Fri, 26 Mar 2021 14:30:33 GMT  
		Size: 135.8 MB (135778542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc369a412303d9bc7d67b498032752b974cc1cf3a1854beba31c5b7705ca819`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ff00ed0d4b2c1c9040bac960068c8cf865ddf3b3417b0b4bfa0372df05ba06`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; s390x

```console
$ docker pull mongo@sha256:cbb067bdf193c627f85874531f3d5c0b692d81db482a9c0c69d026a81383afe5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169136167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651556f82f603bac974f5788631fd43b058c3c818c1c6a96cf2e2dc5c2a0a289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:31 GMT
ADD file:1c7dbc64158234b813a2eeff0c325efa0cff7c3983e93fc9f7de0004e901c2c1 in / 
# Thu, 25 Mar 2021 22:53:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:35 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 08:57:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 08:57:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:57:20 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 08:57:21 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 08:57:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 08:57:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 08:57:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 08:57:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 08:57:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 08:57:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 08:57:41 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 08:57:42 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 08:58:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 08:58:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 08:58:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 08:58:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 08:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:58:33 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 08:58:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:bf8da0ed3f9ec60019cec9fac782f04b7281f232a86e7613579e54c348b8402b`  
		Last Modified: Thu, 25 Mar 2021 22:54:27 GMT  
		Size: 25.4 MB (25381419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de72c87d1d7a4355d21e04b9ce611f427f0c84ee6705dd53a1fd990012cefdd6`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffe2f5d8eac8afe4b79981c9c93b44c985dbb7b3bb5f9af5e918c6aac415fcf`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2808460e51d63b807cb6cb00bf034b7f2643599362ad55d9df26c6bc9ffad42c`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400c3133d141345611000d1de01cfadc8b8a785e209b80afcafa9214669ffd8f`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 2.7 MB (2708345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cdf5b66f6831b7db4ee570b487453c025248b2607e441c34db29488fcc35d4`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 5.7 MB (5747339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0de8bd807c307aaa480d335670e64efb51855df37c491f9e888d1848637001`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d58b3f14f22d07c415679c463eb1f4af10f1cbf89aa20fb46aaf3e31a41c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eef524d85fb192432f8eb7fc575cef6576292d4d47939a2b3650fd72dba5c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34edb6160fb71ce9809aec003c97570df6d05e2b19a1eb3ec267806ba9586f1`  
		Last Modified: Fri, 26 Mar 2021 08:59:21 GMT  
		Size: 135.3 MB (135289747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa65663451ec46890ca56252fcc498672e68e9b5dfa0df327c68150aa50226`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8215528e5cd8c0cb268785c0f8d75cfeb8ac2b40dd7f267effa9793d6fb487c5`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-bionic`

```console
$ docker pull mongo@sha256:1fdc0fd04f4c1006a41c81066521c8d396a4fe9cbbb7d8df99dfba9ba670bfe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:424cadd696e9a0dbc691a4e2680722f2a9e8ab604374b482e2a9890fdc8ab0c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175093468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03be0dc25f8732caef29f051c91ce7447f8305738032e91c23b13cba3e74e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:03:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 12:03:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:03:30 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:03:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 12:03:32 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:05:11 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:05:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:05:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:05:13 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:05:13 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:05:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8c3715616e84c33c0038ba795484161fd38d0930d82e09b68283a1a18f451`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac42b84e850eda3c7655d1937d8a023de9fa68199e383acb2262d323442219d`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724cb122c25fe9272d20cdf76c45c6aab3f447f4e6f3b0ebfdfbb46724eb2ef`  
		Last Modified: Fri, 26 Mar 2021 12:08:02 GMT  
		Size: 139.6 MB (139567497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe10b8b0c12777d4c337f611abaf127960fab70650c1f7ad27073ac9bd2521`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e025c87f29ce34b87590b9f4dcc0b3b164ddba3bb903fcb1b9e0b91b0c7a7b`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:18b9ba93b6208cd80e1a723a241269f6e1eb44bfaa6ce1dd3de9be32f717daf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167536780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58929ecfa3caf151a12d97acb343f9b94bd867df524c3cdc9f60a00f46df5496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:27:42 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 14:27:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:27:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:27:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:50 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 14:27:51 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 14:27:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:28:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:28:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:28:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:28:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:28:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:28:46 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:28:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada24af95b05b298538ab63d883be491085362960192889c5c5d07627dfc446`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877762b7148d23f4cef028d66cb3f7ab51c8fb232f674d8cb2ce546675f0803`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a783117ad78ea48199bae4e86a245b13ae202fd98202cc2d5cd9df8bb0564432`  
		Last Modified: Fri, 26 Mar 2021 14:30:33 GMT  
		Size: 135.8 MB (135778542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc369a412303d9bc7d67b498032752b974cc1cf3a1854beba31c5b7705ca819`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ff00ed0d4b2c1c9040bac960068c8cf865ddf3b3417b0b4bfa0372df05ba06`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:cbb067bdf193c627f85874531f3d5c0b692d81db482a9c0c69d026a81383afe5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169136167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651556f82f603bac974f5788631fd43b058c3c818c1c6a96cf2e2dc5c2a0a289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:31 GMT
ADD file:1c7dbc64158234b813a2eeff0c325efa0cff7c3983e93fc9f7de0004e901c2c1 in / 
# Thu, 25 Mar 2021 22:53:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:35 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 08:57:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 08:57:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:57:20 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 08:57:21 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 08:57:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 08:57:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 08:57:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 08:57:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 08:57:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 08:57:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 08:57:41 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 08:57:42 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 08:58:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 08:58:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 08:58:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 08:58:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 08:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:58:33 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 08:58:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:bf8da0ed3f9ec60019cec9fac782f04b7281f232a86e7613579e54c348b8402b`  
		Last Modified: Thu, 25 Mar 2021 22:54:27 GMT  
		Size: 25.4 MB (25381419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de72c87d1d7a4355d21e04b9ce611f427f0c84ee6705dd53a1fd990012cefdd6`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffe2f5d8eac8afe4b79981c9c93b44c985dbb7b3bb5f9af5e918c6aac415fcf`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2808460e51d63b807cb6cb00bf034b7f2643599362ad55d9df26c6bc9ffad42c`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400c3133d141345611000d1de01cfadc8b8a785e209b80afcafa9214669ffd8f`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 2.7 MB (2708345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cdf5b66f6831b7db4ee570b487453c025248b2607e441c34db29488fcc35d4`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 5.7 MB (5747339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0de8bd807c307aaa480d335670e64efb51855df37c491f9e888d1848637001`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d58b3f14f22d07c415679c463eb1f4af10f1cbf89aa20fb46aaf3e31a41c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eef524d85fb192432f8eb7fc575cef6576292d4d47939a2b3650fd72dba5c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34edb6160fb71ce9809aec003c97570df6d05e2b19a1eb3ec267806ba9586f1`  
		Last Modified: Fri, 26 Mar 2021 08:59:21 GMT  
		Size: 135.3 MB (135289747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa65663451ec46890ca56252fcc498672e68e9b5dfa0df327c68150aa50226`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8215528e5cd8c0cb268785c0f8d75cfeb8ac2b40dd7f267effa9793d6fb487c5`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore`

```console
$ docker pull mongo@sha256:015fbab5dc985d5281b38ea374ec95fe55adddab9f883b59e8b37c7c61090cba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.4-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:60acbac1cd7c075dc499da7ed7b6a9176c62fbab80a72afad59554330adc6d56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:4.4-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:13cc45bcbe04fd9d2f1acea62d4bc57a1a533cae59c01cfcc74bff9aa5f2a501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4`

```console
$ docker pull mongo@sha256:75a5f624bd6d14254e0d84c2833f576109672750aaf2bf01d61cb5ead44f4505
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.4.4` - linux; amd64

```console
$ docker pull mongo@sha256:424cadd696e9a0dbc691a4e2680722f2a9e8ab604374b482e2a9890fdc8ab0c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175093468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03be0dc25f8732caef29f051c91ce7447f8305738032e91c23b13cba3e74e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:03:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 12:03:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:03:30 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:03:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 12:03:32 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:05:11 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:05:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:05:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:05:13 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:05:13 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:05:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8c3715616e84c33c0038ba795484161fd38d0930d82e09b68283a1a18f451`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac42b84e850eda3c7655d1937d8a023de9fa68199e383acb2262d323442219d`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724cb122c25fe9272d20cdf76c45c6aab3f447f4e6f3b0ebfdfbb46724eb2ef`  
		Last Modified: Fri, 26 Mar 2021 12:08:02 GMT  
		Size: 139.6 MB (139567497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe10b8b0c12777d4c337f611abaf127960fab70650c1f7ad27073ac9bd2521`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e025c87f29ce34b87590b9f4dcc0b3b164ddba3bb903fcb1b9e0b91b0c7a7b`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:18b9ba93b6208cd80e1a723a241269f6e1eb44bfaa6ce1dd3de9be32f717daf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167536780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58929ecfa3caf151a12d97acb343f9b94bd867df524c3cdc9f60a00f46df5496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:27:42 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 14:27:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:27:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:27:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:50 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 14:27:51 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 14:27:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:28:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:28:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:28:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:28:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:28:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:28:46 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:28:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada24af95b05b298538ab63d883be491085362960192889c5c5d07627dfc446`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877762b7148d23f4cef028d66cb3f7ab51c8fb232f674d8cb2ce546675f0803`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a783117ad78ea48199bae4e86a245b13ae202fd98202cc2d5cd9df8bb0564432`  
		Last Modified: Fri, 26 Mar 2021 14:30:33 GMT  
		Size: 135.8 MB (135778542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc369a412303d9bc7d67b498032752b974cc1cf3a1854beba31c5b7705ca819`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ff00ed0d4b2c1c9040bac960068c8cf865ddf3b3417b0b4bfa0372df05ba06`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4` - linux; s390x

```console
$ docker pull mongo@sha256:cbb067bdf193c627f85874531f3d5c0b692d81db482a9c0c69d026a81383afe5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169136167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651556f82f603bac974f5788631fd43b058c3c818c1c6a96cf2e2dc5c2a0a289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:31 GMT
ADD file:1c7dbc64158234b813a2eeff0c325efa0cff7c3983e93fc9f7de0004e901c2c1 in / 
# Thu, 25 Mar 2021 22:53:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:35 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 08:57:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 08:57:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:57:20 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 08:57:21 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 08:57:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 08:57:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 08:57:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 08:57:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 08:57:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 08:57:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 08:57:41 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 08:57:42 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 08:58:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 08:58:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 08:58:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 08:58:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 08:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:58:33 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 08:58:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:bf8da0ed3f9ec60019cec9fac782f04b7281f232a86e7613579e54c348b8402b`  
		Last Modified: Thu, 25 Mar 2021 22:54:27 GMT  
		Size: 25.4 MB (25381419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de72c87d1d7a4355d21e04b9ce611f427f0c84ee6705dd53a1fd990012cefdd6`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffe2f5d8eac8afe4b79981c9c93b44c985dbb7b3bb5f9af5e918c6aac415fcf`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2808460e51d63b807cb6cb00bf034b7f2643599362ad55d9df26c6bc9ffad42c`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400c3133d141345611000d1de01cfadc8b8a785e209b80afcafa9214669ffd8f`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 2.7 MB (2708345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cdf5b66f6831b7db4ee570b487453c025248b2607e441c34db29488fcc35d4`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 5.7 MB (5747339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0de8bd807c307aaa480d335670e64efb51855df37c491f9e888d1848637001`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d58b3f14f22d07c415679c463eb1f4af10f1cbf89aa20fb46aaf3e31a41c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eef524d85fb192432f8eb7fc575cef6576292d4d47939a2b3650fd72dba5c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34edb6160fb71ce9809aec003c97570df6d05e2b19a1eb3ec267806ba9586f1`  
		Last Modified: Fri, 26 Mar 2021 08:59:21 GMT  
		Size: 135.3 MB (135289747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa65663451ec46890ca56252fcc498672e68e9b5dfa0df327c68150aa50226`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8215528e5cd8c0cb268785c0f8d75cfeb8ac2b40dd7f267effa9793d6fb487c5`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4-bionic`

```console
$ docker pull mongo@sha256:1fdc0fd04f4c1006a41c81066521c8d396a4fe9cbbb7d8df99dfba9ba670bfe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:424cadd696e9a0dbc691a4e2680722f2a9e8ab604374b482e2a9890fdc8ab0c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175093468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03be0dc25f8732caef29f051c91ce7447f8305738032e91c23b13cba3e74e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:03:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 12:03:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:03:30 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:03:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 12:03:32 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:05:11 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:05:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:05:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:05:13 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:05:13 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:05:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8c3715616e84c33c0038ba795484161fd38d0930d82e09b68283a1a18f451`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac42b84e850eda3c7655d1937d8a023de9fa68199e383acb2262d323442219d`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724cb122c25fe9272d20cdf76c45c6aab3f447f4e6f3b0ebfdfbb46724eb2ef`  
		Last Modified: Fri, 26 Mar 2021 12:08:02 GMT  
		Size: 139.6 MB (139567497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe10b8b0c12777d4c337f611abaf127960fab70650c1f7ad27073ac9bd2521`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e025c87f29ce34b87590b9f4dcc0b3b164ddba3bb903fcb1b9e0b91b0c7a7b`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:18b9ba93b6208cd80e1a723a241269f6e1eb44bfaa6ce1dd3de9be32f717daf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167536780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58929ecfa3caf151a12d97acb343f9b94bd867df524c3cdc9f60a00f46df5496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:27:42 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 14:27:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:27:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:27:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:50 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 14:27:51 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 14:27:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:28:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:28:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:28:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:28:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:28:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:28:46 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:28:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada24af95b05b298538ab63d883be491085362960192889c5c5d07627dfc446`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877762b7148d23f4cef028d66cb3f7ab51c8fb232f674d8cb2ce546675f0803`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a783117ad78ea48199bae4e86a245b13ae202fd98202cc2d5cd9df8bb0564432`  
		Last Modified: Fri, 26 Mar 2021 14:30:33 GMT  
		Size: 135.8 MB (135778542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc369a412303d9bc7d67b498032752b974cc1cf3a1854beba31c5b7705ca819`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ff00ed0d4b2c1c9040bac960068c8cf865ddf3b3417b0b4bfa0372df05ba06`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:cbb067bdf193c627f85874531f3d5c0b692d81db482a9c0c69d026a81383afe5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169136167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651556f82f603bac974f5788631fd43b058c3c818c1c6a96cf2e2dc5c2a0a289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:31 GMT
ADD file:1c7dbc64158234b813a2eeff0c325efa0cff7c3983e93fc9f7de0004e901c2c1 in / 
# Thu, 25 Mar 2021 22:53:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:35 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 08:57:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 08:57:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:57:20 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 08:57:21 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 08:57:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 08:57:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 08:57:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 08:57:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 08:57:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 08:57:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 08:57:41 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 08:57:42 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 08:58:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 08:58:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 08:58:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 08:58:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 08:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:58:33 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 08:58:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:bf8da0ed3f9ec60019cec9fac782f04b7281f232a86e7613579e54c348b8402b`  
		Last Modified: Thu, 25 Mar 2021 22:54:27 GMT  
		Size: 25.4 MB (25381419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de72c87d1d7a4355d21e04b9ce611f427f0c84ee6705dd53a1fd990012cefdd6`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffe2f5d8eac8afe4b79981c9c93b44c985dbb7b3bb5f9af5e918c6aac415fcf`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2808460e51d63b807cb6cb00bf034b7f2643599362ad55d9df26c6bc9ffad42c`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400c3133d141345611000d1de01cfadc8b8a785e209b80afcafa9214669ffd8f`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 2.7 MB (2708345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cdf5b66f6831b7db4ee570b487453c025248b2607e441c34db29488fcc35d4`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 5.7 MB (5747339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0de8bd807c307aaa480d335670e64efb51855df37c491f9e888d1848637001`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d58b3f14f22d07c415679c463eb1f4af10f1cbf89aa20fb46aaf3e31a41c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eef524d85fb192432f8eb7fc575cef6576292d4d47939a2b3650fd72dba5c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34edb6160fb71ce9809aec003c97570df6d05e2b19a1eb3ec267806ba9586f1`  
		Last Modified: Fri, 26 Mar 2021 08:59:21 GMT  
		Size: 135.3 MB (135289747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa65663451ec46890ca56252fcc498672e68e9b5dfa0df327c68150aa50226`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8215528e5cd8c0cb268785c0f8d75cfeb8ac2b40dd7f267effa9793d6fb487c5`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4-windowsservercore`

```console
$ docker pull mongo@sha256:015fbab5dc985d5281b38ea374ec95fe55adddab9f883b59e8b37c7c61090cba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.4.4-windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4-windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:60acbac1cd7c075dc499da7ed7b6a9176c62fbab80a72afad59554330adc6d56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:4.4.4-windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:13cc45bcbe04fd9d2f1acea62d4bc57a1a533cae59c01cfcc74bff9aa5f2a501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.4.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:1fdc0fd04f4c1006a41c81066521c8d396a4fe9cbbb7d8df99dfba9ba670bfe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:424cadd696e9a0dbc691a4e2680722f2a9e8ab604374b482e2a9890fdc8ab0c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175093468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03be0dc25f8732caef29f051c91ce7447f8305738032e91c23b13cba3e74e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:03:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 12:03:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:03:30 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:03:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 12:03:32 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:05:11 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:05:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:05:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:05:13 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:05:13 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:05:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8c3715616e84c33c0038ba795484161fd38d0930d82e09b68283a1a18f451`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac42b84e850eda3c7655d1937d8a023de9fa68199e383acb2262d323442219d`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724cb122c25fe9272d20cdf76c45c6aab3f447f4e6f3b0ebfdfbb46724eb2ef`  
		Last Modified: Fri, 26 Mar 2021 12:08:02 GMT  
		Size: 139.6 MB (139567497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe10b8b0c12777d4c337f611abaf127960fab70650c1f7ad27073ac9bd2521`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e025c87f29ce34b87590b9f4dcc0b3b164ddba3bb903fcb1b9e0b91b0c7a7b`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:18b9ba93b6208cd80e1a723a241269f6e1eb44bfaa6ce1dd3de9be32f717daf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167536780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58929ecfa3caf151a12d97acb343f9b94bd867df524c3cdc9f60a00f46df5496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:27:42 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 14:27:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:27:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:27:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:50 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 14:27:51 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 14:27:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:28:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:28:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:28:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:28:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:28:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:28:46 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:28:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada24af95b05b298538ab63d883be491085362960192889c5c5d07627dfc446`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877762b7148d23f4cef028d66cb3f7ab51c8fb232f674d8cb2ce546675f0803`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a783117ad78ea48199bae4e86a245b13ae202fd98202cc2d5cd9df8bb0564432`  
		Last Modified: Fri, 26 Mar 2021 14:30:33 GMT  
		Size: 135.8 MB (135778542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc369a412303d9bc7d67b498032752b974cc1cf3a1854beba31c5b7705ca819`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ff00ed0d4b2c1c9040bac960068c8cf865ddf3b3417b0b4bfa0372df05ba06`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:cbb067bdf193c627f85874531f3d5c0b692d81db482a9c0c69d026a81383afe5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169136167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651556f82f603bac974f5788631fd43b058c3c818c1c6a96cf2e2dc5c2a0a289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:31 GMT
ADD file:1c7dbc64158234b813a2eeff0c325efa0cff7c3983e93fc9f7de0004e901c2c1 in / 
# Thu, 25 Mar 2021 22:53:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:35 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 08:57:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 08:57:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:57:20 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 08:57:21 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 08:57:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 08:57:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 08:57:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 08:57:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 08:57:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 08:57:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 08:57:41 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 08:57:42 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 08:58:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 08:58:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 08:58:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 08:58:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 08:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:58:33 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 08:58:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:bf8da0ed3f9ec60019cec9fac782f04b7281f232a86e7613579e54c348b8402b`  
		Last Modified: Thu, 25 Mar 2021 22:54:27 GMT  
		Size: 25.4 MB (25381419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de72c87d1d7a4355d21e04b9ce611f427f0c84ee6705dd53a1fd990012cefdd6`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffe2f5d8eac8afe4b79981c9c93b44c985dbb7b3bb5f9af5e918c6aac415fcf`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2808460e51d63b807cb6cb00bf034b7f2643599362ad55d9df26c6bc9ffad42c`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400c3133d141345611000d1de01cfadc8b8a785e209b80afcafa9214669ffd8f`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 2.7 MB (2708345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cdf5b66f6831b7db4ee570b487453c025248b2607e441c34db29488fcc35d4`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 5.7 MB (5747339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0de8bd807c307aaa480d335670e64efb51855df37c491f9e888d1848637001`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d58b3f14f22d07c415679c463eb1f4af10f1cbf89aa20fb46aaf3e31a41c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eef524d85fb192432f8eb7fc575cef6576292d4d47939a2b3650fd72dba5c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34edb6160fb71ce9809aec003c97570df6d05e2b19a1eb3ec267806ba9586f1`  
		Last Modified: Fri, 26 Mar 2021 08:59:21 GMT  
		Size: 135.3 MB (135289747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa65663451ec46890ca56252fcc498672e68e9b5dfa0df327c68150aa50226`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8215528e5cd8c0cb268785c0f8d75cfeb8ac2b40dd7f267effa9793d6fb487c5`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:75a5f624bd6d14254e0d84c2833f576109672750aaf2bf01d61cb5ead44f4505
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:424cadd696e9a0dbc691a4e2680722f2a9e8ab604374b482e2a9890fdc8ab0c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175093468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f03be0dc25f8732caef29f051c91ce7447f8305738032e91c23b13cba3e74e40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:32:58 GMT
ADD file:e80ae8d359b484dac5346f98c549abc694e1d0c87e1d9753d495aed4d9c8b2b3 in / 
# Thu, 25 Mar 2021 22:32:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:33:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:02 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 12:02:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 12:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:02:25 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 12:02:25 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 12:02:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 12:02:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 12:03:29 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 12:03:30 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 12:03:30 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 12:03:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 12:03:31 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 12:03:32 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 12:05:11 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 12:05:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 12:05:13 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 12:05:13 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 12:05:13 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 12:05:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6e0aa5e7af40303f56126b1469d1f37525b3a55a788836a6c9b773f6ce8bc446`  
		Last Modified: Thu, 25 Mar 2021 22:34:24 GMT  
		Size: 26.7 MB (26710781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47239a868b3375462d644f2ffb1b20114623fac03109d2950bdf0d57ab487d2`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49cbb10cca8504e3dbd65eb5db3c1dd0cd27070154386f819c5936de321c14b1`  
		Last Modified: Thu, 25 Mar 2021 22:34:20 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9729d7ec22de54c7a9e2dd0391cb2b89e18c79a964aa7fa571f0295e0a46ea5d`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fd72268d8a3e431bcc0cf92d6c24830fdc145c8d5d066a8867bcc9857f33f`  
		Last Modified: Fri, 26 Mar 2021 12:07:10 GMT  
		Size: 3.0 MB (2977455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2934dacaf58b563f07d40773619b4b95bec260e84b0a7e74575b55609fe160`  
		Last Modified: Fri, 26 Mar 2021 12:07:13 GMT  
		Size: 5.8 MB (5828414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9da24d4b2c3a01b52968f172a3c7930a2f33d3035046e3b974643b1502587e`  
		Last Modified: Fri, 26 Mar 2021 12:07:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8c3715616e84c33c0038ba795484161fd38d0930d82e09b68283a1a18f451`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac42b84e850eda3c7655d1937d8a023de9fa68199e383acb2262d323442219d`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724cb122c25fe9272d20cdf76c45c6aab3f447f4e6f3b0ebfdfbb46724eb2ef`  
		Last Modified: Fri, 26 Mar 2021 12:08:02 GMT  
		Size: 139.6 MB (139567497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fe10b8b0c12777d4c337f611abaf127960fab70650c1f7ad27073ac9bd2521`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e025c87f29ce34b87590b9f4dcc0b3b164ddba3bb903fcb1b9e0b91b0c7a7b`  
		Last Modified: Fri, 26 Mar 2021 12:07:38 GMT  
		Size: 4.4 KB (4422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:18b9ba93b6208cd80e1a723a241269f6e1eb44bfaa6ce1dd3de9be32f717daf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167536780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58929ecfa3caf151a12d97acb343f9b94bd867df524c3cdc9f60a00f46df5496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 23:21:42 GMT
ADD file:c2ebeb57ae78696b3c16020bf2c3030d8f36acd3032907fea3fec885ac614541 in / 
# Thu, 25 Mar 2021 23:21:47 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 23:21:57 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 23:22:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 23:22:07 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 14:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 14:25:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 14:25:57 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 14:25:58 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 14:26:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 14:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 14:27:42 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 14:27:45 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 14:27:46 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 14:27:47 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:48 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 14:27:50 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 14:27:51 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 14:27:53 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 14:28:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 14:28:38 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 14:28:40 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 14:28:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 14:28:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 14:28:46 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 14:28:47 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:af9ca2923c1e73640f6df497fc7fc63e3c2e24892f1d6abbd4225542339b6e06`  
		Last Modified: Thu, 25 Mar 2021 23:27:04 GMT  
		Size: 23.7 MB (23732791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2babfbd9d095d8a0dc7cfbaa658447a483120087d4ea77cae9ee9a78e370c2`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83b7f31d752fef6bce03359dc68487e2d02040b70c57526b72004a0ced4cbf5`  
		Last Modified: Thu, 25 Mar 2021 23:26:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d65028a76f2b15aa23f515778e097ec60c50a7f1f6f4b2a18b05eb6d9d46a4`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e52e6ccfbdddb05fb0a2557c65495579ff4280f5cfff2ae9384df791faf8e9`  
		Last Modified: Fri, 26 Mar 2021 14:29:30 GMT  
		Size: 2.7 MB (2668994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f39204b48d626ef1add7a61949ba35330339e5e079fc98d3c9c1231a7a603`  
		Last Modified: Fri, 26 Mar 2021 14:29:31 GMT  
		Size: 5.3 MB (5347127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e3812814ad24516e84a498b28d7b54d530f1dbb2be5f5778c3776aeb213b10`  
		Last Modified: Fri, 26 Mar 2021 14:29:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada24af95b05b298538ab63d883be491085362960192889c5c5d07627dfc446`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c877762b7148d23f4cef028d66cb3f7ab51c8fb232f674d8cb2ce546675f0803`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a783117ad78ea48199bae4e86a245b13ae202fd98202cc2d5cd9df8bb0564432`  
		Last Modified: Fri, 26 Mar 2021 14:30:33 GMT  
		Size: 135.8 MB (135778542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc369a412303d9bc7d67b498032752b974cc1cf3a1854beba31c5b7705ca819`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ff00ed0d4b2c1c9040bac960068c8cf865ddf3b3417b0b4bfa0372df05ba06`  
		Last Modified: Fri, 26 Mar 2021 14:30:06 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:cbb067bdf193c627f85874531f3d5c0b692d81db482a9c0c69d026a81383afe5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169136167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:651556f82f603bac974f5788631fd43b058c3c818c1c6a96cf2e2dc5c2a0a289`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 25 Mar 2021 22:53:31 GMT
ADD file:1c7dbc64158234b813a2eeff0c325efa0cff7c3983e93fc9f7de0004e901c2c1 in / 
# Thu, 25 Mar 2021 22:53:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:53:34 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 25 Mar 2021 22:53:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:53:35 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 08:57:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 26 Mar 2021 08:57:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:57:20 GMT
ENV GOSU_VERSION=1.12
# Fri, 26 Mar 2021 08:57:21 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 26 Mar 2021 08:57:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 26 Mar 2021 08:57:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 26 Mar 2021 08:57:38 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Fri, 26 Mar 2021 08:57:39 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Fri, 26 Mar 2021 08:57:39 GMT
ARG MONGO_PACKAGE=mongodb-org
# Fri, 26 Mar 2021 08:57:40 GMT
ARG MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Fri, 26 Mar 2021 08:57:40 GMT
ENV MONGO_MAJOR=4.4
# Fri, 26 Mar 2021 08:57:41 GMT
ENV MONGO_VERSION=4.4.4
# Fri, 26 Mar 2021 08:57:42 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 26 Mar 2021 08:58:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 26 Mar 2021 08:58:31 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 26 Mar 2021 08:58:31 GMT
VOLUME [/data/db /data/configdb]
# Fri, 26 Mar 2021 08:58:32 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Fri, 26 Mar 2021 08:58:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 08:58:33 GMT
EXPOSE 27017
# Fri, 26 Mar 2021 08:58:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:bf8da0ed3f9ec60019cec9fac782f04b7281f232a86e7613579e54c348b8402b`  
		Last Modified: Thu, 25 Mar 2021 22:54:27 GMT  
		Size: 25.4 MB (25381419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de72c87d1d7a4355d21e04b9ce611f427f0c84ee6705dd53a1fd990012cefdd6`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffe2f5d8eac8afe4b79981c9c93b44c985dbb7b3bb5f9af5e918c6aac415fcf`  
		Last Modified: Thu, 25 Mar 2021 22:54:24 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2808460e51d63b807cb6cb00bf034b7f2643599362ad55d9df26c6bc9ffad42c`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 1.9 KB (1878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:400c3133d141345611000d1de01cfadc8b8a785e209b80afcafa9214669ffd8f`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 2.7 MB (2708345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cdf5b66f6831b7db4ee570b487453c025248b2607e441c34db29488fcc35d4`  
		Last Modified: Fri, 26 Mar 2021 08:59:06 GMT  
		Size: 5.7 MB (5747339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0de8bd807c307aaa480d335670e64efb51855df37c491f9e888d1848637001`  
		Last Modified: Fri, 26 Mar 2021 08:59:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550d58b3f14f22d07c415679c463eb1f4af10f1cbf89aa20fb46aaf3e31a41c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57eef524d85fb192432f8eb7fc575cef6576292d4d47939a2b3650fd72dba5c0`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34edb6160fb71ce9809aec003c97570df6d05e2b19a1eb3ec267806ba9586f1`  
		Last Modified: Fri, 26 Mar 2021 08:59:21 GMT  
		Size: 135.3 MB (135289747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fa65663451ec46890ca56252fcc498672e68e9b5dfa0df327c68150aa50226`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8215528e5cd8c0cb268785c0f8d75cfeb8ac2b40dd7f267effa9793d6fb487c5`  
		Last Modified: Fri, 26 Mar 2021 08:59:03 GMT  
		Size: 4.4 KB (4425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:015fbab5dc985d5281b38ea374ec95fe55adddab9f883b59e8b37c7c61090cba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:windowsservercore` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:60acbac1cd7c075dc499da7ed7b6a9176c62fbab80a72afad59554330adc6d56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull mongo@sha256:8ff442e9b1680555fc89ad282175a007ac027109a8c3ee9d431696743fdde8fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2701828848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5090ab9db7afa2ad4d8701fb3859432ac61c350662f2f4206222bc55705adc6c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 14:15:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:14:25 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:14:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:14:27 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:16:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:16:36 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:16:37 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:16:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31ae1fcdffac4071930a0d98172fc515a43c93aa55870e4b6cc8c789b9444e73`  
		Last Modified: Wed, 10 Mar 2021 16:22:41 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311d0df16d36b3937d46be181e0a229cceb0adf48f12ed8e53bd85c7a2a173ec`  
		Last Modified: Wed, 10 Mar 2021 22:36:31 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9df5472ada4ede6abc048d047d07402cdef3880c0a532a56db49e92e3dfb60a`  
		Last Modified: Wed, 10 Mar 2021 22:36:32 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136798993baa7d19b266d06b0ec0e0691468400523e93fecfcd76edbff64a13d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ff73655b2823ee2b72110b5863c2a1b2fd8df0f8a4e66bbf59f7eb5ec22250`  
		Last Modified: Wed, 10 Mar 2021 22:37:15 GMT  
		Size: 240.3 MB (240284525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7697d7471e9a52cde26dcb966d286ade2d3447c1f2f20f0cd9a62c1ed0b42d28`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8f8e4802c75722cf888728d6862a04c1fdb24670b0fb6203154bf5589216fb`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2e5b172c45cdd07b520a7d3a55c5b2c4daec86846fbf5de3d5e0bd3e8d729d`  
		Last Modified: Wed, 10 Mar 2021 22:36:29 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:13cc45bcbe04fd9d2f1acea62d4bc57a1a533cae59c01cfcc74bff9aa5f2a501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull mongo@sha256:c37685976ea2150a613da628894c276826cd170429d3a9f085d7bcc7cad021b6
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6037919826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4024031ac3a3c33ab049be74022c086ae002d1b40782fe58eb8c7262fb4e77a2`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 14:25:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Mar 2021 22:16:53 GMT
ENV MONGO_VERSION=4.4.4
# Wed, 10 Mar 2021 22:16:55 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.4-signed.msi
# Wed, 10 Mar 2021 22:16:56 GMT
ENV MONGO_DOWNLOAD_SHA256=170eda3fb648ade8350a5bb0f1ffa367d81b020ea18e6e9e28107a77fff0d340
# Wed, 10 Mar 2021 22:19:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 10 Mar 2021 22:19:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 10 Mar 2021 22:19:55 GMT
EXPOSE 27017
# Wed, 10 Mar 2021 22:19:56 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5205e01a19ce3835a7f1caba14b71dbbcae05a77274c60358d9794ee0e2a3e65`  
		Last Modified: Wed, 10 Mar 2021 16:23:35 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf03de58aa28b3545afaa0768e22fde41055e2780b453f856d93e4329443b25`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797e54b97def836889ee59750bd5169cd506550b41ac8dd8dcb275824aa3f951`  
		Last Modified: Wed, 10 Mar 2021 22:37:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2422f8445181a8688b959da797d4a368623600db2562385e755f00256e977a37`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15bc7d40b91f58b075ce4e734c26574a9ef530450a3e6f3186ca66bf171f39`  
		Last Modified: Wed, 10 Mar 2021 22:42:15 GMT  
		Size: 241.0 MB (240999116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9638de9d0099fc8db8fba27d6ac12ee3935edfc323ef0beff5808d5881c13110`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800180d8958f84cb49668aaeeda8e9ff2a74f1a4dc42aea84e8637ca54f5e213`  
		Last Modified: Wed, 10 Mar 2021 22:37:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02fa96a1dc62df59d84a0ea8ed52f520fbef98d92a3c3be93d89cf0507fc938`  
		Last Modified: Wed, 10 Mar 2021 22:37:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
