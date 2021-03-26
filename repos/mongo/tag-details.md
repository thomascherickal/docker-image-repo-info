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
$ docker pull mongo@sha256:36aaa3ec53b724f227bd47cbb924bb2d9c0554a5c317b62c1655148572162f09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:94283bb145f9791519b682a58eb2248df0a556b3feb73f6a530124f7c1fd5b77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a0031d25b85ff42832fc287e3370643e3e1166cf089082e2f650132612d0d4`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:24:40 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 22 Mar 2021 19:24:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:24:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:24:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_MAJOR=3.6
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:24:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:24:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:00 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:00 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:00 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:00 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:01 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f13f032c38120d6518aa402559f943a6d01eb639315d9a614295eb67cd73dd`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb12d006b934ee9f8a031bc0325e945d2f7cfd239bc70a020af743b1c9c9a6`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d0465a2b970cb7064a3e4aeffcf968b4180fca96e9dd661da1d0981c01e429`  
		Last Modified: Mon, 22 Mar 2021 19:28:21 GMT  
		Size: 119.4 MB (119407969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160e471aa05812a6cc1fa764748cfe73499b3ecf27c77c635987b8dcfb9ed8a`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28d3bfc6f02ffb3c2db2053ae8ecb04fa89137dff3711779bdcdac551475a1d`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:01717d16c9725a25f61bba4c0aa3a6ca1d672d352f9de5cc4844a2525fc71b10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:94283bb145f9791519b682a58eb2248df0a556b3feb73f6a530124f7c1fd5b77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a0031d25b85ff42832fc287e3370643e3e1166cf089082e2f650132612d0d4`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:24:40 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 22 Mar 2021 19:24:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:24:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:24:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_MAJOR=3.6
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:24:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:24:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:00 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:00 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:00 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:00 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:01 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f13f032c38120d6518aa402559f943a6d01eb639315d9a614295eb67cd73dd`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb12d006b934ee9f8a031bc0325e945d2f7cfd239bc70a020af743b1c9c9a6`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d0465a2b970cb7064a3e4aeffcf968b4180fca96e9dd661da1d0981c01e429`  
		Last Modified: Mon, 22 Mar 2021 19:28:21 GMT  
		Size: 119.4 MB (119407969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160e471aa05812a6cc1fa764748cfe73499b3ecf27c77c635987b8dcfb9ed8a`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28d3bfc6f02ffb3c2db2053ae8ecb04fa89137dff3711779bdcdac551475a1d`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:36aaa3ec53b724f227bd47cbb924bb2d9c0554a5c317b62c1655148572162f09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:94283bb145f9791519b682a58eb2248df0a556b3feb73f6a530124f7c1fd5b77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a0031d25b85ff42832fc287e3370643e3e1166cf089082e2f650132612d0d4`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:24:40 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 22 Mar 2021 19:24:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:24:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:24:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_MAJOR=3.6
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:24:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:24:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:00 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:00 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:00 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:00 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:01 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f13f032c38120d6518aa402559f943a6d01eb639315d9a614295eb67cd73dd`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb12d006b934ee9f8a031bc0325e945d2f7cfd239bc70a020af743b1c9c9a6`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d0465a2b970cb7064a3e4aeffcf968b4180fca96e9dd661da1d0981c01e429`  
		Last Modified: Mon, 22 Mar 2021 19:28:21 GMT  
		Size: 119.4 MB (119407969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160e471aa05812a6cc1fa764748cfe73499b3ecf27c77c635987b8dcfb9ed8a`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28d3bfc6f02ffb3c2db2053ae8ecb04fa89137dff3711779bdcdac551475a1d`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:01717d16c9725a25f61bba4c0aa3a6ca1d672d352f9de5cc4844a2525fc71b10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:94283bb145f9791519b682a58eb2248df0a556b3feb73f6a530124f7c1fd5b77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a0031d25b85ff42832fc287e3370643e3e1166cf089082e2f650132612d0d4`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:24:40 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 22 Mar 2021 19:24:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:24:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:24:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_MAJOR=3.6
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:24:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:24:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:00 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:00 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:00 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:00 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:01 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f13f032c38120d6518aa402559f943a6d01eb639315d9a614295eb67cd73dd`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb12d006b934ee9f8a031bc0325e945d2f7cfd239bc70a020af743b1c9c9a6`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d0465a2b970cb7064a3e4aeffcf968b4180fca96e9dd661da1d0981c01e429`  
		Last Modified: Mon, 22 Mar 2021 19:28:21 GMT  
		Size: 119.4 MB (119407969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160e471aa05812a6cc1fa764748cfe73499b3ecf27c77c635987b8dcfb9ed8a`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28d3bfc6f02ffb3c2db2053ae8ecb04fa89137dff3711779bdcdac551475a1d`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:36aaa3ec53b724f227bd47cbb924bb2d9c0554a5c317b62c1655148572162f09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:3.6.23` - linux; amd64

```console
$ docker pull mongo@sha256:94283bb145f9791519b682a58eb2248df0a556b3feb73f6a530124f7c1fd5b77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a0031d25b85ff42832fc287e3370643e3e1166cf089082e2f650132612d0d4`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:24:40 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 22 Mar 2021 19:24:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:24:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:24:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_MAJOR=3.6
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:24:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:24:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:00 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:00 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:00 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:00 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:01 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f13f032c38120d6518aa402559f943a6d01eb639315d9a614295eb67cd73dd`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb12d006b934ee9f8a031bc0325e945d2f7cfd239bc70a020af743b1c9c9a6`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d0465a2b970cb7064a3e4aeffcf968b4180fca96e9dd661da1d0981c01e429`  
		Last Modified: Mon, 22 Mar 2021 19:28:21 GMT  
		Size: 119.4 MB (119407969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160e471aa05812a6cc1fa764748cfe73499b3ecf27c77c635987b8dcfb9ed8a`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28d3bfc6f02ffb3c2db2053ae8ecb04fa89137dff3711779bdcdac551475a1d`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:01717d16c9725a25f61bba4c0aa3a6ca1d672d352f9de5cc4844a2525fc71b10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.23-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:94283bb145f9791519b682a58eb2248df0a556b3feb73f6a530124f7c1fd5b77
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169593030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a0031d25b85ff42832fc287e3370643e3e1166cf089082e2f650132612d0d4`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:24:40 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Mon, 22 Mar 2021 19:24:41 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:24:41 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:24:42 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_MAJOR=3.6
# Mon, 22 Mar 2021 19:24:42 GMT
ENV MONGO_VERSION=3.6.23
# Mon, 22 Mar 2021 19:24:43 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:24:58 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:00 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:00 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:00 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:00 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:01 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f13f032c38120d6518aa402559f943a6d01eb639315d9a614295eb67cd73dd`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65eb12d006b934ee9f8a031bc0325e945d2f7cfd239bc70a020af743b1c9c9a6`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d0465a2b970cb7064a3e4aeffcf968b4180fca96e9dd661da1d0981c01e429`  
		Last Modified: Mon, 22 Mar 2021 19:28:21 GMT  
		Size: 119.4 MB (119407969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6160e471aa05812a6cc1fa764748cfe73499b3ecf27c77c635987b8dcfb9ed8a`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28d3bfc6f02ffb3c2db2053ae8ecb04fa89137dff3711779bdcdac551475a1d`  
		Last Modified: Mon, 22 Mar 2021 19:28:04 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:a0943cd354ccf6b98ff598b783c50a73fb36c160be958a85c1373443ddcfec0e
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
$ docker pull mongo@sha256:5a1c46c78bac63be123bff52d38c2d10a02153af42c511c952c4af8dbb0a14c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175096021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85055945985ff6073cd1c27f52ab7da65bfd72af9af4c5bd2c94875a85044f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:27:13 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Mon, 22 Mar 2021 19:27:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:27:14 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:27:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_MAJOR=4.4
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_VERSION=4.4.4
# Mon, 22 Mar 2021 19:27:16 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:27:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:27:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:27:35 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:27:35 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:27:36 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81a8b8de1c04784d6d1e72f48119a95f94d72b8ae5f960d2b4097c232ba606`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782487be328415ddb46d726867068844c1fae6e9e4bcfcbcf6d6b7d2815deae4`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2092e9a3c4a7ad8deed4f6fe99dfaa6bc99a05748a35d9aff3b566f0aed48153`  
		Last Modified: Mon, 22 Mar 2021 19:29:59 GMT  
		Size: 139.6 MB (139568674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487d84247ee7669555e838408e05c3dabfeaa86ac1026553b49f95d33046914`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad1ed2c45ef912c44033b2049bb21d7602a2631666a1a00ea34a72385212358`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f56f614825f3f91b317f3db0564741146070246d5be546bd1e38cbc37c8cae4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167499715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3baaccfe9bec5aa2412a52b36fc411679e2c769501bc05b5bdf7d71d96125c9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:35:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 04:35:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 04:35:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 04:35:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 04:35:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 04:35:41 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 04:35:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 04:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 04:35:43 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 04:35:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823e0c350f02b4f697b67327987e02f972cd52cf2ea0f96f2cc3746ea0b50a44`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120da36ea9c1eed89a75905bed5f647c197c478a1db43e5a3a00f378e650a906`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2b71f7401e15f285d2758653f2d7b386770dfd75cd3e47d8833b80866c570f`  
		Last Modified: Thu, 04 Mar 2021 04:37:16 GMT  
		Size: 135.7 MB (135742521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12473a22009e488412a3ccfc540781b09b32758dacec9d6eaa8593364e4c20b2`  
		Last Modified: Thu, 04 Mar 2021 04:36:47 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52361ab241ff118e8095349be7438caaa778c9bc6d244532be2e5442b83c589`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:6a8ce34e89e708d16e4b381a922c1d16ecf06d2383c39fbadb735f7d3b00c855
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:5a1c46c78bac63be123bff52d38c2d10a02153af42c511c952c4af8dbb0a14c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175096021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85055945985ff6073cd1c27f52ab7da65bfd72af9af4c5bd2c94875a85044f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:27:13 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Mon, 22 Mar 2021 19:27:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:27:14 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:27:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_MAJOR=4.4
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_VERSION=4.4.4
# Mon, 22 Mar 2021 19:27:16 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:27:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:27:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:27:35 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:27:35 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:27:36 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81a8b8de1c04784d6d1e72f48119a95f94d72b8ae5f960d2b4097c232ba606`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782487be328415ddb46d726867068844c1fae6e9e4bcfcbcf6d6b7d2815deae4`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2092e9a3c4a7ad8deed4f6fe99dfaa6bc99a05748a35d9aff3b566f0aed48153`  
		Last Modified: Mon, 22 Mar 2021 19:29:59 GMT  
		Size: 139.6 MB (139568674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487d84247ee7669555e838408e05c3dabfeaa86ac1026553b49f95d33046914`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad1ed2c45ef912c44033b2049bb21d7602a2631666a1a00ea34a72385212358`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f56f614825f3f91b317f3db0564741146070246d5be546bd1e38cbc37c8cae4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167499715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3baaccfe9bec5aa2412a52b36fc411679e2c769501bc05b5bdf7d71d96125c9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:35:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 04:35:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 04:35:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 04:35:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 04:35:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 04:35:41 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 04:35:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 04:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 04:35:43 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 04:35:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823e0c350f02b4f697b67327987e02f972cd52cf2ea0f96f2cc3746ea0b50a44`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120da36ea9c1eed89a75905bed5f647c197c478a1db43e5a3a00f378e650a906`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2b71f7401e15f285d2758653f2d7b386770dfd75cd3e47d8833b80866c570f`  
		Last Modified: Thu, 04 Mar 2021 04:37:16 GMT  
		Size: 135.7 MB (135742521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12473a22009e488412a3ccfc540781b09b32758dacec9d6eaa8593364e4c20b2`  
		Last Modified: Thu, 04 Mar 2021 04:36:47 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52361ab241ff118e8095349be7438caaa778c9bc6d244532be2e5442b83c589`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:cedc456e62d1fe1f909c08d993326219cef0656ec8e7770a8ff6462c9e21576e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:19aa64336ca3f33361923be024f05053762b7aec90364eba7679b49b005fdd48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156130272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb94735a5cbe30602d8eca47be02851f779a1db2a6e7f255d4afb79e2109fef`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:25:14 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Mon, 22 Mar 2021 19:25:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:25:15 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:25:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:25:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:25:16 GMT
ENV MONGO_MAJOR=4.0
# Mon, 22 Mar 2021 19:25:16 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Mar 2021 19:25:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:25:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:34 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:34 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:34 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:34 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af018cb3cc4d181322b8109134602e433f917c0161e459cf19f2bbc2a4856d47`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a8f95f9f58e0802d204f36dd62a639cbd6ab71e739e0bf7123e794d7bf09d`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9bcf435643489ff958a03ef96327ef871c7e4d238f6c3e568066edcfa8a002`  
		Last Modified: Mon, 22 Mar 2021 19:28:55 GMT  
		Size: 105.9 MB (105945780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773627d8b342410bd4565b4ebe3ee551d22942accefd1659bca32187f1955db`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689fb57376d390888b937811a6eff9d4d37421bba90672a6869907c2617437a1`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 4.4 KB (4422 bytes)  
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
$ docker pull mongo@sha256:295fcc88169fca23a134dcd2aaf73ade7c9366a62ef4568f5bd13a59b505510d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:19aa64336ca3f33361923be024f05053762b7aec90364eba7679b49b005fdd48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156130272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb94735a5cbe30602d8eca47be02851f779a1db2a6e7f255d4afb79e2109fef`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:25:14 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Mon, 22 Mar 2021 19:25:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:25:15 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:25:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:25:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:25:16 GMT
ENV MONGO_MAJOR=4.0
# Mon, 22 Mar 2021 19:25:16 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Mar 2021 19:25:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:25:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:34 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:34 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:34 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:34 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af018cb3cc4d181322b8109134602e433f917c0161e459cf19f2bbc2a4856d47`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a8f95f9f58e0802d204f36dd62a639cbd6ab71e739e0bf7123e794d7bf09d`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9bcf435643489ff958a03ef96327ef871c7e4d238f6c3e568066edcfa8a002`  
		Last Modified: Mon, 22 Mar 2021 19:28:55 GMT  
		Size: 105.9 MB (105945780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773627d8b342410bd4565b4ebe3ee551d22942accefd1659bca32187f1955db`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689fb57376d390888b937811a6eff9d4d37421bba90672a6869907c2617437a1`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 4.4 KB (4422 bytes)  
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
$ docker pull mongo@sha256:cedc456e62d1fe1f909c08d993326219cef0656ec8e7770a8ff6462c9e21576e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.0.23` - linux; amd64

```console
$ docker pull mongo@sha256:19aa64336ca3f33361923be024f05053762b7aec90364eba7679b49b005fdd48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156130272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb94735a5cbe30602d8eca47be02851f779a1db2a6e7f255d4afb79e2109fef`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:25:14 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Mon, 22 Mar 2021 19:25:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:25:15 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:25:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:25:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:25:16 GMT
ENV MONGO_MAJOR=4.0
# Mon, 22 Mar 2021 19:25:16 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Mar 2021 19:25:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:25:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:34 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:34 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:34 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:34 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af018cb3cc4d181322b8109134602e433f917c0161e459cf19f2bbc2a4856d47`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a8f95f9f58e0802d204f36dd62a639cbd6ab71e739e0bf7123e794d7bf09d`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9bcf435643489ff958a03ef96327ef871c7e4d238f6c3e568066edcfa8a002`  
		Last Modified: Mon, 22 Mar 2021 19:28:55 GMT  
		Size: 105.9 MB (105945780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773627d8b342410bd4565b4ebe3ee551d22942accefd1659bca32187f1955db`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689fb57376d390888b937811a6eff9d4d37421bba90672a6869907c2617437a1`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 4.4 KB (4422 bytes)  
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
$ docker pull mongo@sha256:295fcc88169fca23a134dcd2aaf73ade7c9366a62ef4568f5bd13a59b505510d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.23-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:19aa64336ca3f33361923be024f05053762b7aec90364eba7679b49b005fdd48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156130272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb94735a5cbe30602d8eca47be02851f779a1db2a6e7f255d4afb79e2109fef`
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
# Mon, 22 Mar 2021 19:23:49 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:24:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:24:10 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:24:10 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:24:39 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:24:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:25:14 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Mon, 22 Mar 2021 19:25:15 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:25:15 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:25:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:25:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:25:16 GMT
ENV MONGO_MAJOR=4.0
# Mon, 22 Mar 2021 19:25:16 GMT
ENV MONGO_VERSION=4.0.23
# Mon, 22 Mar 2021 19:25:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:25:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:25:34 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:25:34 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:25:34 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:25:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:25:34 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:25:34 GMT
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
	-	`sha256:18e1cb7b6ea5b8dc19152782b4f456c2ae89cb3e8e9db641900c99efcdac8bc1`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 2.0 KB (1988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88627ab2894ac222e6a29fc9c51e0202853983383a92fd1c7d512245b9fc533`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 2.9 MB (2906662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c40556fa992da6145f6b5b941db23950107228991c0f548c42fb5d77f91b45`  
		Last Modified: Mon, 22 Mar 2021 19:28:07 GMT  
		Size: 1.3 MB (1305538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d61aed3bb35b2b335e679bbeea8435b6aff0152cc9a657e40b73cf46b05b0b`  
		Last Modified: Mon, 22 Mar 2021 19:28:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af018cb3cc4d181322b8109134602e433f917c0161e459cf19f2bbc2a4856d47`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a8f95f9f58e0802d204f36dd62a639cbd6ab71e739e0bf7123e794d7bf09d`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9bcf435643489ff958a03ef96327ef871c7e4d238f6c3e568066edcfa8a002`  
		Last Modified: Mon, 22 Mar 2021 19:28:55 GMT  
		Size: 105.9 MB (105945780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c773627d8b342410bd4565b4ebe3ee551d22942accefd1659bca32187f1955db`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689fb57376d390888b937811a6eff9d4d37421bba90672a6869907c2617437a1`  
		Last Modified: Mon, 22 Mar 2021 19:28:40 GMT  
		Size: 4.4 KB (4422 bytes)  
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
$ docker pull mongo@sha256:fe6e844dd03bb1ec9d5dd71f5f450a7a79a1c54412a087d4522e40eb5b682b38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:e74b2dc8dacd0e135fccd958422d6ba6aa9ca6cd8882b128674919f4a109ef2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165341250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bde40678bdd380a5252b895a3d8d08715ffab630dabe2986a428f7a6bf2f9e03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:26:31 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 22 Mar 2021 19:26:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:26:32 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:26:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:26:32 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:26:33 GMT
ENV MONGO_MAJOR=4.2
# Mon, 22 Mar 2021 19:26:33 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:26:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:26:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:26:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:26:57 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:26:57 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:26:57 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:26:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e4d68a0e6c65998c4b505ac1bde7f13f9d43af06dc4393e19a1cccad46435a`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2447cb986170ed91f5c9ef1b84e31945393b032ed8f4310a49a61ee253dc090`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d787c416e2a892b640886046243180ee2c735cb4b5ca664ddf0c7e8f026d9`  
		Last Modified: Mon, 22 Mar 2021 19:29:24 GMT  
		Size: 129.8 MB (129813907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927065caf369ca7a2148dd4f6c9bef8acdc6e2fdd34718f1e63f08633f2c5d60`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c4d592a806db6c1a5353926cdcbf1c5b6624bc1faa27e484b8c474da55ded5`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dba45579517ec71cf5e8d5718cf8b90aeec6aaf1cc120268130ae84624b1a1a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155377851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6fe0d16d8063552d90fb711c51bac1a711cd2db607093fa48064c1b9f83d77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:34:04 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 04 Mar 2021 04:34:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:34:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:34:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:34:09 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:34:10 GMT
ENV MONGO_MAJOR=4.2
# Mon, 22 Mar 2021 19:41:20 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:41:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:49 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:53 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:54 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:54 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:56 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6967ff7398fec6e3a94eee908479fe4752e28e300e6d68e1e7424c47d5d384a1`  
		Last Modified: Thu, 04 Mar 2021 04:36:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c970293bc12fe0e8bf004aa47d8a9168d8a8b11106044c3b83c6e1ab53392df`  
		Last Modified: Mon, 22 Mar 2021 19:43:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73c0665cadb202c43ac9e1bf63dcdbcf72b346350dfae490ec05f41d19957c`  
		Last Modified: Mon, 22 Mar 2021 19:43:35 GMT  
		Size: 123.6 MB (123620652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc9863cf29800c65da240551a6afbdb34569c05910618b13993db77bf74dc33`  
		Last Modified: Mon, 22 Mar 2021 19:43:10 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430e0aa5b9e93b6cd1eed3769211d4caeb9f679bb0860381524c23ada2b61095`  
		Last Modified: Mon, 22 Mar 2021 19:43:09 GMT  
		Size: 4.4 KB (4423 bytes)  
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
$ docker pull mongo@sha256:153982c2a695d4a4dcc62f399193dd8cae3a027614e7d8d8096f12dc2538961a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:e74b2dc8dacd0e135fccd958422d6ba6aa9ca6cd8882b128674919f4a109ef2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165341250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bde40678bdd380a5252b895a3d8d08715ffab630dabe2986a428f7a6bf2f9e03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:26:31 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 22 Mar 2021 19:26:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:26:32 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:26:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:26:32 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:26:33 GMT
ENV MONGO_MAJOR=4.2
# Mon, 22 Mar 2021 19:26:33 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:26:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:26:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:26:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:26:57 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:26:57 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:26:57 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:26:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e4d68a0e6c65998c4b505ac1bde7f13f9d43af06dc4393e19a1cccad46435a`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2447cb986170ed91f5c9ef1b84e31945393b032ed8f4310a49a61ee253dc090`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d787c416e2a892b640886046243180ee2c735cb4b5ca664ddf0c7e8f026d9`  
		Last Modified: Mon, 22 Mar 2021 19:29:24 GMT  
		Size: 129.8 MB (129813907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927065caf369ca7a2148dd4f6c9bef8acdc6e2fdd34718f1e63f08633f2c5d60`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c4d592a806db6c1a5353926cdcbf1c5b6624bc1faa27e484b8c474da55ded5`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dba45579517ec71cf5e8d5718cf8b90aeec6aaf1cc120268130ae84624b1a1a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155377851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6fe0d16d8063552d90fb711c51bac1a711cd2db607093fa48064c1b9f83d77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:34:04 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 04 Mar 2021 04:34:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:34:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:34:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:34:09 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:34:10 GMT
ENV MONGO_MAJOR=4.2
# Mon, 22 Mar 2021 19:41:20 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:41:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:49 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:53 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:54 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:54 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:56 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6967ff7398fec6e3a94eee908479fe4752e28e300e6d68e1e7424c47d5d384a1`  
		Last Modified: Thu, 04 Mar 2021 04:36:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c970293bc12fe0e8bf004aa47d8a9168d8a8b11106044c3b83c6e1ab53392df`  
		Last Modified: Mon, 22 Mar 2021 19:43:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73c0665cadb202c43ac9e1bf63dcdbcf72b346350dfae490ec05f41d19957c`  
		Last Modified: Mon, 22 Mar 2021 19:43:35 GMT  
		Size: 123.6 MB (123620652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc9863cf29800c65da240551a6afbdb34569c05910618b13993db77bf74dc33`  
		Last Modified: Mon, 22 Mar 2021 19:43:10 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430e0aa5b9e93b6cd1eed3769211d4caeb9f679bb0860381524c23ada2b61095`  
		Last Modified: Mon, 22 Mar 2021 19:43:09 GMT  
		Size: 4.4 KB (4423 bytes)  
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
$ docker pull mongo@sha256:fe6e844dd03bb1ec9d5dd71f5f450a7a79a1c54412a087d4522e40eb5b682b38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1817; amd64
	-	windows version 10.0.14393.4283; amd64

### `mongo:4.2.13` - linux; amd64

```console
$ docker pull mongo@sha256:e74b2dc8dacd0e135fccd958422d6ba6aa9ca6cd8882b128674919f4a109ef2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165341250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bde40678bdd380a5252b895a3d8d08715ffab630dabe2986a428f7a6bf2f9e03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:26:31 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 22 Mar 2021 19:26:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:26:32 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:26:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:26:32 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:26:33 GMT
ENV MONGO_MAJOR=4.2
# Mon, 22 Mar 2021 19:26:33 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:26:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:26:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:26:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:26:57 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:26:57 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:26:57 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:26:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e4d68a0e6c65998c4b505ac1bde7f13f9d43af06dc4393e19a1cccad46435a`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2447cb986170ed91f5c9ef1b84e31945393b032ed8f4310a49a61ee253dc090`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d787c416e2a892b640886046243180ee2c735cb4b5ca664ddf0c7e8f026d9`  
		Last Modified: Mon, 22 Mar 2021 19:29:24 GMT  
		Size: 129.8 MB (129813907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927065caf369ca7a2148dd4f6c9bef8acdc6e2fdd34718f1e63f08633f2c5d60`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c4d592a806db6c1a5353926cdcbf1c5b6624bc1faa27e484b8c474da55ded5`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.13` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dba45579517ec71cf5e8d5718cf8b90aeec6aaf1cc120268130ae84624b1a1a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155377851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6fe0d16d8063552d90fb711c51bac1a711cd2db607093fa48064c1b9f83d77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:34:04 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 04 Mar 2021 04:34:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:34:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:34:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:34:09 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:34:10 GMT
ENV MONGO_MAJOR=4.2
# Mon, 22 Mar 2021 19:41:20 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:41:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:49 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:53 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:54 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:54 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:56 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6967ff7398fec6e3a94eee908479fe4752e28e300e6d68e1e7424c47d5d384a1`  
		Last Modified: Thu, 04 Mar 2021 04:36:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c970293bc12fe0e8bf004aa47d8a9168d8a8b11106044c3b83c6e1ab53392df`  
		Last Modified: Mon, 22 Mar 2021 19:43:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73c0665cadb202c43ac9e1bf63dcdbcf72b346350dfae490ec05f41d19957c`  
		Last Modified: Mon, 22 Mar 2021 19:43:35 GMT  
		Size: 123.6 MB (123620652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc9863cf29800c65da240551a6afbdb34569c05910618b13993db77bf74dc33`  
		Last Modified: Mon, 22 Mar 2021 19:43:10 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430e0aa5b9e93b6cd1eed3769211d4caeb9f679bb0860381524c23ada2b61095`  
		Last Modified: Mon, 22 Mar 2021 19:43:09 GMT  
		Size: 4.4 KB (4423 bytes)  
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
$ docker pull mongo@sha256:153982c2a695d4a4dcc62f399193dd8cae3a027614e7d8d8096f12dc2538961a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2.13-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:e74b2dc8dacd0e135fccd958422d6ba6aa9ca6cd8882b128674919f4a109ef2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.3 MB (165341250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bde40678bdd380a5252b895a3d8d08715ffab630dabe2986a428f7a6bf2f9e03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:26:31 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Mon, 22 Mar 2021 19:26:32 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:26:32 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:26:32 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:26:32 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:26:33 GMT
ENV MONGO_MAJOR=4.2
# Mon, 22 Mar 2021 19:26:33 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:26:34 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:26:55 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:26:56 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:26:57 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:26:57 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:26:57 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:26:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e4d68a0e6c65998c4b505ac1bde7f13f9d43af06dc4393e19a1cccad46435a`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2447cb986170ed91f5c9ef1b84e31945393b032ed8f4310a49a61ee253dc090`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d787c416e2a892b640886046243180ee2c735cb4b5ca664ddf0c7e8f026d9`  
		Last Modified: Mon, 22 Mar 2021 19:29:24 GMT  
		Size: 129.8 MB (129813907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927065caf369ca7a2148dd4f6c9bef8acdc6e2fdd34718f1e63f08633f2c5d60`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c4d592a806db6c1a5353926cdcbf1c5b6624bc1faa27e484b8c474da55ded5`  
		Last Modified: Mon, 22 Mar 2021 19:29:07 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.13-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:dba45579517ec71cf5e8d5718cf8b90aeec6aaf1cc120268130ae84624b1a1a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.4 MB (155377851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea6fe0d16d8063552d90fb711c51bac1a711cd2db607093fa48064c1b9f83d77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:34:04 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 04 Mar 2021 04:34:07 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:34:07 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:34:08 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:34:09 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:34:10 GMT
ENV MONGO_MAJOR=4.2
# Mon, 22 Mar 2021 19:41:20 GMT
ENV MONGO_VERSION=4.2.13
# Mon, 22 Mar 2021 19:41:22 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:41:49 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:41:53 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:41:54 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:41:54 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:41:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:41:56 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:41:57 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6967ff7398fec6e3a94eee908479fe4752e28e300e6d68e1e7424c47d5d384a1`  
		Last Modified: Thu, 04 Mar 2021 04:36:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c970293bc12fe0e8bf004aa47d8a9168d8a8b11106044c3b83c6e1ab53392df`  
		Last Modified: Mon, 22 Mar 2021 19:43:09 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73c0665cadb202c43ac9e1bf63dcdbcf72b346350dfae490ec05f41d19957c`  
		Last Modified: Mon, 22 Mar 2021 19:43:35 GMT  
		Size: 123.6 MB (123620652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc9863cf29800c65da240551a6afbdb34569c05910618b13993db77bf74dc33`  
		Last Modified: Mon, 22 Mar 2021 19:43:10 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430e0aa5b9e93b6cd1eed3769211d4caeb9f679bb0860381524c23ada2b61095`  
		Last Modified: Mon, 22 Mar 2021 19:43:09 GMT  
		Size: 4.4 KB (4423 bytes)  
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
$ docker pull mongo@sha256:a0943cd354ccf6b98ff598b783c50a73fb36c160be958a85c1373443ddcfec0e
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
$ docker pull mongo@sha256:5a1c46c78bac63be123bff52d38c2d10a02153af42c511c952c4af8dbb0a14c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175096021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85055945985ff6073cd1c27f52ab7da65bfd72af9af4c5bd2c94875a85044f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:27:13 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Mon, 22 Mar 2021 19:27:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:27:14 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:27:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_MAJOR=4.4
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_VERSION=4.4.4
# Mon, 22 Mar 2021 19:27:16 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:27:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:27:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:27:35 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:27:35 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:27:36 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81a8b8de1c04784d6d1e72f48119a95f94d72b8ae5f960d2b4097c232ba606`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782487be328415ddb46d726867068844c1fae6e9e4bcfcbcf6d6b7d2815deae4`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2092e9a3c4a7ad8deed4f6fe99dfaa6bc99a05748a35d9aff3b566f0aed48153`  
		Last Modified: Mon, 22 Mar 2021 19:29:59 GMT  
		Size: 139.6 MB (139568674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487d84247ee7669555e838408e05c3dabfeaa86ac1026553b49f95d33046914`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad1ed2c45ef912c44033b2049bb21d7602a2631666a1a00ea34a72385212358`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f56f614825f3f91b317f3db0564741146070246d5be546bd1e38cbc37c8cae4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167499715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3baaccfe9bec5aa2412a52b36fc411679e2c769501bc05b5bdf7d71d96125c9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:35:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 04:35:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 04:35:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 04:35:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 04:35:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 04:35:41 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 04:35:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 04:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 04:35:43 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 04:35:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823e0c350f02b4f697b67327987e02f972cd52cf2ea0f96f2cc3746ea0b50a44`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120da36ea9c1eed89a75905bed5f647c197c478a1db43e5a3a00f378e650a906`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2b71f7401e15f285d2758653f2d7b386770dfd75cd3e47d8833b80866c570f`  
		Last Modified: Thu, 04 Mar 2021 04:37:16 GMT  
		Size: 135.7 MB (135742521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12473a22009e488412a3ccfc540781b09b32758dacec9d6eaa8593364e4c20b2`  
		Last Modified: Thu, 04 Mar 2021 04:36:47 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52361ab241ff118e8095349be7438caaa778c9bc6d244532be2e5442b83c589`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:6a8ce34e89e708d16e4b381a922c1d16ecf06d2383c39fbadb735f7d3b00c855
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:5a1c46c78bac63be123bff52d38c2d10a02153af42c511c952c4af8dbb0a14c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175096021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85055945985ff6073cd1c27f52ab7da65bfd72af9af4c5bd2c94875a85044f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:27:13 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Mon, 22 Mar 2021 19:27:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:27:14 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:27:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_MAJOR=4.4
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_VERSION=4.4.4
# Mon, 22 Mar 2021 19:27:16 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:27:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:27:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:27:35 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:27:35 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:27:36 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81a8b8de1c04784d6d1e72f48119a95f94d72b8ae5f960d2b4097c232ba606`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782487be328415ddb46d726867068844c1fae6e9e4bcfcbcf6d6b7d2815deae4`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2092e9a3c4a7ad8deed4f6fe99dfaa6bc99a05748a35d9aff3b566f0aed48153`  
		Last Modified: Mon, 22 Mar 2021 19:29:59 GMT  
		Size: 139.6 MB (139568674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487d84247ee7669555e838408e05c3dabfeaa86ac1026553b49f95d33046914`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad1ed2c45ef912c44033b2049bb21d7602a2631666a1a00ea34a72385212358`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f56f614825f3f91b317f3db0564741146070246d5be546bd1e38cbc37c8cae4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167499715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3baaccfe9bec5aa2412a52b36fc411679e2c769501bc05b5bdf7d71d96125c9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:35:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 04:35:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 04:35:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 04:35:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 04:35:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 04:35:41 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 04:35:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 04:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 04:35:43 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 04:35:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823e0c350f02b4f697b67327987e02f972cd52cf2ea0f96f2cc3746ea0b50a44`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120da36ea9c1eed89a75905bed5f647c197c478a1db43e5a3a00f378e650a906`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2b71f7401e15f285d2758653f2d7b386770dfd75cd3e47d8833b80866c570f`  
		Last Modified: Thu, 04 Mar 2021 04:37:16 GMT  
		Size: 135.7 MB (135742521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12473a22009e488412a3ccfc540781b09b32758dacec9d6eaa8593364e4c20b2`  
		Last Modified: Thu, 04 Mar 2021 04:36:47 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52361ab241ff118e8095349be7438caaa778c9bc6d244532be2e5442b83c589`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:a0943cd354ccf6b98ff598b783c50a73fb36c160be958a85c1373443ddcfec0e
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
$ docker pull mongo@sha256:5a1c46c78bac63be123bff52d38c2d10a02153af42c511c952c4af8dbb0a14c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175096021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85055945985ff6073cd1c27f52ab7da65bfd72af9af4c5bd2c94875a85044f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:27:13 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Mon, 22 Mar 2021 19:27:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:27:14 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:27:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_MAJOR=4.4
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_VERSION=4.4.4
# Mon, 22 Mar 2021 19:27:16 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:27:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:27:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:27:35 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:27:35 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:27:36 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81a8b8de1c04784d6d1e72f48119a95f94d72b8ae5f960d2b4097c232ba606`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782487be328415ddb46d726867068844c1fae6e9e4bcfcbcf6d6b7d2815deae4`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2092e9a3c4a7ad8deed4f6fe99dfaa6bc99a05748a35d9aff3b566f0aed48153`  
		Last Modified: Mon, 22 Mar 2021 19:29:59 GMT  
		Size: 139.6 MB (139568674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487d84247ee7669555e838408e05c3dabfeaa86ac1026553b49f95d33046914`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad1ed2c45ef912c44033b2049bb21d7602a2631666a1a00ea34a72385212358`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f56f614825f3f91b317f3db0564741146070246d5be546bd1e38cbc37c8cae4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167499715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3baaccfe9bec5aa2412a52b36fc411679e2c769501bc05b5bdf7d71d96125c9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:35:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 04:35:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 04:35:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 04:35:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 04:35:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 04:35:41 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 04:35:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 04:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 04:35:43 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 04:35:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823e0c350f02b4f697b67327987e02f972cd52cf2ea0f96f2cc3746ea0b50a44`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120da36ea9c1eed89a75905bed5f647c197c478a1db43e5a3a00f378e650a906`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2b71f7401e15f285d2758653f2d7b386770dfd75cd3e47d8833b80866c570f`  
		Last Modified: Thu, 04 Mar 2021 04:37:16 GMT  
		Size: 135.7 MB (135742521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12473a22009e488412a3ccfc540781b09b32758dacec9d6eaa8593364e4c20b2`  
		Last Modified: Thu, 04 Mar 2021 04:36:47 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52361ab241ff118e8095349be7438caaa778c9bc6d244532be2e5442b83c589`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:6a8ce34e89e708d16e4b381a922c1d16ecf06d2383c39fbadb735f7d3b00c855
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:5a1c46c78bac63be123bff52d38c2d10a02153af42c511c952c4af8dbb0a14c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175096021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85055945985ff6073cd1c27f52ab7da65bfd72af9af4c5bd2c94875a85044f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:27:13 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Mon, 22 Mar 2021 19:27:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:27:14 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:27:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_MAJOR=4.4
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_VERSION=4.4.4
# Mon, 22 Mar 2021 19:27:16 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:27:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:27:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:27:35 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:27:35 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:27:36 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81a8b8de1c04784d6d1e72f48119a95f94d72b8ae5f960d2b4097c232ba606`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782487be328415ddb46d726867068844c1fae6e9e4bcfcbcf6d6b7d2815deae4`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2092e9a3c4a7ad8deed4f6fe99dfaa6bc99a05748a35d9aff3b566f0aed48153`  
		Last Modified: Mon, 22 Mar 2021 19:29:59 GMT  
		Size: 139.6 MB (139568674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487d84247ee7669555e838408e05c3dabfeaa86ac1026553b49f95d33046914`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad1ed2c45ef912c44033b2049bb21d7602a2631666a1a00ea34a72385212358`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f56f614825f3f91b317f3db0564741146070246d5be546bd1e38cbc37c8cae4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167499715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3baaccfe9bec5aa2412a52b36fc411679e2c769501bc05b5bdf7d71d96125c9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:35:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 04:35:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 04:35:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 04:35:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 04:35:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 04:35:41 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 04:35:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 04:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 04:35:43 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 04:35:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823e0c350f02b4f697b67327987e02f972cd52cf2ea0f96f2cc3746ea0b50a44`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120da36ea9c1eed89a75905bed5f647c197c478a1db43e5a3a00f378e650a906`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2b71f7401e15f285d2758653f2d7b386770dfd75cd3e47d8833b80866c570f`  
		Last Modified: Thu, 04 Mar 2021 04:37:16 GMT  
		Size: 135.7 MB (135742521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12473a22009e488412a3ccfc540781b09b32758dacec9d6eaa8593364e4c20b2`  
		Last Modified: Thu, 04 Mar 2021 04:36:47 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52361ab241ff118e8095349be7438caaa778c9bc6d244532be2e5442b83c589`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:6a8ce34e89e708d16e4b381a922c1d16ecf06d2383c39fbadb735f7d3b00c855
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:5a1c46c78bac63be123bff52d38c2d10a02153af42c511c952c4af8dbb0a14c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175096021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85055945985ff6073cd1c27f52ab7da65bfd72af9af4c5bd2c94875a85044f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:27:13 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Mon, 22 Mar 2021 19:27:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:27:14 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:27:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_MAJOR=4.4
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_VERSION=4.4.4
# Mon, 22 Mar 2021 19:27:16 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:27:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:27:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:27:35 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:27:35 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:27:36 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81a8b8de1c04784d6d1e72f48119a95f94d72b8ae5f960d2b4097c232ba606`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782487be328415ddb46d726867068844c1fae6e9e4bcfcbcf6d6b7d2815deae4`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2092e9a3c4a7ad8deed4f6fe99dfaa6bc99a05748a35d9aff3b566f0aed48153`  
		Last Modified: Mon, 22 Mar 2021 19:29:59 GMT  
		Size: 139.6 MB (139568674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487d84247ee7669555e838408e05c3dabfeaa86ac1026553b49f95d33046914`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad1ed2c45ef912c44033b2049bb21d7602a2631666a1a00ea34a72385212358`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f56f614825f3f91b317f3db0564741146070246d5be546bd1e38cbc37c8cae4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167499715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3baaccfe9bec5aa2412a52b36fc411679e2c769501bc05b5bdf7d71d96125c9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:35:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 04:35:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 04:35:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 04:35:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 04:35:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 04:35:41 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 04:35:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 04:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 04:35:43 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 04:35:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823e0c350f02b4f697b67327987e02f972cd52cf2ea0f96f2cc3746ea0b50a44`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120da36ea9c1eed89a75905bed5f647c197c478a1db43e5a3a00f378e650a906`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2b71f7401e15f285d2758653f2d7b386770dfd75cd3e47d8833b80866c570f`  
		Last Modified: Thu, 04 Mar 2021 04:37:16 GMT  
		Size: 135.7 MB (135742521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12473a22009e488412a3ccfc540781b09b32758dacec9d6eaa8593364e4c20b2`  
		Last Modified: Thu, 04 Mar 2021 04:36:47 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52361ab241ff118e8095349be7438caaa778c9bc6d244532be2e5442b83c589`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 4.4 KB (4421 bytes)  
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
$ docker pull mongo@sha256:a0943cd354ccf6b98ff598b783c50a73fb36c160be958a85c1373443ddcfec0e
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
$ docker pull mongo@sha256:5a1c46c78bac63be123bff52d38c2d10a02153af42c511c952c4af8dbb0a14c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.1 MB (175096021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85055945985ff6073cd1c27f52ab7da65bfd72af9af4c5bd2c94875a85044f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:24:26 GMT
ADD file:d65963eb4f4b3a8c8e57119725a91036e8932a3e8f604e7edc21ff9665472da9 in / 
# Thu, 04 Mar 2021 02:24:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:24:28 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:24:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:24:29 GMT
CMD ["/bin/bash"]
# Mon, 22 Mar 2021 19:25:40 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Mon, 22 Mar 2021 19:26:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 22 Mar 2021 19:26:01 GMT
ENV GOSU_VERSION=1.12
# Mon, 22 Mar 2021 19:26:01 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 22 Mar 2021 19:26:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 22 Mar 2021 19:26:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 22 Mar 2021 19:27:13 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Mon, 22 Mar 2021 19:27:14 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Mon, 22 Mar 2021 19:27:14 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 22 Mar 2021 19:27:15 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_MAJOR=4.4
# Mon, 22 Mar 2021 19:27:15 GMT
ENV MONGO_VERSION=4.4.4
# Mon, 22 Mar 2021 19:27:16 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 22 Mar 2021 19:27:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 22 Mar 2021 19:27:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 22 Mar 2021 19:27:35 GMT
VOLUME [/data/db /data/configdb]
# Mon, 22 Mar 2021 19:27:35 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Mon, 22 Mar 2021 19:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 22 Mar 2021 19:27:36 GMT
EXPOSE 27017
# Mon, 22 Mar 2021 19:27:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:92dc2a97ff99354714f17180401813eb3073e4f62a67643d66b461505a604cbe`  
		Last Modified: Mon, 01 Mar 2021 16:09:46 GMT  
		Size: 26.7 MB (26710147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be13a9d27eb82db7e9c7f3a76f70919a2d690e34e78cda8cae60161b0f5e9137`  
		Last Modified: Thu, 04 Mar 2021 02:25:42 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8299583700ab4cc65a0126f99ca6f2b836a097dedcc64270094bea59b8b4306`  
		Last Modified: Thu, 04 Mar 2021 02:25:41 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5220358841a30196b99e6131310b5de8906226eefd4a5edde6882da4e2b5c1ac`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 1.9 KB (1875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e22072c39343ffad2849263b8cbbc3368c9eddf43a1589a7e3d90ff5a54133`  
		Last Modified: Mon, 22 Mar 2021 19:29:10 GMT  
		Size: 3.0 MB (2978337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31510a0ece571928ec103d01d66765cc5f2ff55fd050fa3375d245e6b02f84af`  
		Last Modified: Mon, 22 Mar 2021 19:29:11 GMT  
		Size: 5.8 MB (5829564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbde17806885159b7a51bc213db1937a9d0259e9a4176aa52474d665c1f6179`  
		Last Modified: Mon, 22 Mar 2021 19:29:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81a8b8de1c04784d6d1e72f48119a95f94d72b8ae5f960d2b4097c232ba606`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782487be328415ddb46d726867068844c1fae6e9e4bcfcbcf6d6b7d2815deae4`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2092e9a3c4a7ad8deed4f6fe99dfaa6bc99a05748a35d9aff3b566f0aed48153`  
		Last Modified: Mon, 22 Mar 2021 19:29:59 GMT  
		Size: 139.6 MB (139568674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487d84247ee7669555e838408e05c3dabfeaa86ac1026553b49f95d33046914`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad1ed2c45ef912c44033b2049bb21d7602a2631666a1a00ea34a72385212358`  
		Last Modified: Mon, 22 Mar 2021 19:29:35 GMT  
		Size: 4.4 KB (4424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f56f614825f3f91b317f3db0564741146070246d5be546bd1e38cbc37c8cae4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.5 MB (167499715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3baaccfe9bec5aa2412a52b36fc411679e2c769501bc05b5bdf7d71d96125c9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 04 Mar 2021 02:52:16 GMT
ADD file:bd92fdc04a5552a5b6596d4efffc3b5ca8dcce88e1f1c8d731c4039ce95b09cf in / 
# Thu, 04 Mar 2021 02:52:19 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 04 Mar 2021 02:52:21 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 04 Mar 2021 02:52:23 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 04 Mar 2021 02:52:24 GMT
CMD ["/bin/bash"]
# Thu, 04 Mar 2021 04:33:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 04 Mar 2021 04:33:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 Mar 2021 04:33:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 04 Mar 2021 04:33:35 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 04 Mar 2021 04:34:00 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 Mar 2021 04:34:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 04 Mar 2021 04:35:01 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 04 Mar 2021 04:35:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 04 Mar 2021 04:35:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_MAJOR=4.4
# Thu, 04 Mar 2021 04:35:07 GMT
ENV MONGO_VERSION=4.4.4
# Thu, 04 Mar 2021 04:35:09 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 04 Mar 2021 04:35:36 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 04 Mar 2021 04:35:40 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 04 Mar 2021 04:35:41 GMT
VOLUME [/data/db /data/configdb]
# Thu, 04 Mar 2021 04:35:42 GMT
COPY file:1e2f89ddb9d0d41f43b004ecc1dc9f0c927feb026da72e058059c2c932824c41 in /usr/local/bin/ 
# Thu, 04 Mar 2021 04:35:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Mar 2021 04:35:43 GMT
EXPOSE 27017
# Thu, 04 Mar 2021 04:35:44 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9243cbd63062004cb0062d0c8235fb578c194179c6526f26999de6c03daded31`  
		Last Modified: Tue, 23 Feb 2021 00:25:02 GMT  
		Size: 23.7 MB (23732051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ce98c92d8885e63c0bde376962ac7d15ebb891a7019f801e1de07be167209`  
		Last Modified: Thu, 04 Mar 2021 02:54:21 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e35ad787dffb8fc50bf32fc5febb71a414956f1a93b71360349b44b113fef`  
		Last Modified: Thu, 04 Mar 2021 02:54:20 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e242d61a3ff759f337cec4abba873a3cf41f30c1189e64300eac3a4adcef77c7`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1609f6354845021c0bbefd7505aba1c19e94e713f207cd697ff3878dc7630`  
		Last Modified: Thu, 04 Mar 2021 04:36:15 GMT  
		Size: 2.7 MB (2668787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92cb925337307ce497ce22ad2bbd2b20f9e939964173f6eebc81576fca9cd9c`  
		Last Modified: Thu, 04 Mar 2021 04:36:16 GMT  
		Size: 5.3 MB (5347024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0100ace87d2dd1694768c927da3180f6db643467fd6c127349d1a175da83754`  
		Last Modified: Thu, 04 Mar 2021 04:36:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823e0c350f02b4f697b67327987e02f972cd52cf2ea0f96f2cc3746ea0b50a44`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120da36ea9c1eed89a75905bed5f647c197c478a1db43e5a3a00f378e650a906`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2b71f7401e15f285d2758653f2d7b386770dfd75cd3e47d8833b80866c570f`  
		Last Modified: Thu, 04 Mar 2021 04:37:16 GMT  
		Size: 135.7 MB (135742521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12473a22009e488412a3ccfc540781b09b32758dacec9d6eaa8593364e4c20b2`  
		Last Modified: Thu, 04 Mar 2021 04:36:47 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52361ab241ff118e8095349be7438caaa778c9bc6d244532be2e5442b83c589`  
		Last Modified: Thu, 04 Mar 2021 04:36:46 GMT  
		Size: 4.4 KB (4421 bytes)  
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
