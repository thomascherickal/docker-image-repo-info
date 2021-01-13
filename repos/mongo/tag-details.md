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
-	[`mongo:4.2.11`](#mongo4211)
-	[`mongo:4.2.11-bionic`](#mongo4211-bionic)
-	[`mongo:4.2.11-windowsservercore`](#mongo4211-windowsservercore)
-	[`mongo:4.2.11-windowsservercore-1809`](#mongo4211-windowsservercore-1809)
-	[`mongo:4.2.11-windowsservercore-ltsc2016`](#mongo4211-windowsservercore-ltsc2016)
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
$ docker pull mongo@sha256:f415d7b5214792ddaff20b7a1bd88e581081a56befd75b66c19abba96984dc96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:3beff045471469bd82e8d072ef1729487a6a5a6f71eaeb6d9751b8a3b44c89f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (167954867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27d3bb28c66354b180c0c6e59580567321da9cee0d85c1ca67f3460f1825d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:27 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 26 Nov 2020 01:26:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_MAJOR=3.6
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 26 Nov 2020 01:26:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:26:46 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:26:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:26:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:08 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:09 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b67cb953c65f1761bc5fa7c37f51b8f9ae4d0028d3735814c28c1ed91e0a2a`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ef1c541d5d070f57546e35a709bbf08f369d0ebe0ef5a7b45f8545001b5e58`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34397889ad3a6209e4a57d2f618f57ffea691fbf53b55ac03d901baf32021a1f`  
		Last Modified: Thu, 26 Nov 2020 01:29:29 GMT  
		Size: 117.9 MB (117880402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d302d4d0319793b0358b6b1de9f6a8b2c0a795b04fdcdca13bdce2ccc8d9c61`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1415a65717211c59ba95b9d57bcebdcf2509a82c1910897e396996a37bd748c`  
		Last Modified: Fri, 11 Dec 2020 01:58:54 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:087797229526eab31efff922d996391bef0b78df6d8bc032e1f4d1cc0c179262
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156502318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38bca6ed6549495a380593103095d3b6aed6851d834f77b53b7c3fa5d5c9bde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:41:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 25 Nov 2020 23:41:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:41:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:41:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_MAJOR=3.6
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 25 Nov 2020 23:41:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:41:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:41:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:41:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:01 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:03 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b103e7401748c14934ea0b4164488d4b7a1586ae2c8a2d4c8ad93aeeb197df88`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1e51c370ae94e12adb627e0396ee1d7b2bc1e0254b2872a4718f232fdfa33`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b10bd75e0c79f031be4487cea6281a8328dfa962ad7e40d34a839d58b585804`  
		Last Modified: Wed, 25 Nov 2020 23:46:22 GMT  
		Size: 112.0 MB (111985589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f340d30b716234febde243893f1a5c20fdcd89555cd505fb7e7eb38eb222203`  
		Last Modified: Wed, 25 Nov 2020 23:45:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341288380326c947b67478074194a43b44a6dc7000b14cc5f31ad10f2b51614`  
		Last Modified: Wed, 13 Jan 2021 20:41:14 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:54c7ce51f0af2b0587ad66afb923a76f96c9a2d0d26a0f3baf097d844e9dcb10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619839732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5afb6190bd36553890eb55361abb2286f0043115b23f76641f0a61fbb6e4e692`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:09:58 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:13:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:13:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:13:19 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:13:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878add6b0813dc6422bfd5ea871624225078e96cd1d575f903d71534d4f1566`  
		Last Modified: Wed, 09 Dec 2020 23:43:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525f836c622f2833b82d00895554d4f2d099ac23abf95cb7c63698c948edd4fb`  
		Last Modified: Wed, 09 Dec 2020 23:43:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fe26e358f2b188b72a25f4e9205fd0110bd55b6f597aabf1961efac4ff7d37`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cde74370bc78d963b82fc925bd231f648457d7d5d0a3ddd1c7a4230bf35a8`  
		Last Modified: Wed, 09 Dec 2020 23:47:45 GMT  
		Size: 229.0 MB (228957311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c45215b7949fa3793d90dea9b18347c146135d1f781c5d5681df807b9e6ac3`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9c071c2e219cfebd610eac7db602ed3b07ca82a7e0a21bd387442db5a785a`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b3dfe0e400f47311228e8af998b4bc00ceed2d759e747422d62a200fba83`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:7084610676e296ea8210535e44c1e9982ac864877eb6c0330f3ddf4d3e09e0fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5998574744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e37f9306838934f62991fe4e4e2d5ad247a739be2687e04ab73fd9ff75e62ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:13:25 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:17:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:17:23 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:17:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4179bceab43ab8ae00ac2ba1c4ed220c48900fa641cc1551acf71ca295f4c672`  
		Last Modified: Wed, 09 Dec 2020 23:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb10d60d9a12b779c42e4a99ea514a9fb61a28f6f12d85483c85613aa6026b`  
		Last Modified: Wed, 09 Dec 2020 23:48:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca09872376df90935f8bb12c53e1991a91f3a4b8aaa81162eea0dc1580a4fae`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358aa22558f72dd990a3e140f71fc85a27574161f5feb066f1663cb20123c916`  
		Last Modified: Wed, 09 Dec 2020 23:48:47 GMT  
		Size: 229.7 MB (229722737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1968a12cbf437f67e090d087025ad0b94eaeabcd022bcf177ffc9069e88fa012`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920c6ce559fd25e6e36594f06fc92428726ead8e5c443139d364c53551458cb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0015d144ab29b7f665c678c239bcad042874fb85fe853c56b42f85bb8b7c23bb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:f415d7b5214792ddaff20b7a1bd88e581081a56befd75b66c19abba96984dc96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:3beff045471469bd82e8d072ef1729487a6a5a6f71eaeb6d9751b8a3b44c89f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (167954867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27d3bb28c66354b180c0c6e59580567321da9cee0d85c1ca67f3460f1825d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:27 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 26 Nov 2020 01:26:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_MAJOR=3.6
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 26 Nov 2020 01:26:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:26:46 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:26:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:26:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:08 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:09 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b67cb953c65f1761bc5fa7c37f51b8f9ae4d0028d3735814c28c1ed91e0a2a`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ef1c541d5d070f57546e35a709bbf08f369d0ebe0ef5a7b45f8545001b5e58`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34397889ad3a6209e4a57d2f618f57ffea691fbf53b55ac03d901baf32021a1f`  
		Last Modified: Thu, 26 Nov 2020 01:29:29 GMT  
		Size: 117.9 MB (117880402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d302d4d0319793b0358b6b1de9f6a8b2c0a795b04fdcdca13bdce2ccc8d9c61`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1415a65717211c59ba95b9d57bcebdcf2509a82c1910897e396996a37bd748c`  
		Last Modified: Fri, 11 Dec 2020 01:58:54 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:087797229526eab31efff922d996391bef0b78df6d8bc032e1f4d1cc0c179262
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156502318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38bca6ed6549495a380593103095d3b6aed6851d834f77b53b7c3fa5d5c9bde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:41:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 25 Nov 2020 23:41:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:41:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:41:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_MAJOR=3.6
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 25 Nov 2020 23:41:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:41:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:41:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:41:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:01 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:03 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b103e7401748c14934ea0b4164488d4b7a1586ae2c8a2d4c8ad93aeeb197df88`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1e51c370ae94e12adb627e0396ee1d7b2bc1e0254b2872a4718f232fdfa33`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b10bd75e0c79f031be4487cea6281a8328dfa962ad7e40d34a839d58b585804`  
		Last Modified: Wed, 25 Nov 2020 23:46:22 GMT  
		Size: 112.0 MB (111985589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f340d30b716234febde243893f1a5c20fdcd89555cd505fb7e7eb38eb222203`  
		Last Modified: Wed, 25 Nov 2020 23:45:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341288380326c947b67478074194a43b44a6dc7000b14cc5f31ad10f2b51614`  
		Last Modified: Wed, 13 Jan 2021 20:41:14 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:54c7ce51f0af2b0587ad66afb923a76f96c9a2d0d26a0f3baf097d844e9dcb10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619839732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5afb6190bd36553890eb55361abb2286f0043115b23f76641f0a61fbb6e4e692`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:09:58 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:13:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:13:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:13:19 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:13:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878add6b0813dc6422bfd5ea871624225078e96cd1d575f903d71534d4f1566`  
		Last Modified: Wed, 09 Dec 2020 23:43:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525f836c622f2833b82d00895554d4f2d099ac23abf95cb7c63698c948edd4fb`  
		Last Modified: Wed, 09 Dec 2020 23:43:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fe26e358f2b188b72a25f4e9205fd0110bd55b6f597aabf1961efac4ff7d37`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cde74370bc78d963b82fc925bd231f648457d7d5d0a3ddd1c7a4230bf35a8`  
		Last Modified: Wed, 09 Dec 2020 23:47:45 GMT  
		Size: 229.0 MB (228957311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c45215b7949fa3793d90dea9b18347c146135d1f781c5d5681df807b9e6ac3`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9c071c2e219cfebd610eac7db602ed3b07ca82a7e0a21bd387442db5a785a`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b3dfe0e400f47311228e8af998b4bc00ceed2d759e747422d62a200fba83`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:7084610676e296ea8210535e44c1e9982ac864877eb6c0330f3ddf4d3e09e0fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5998574744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e37f9306838934f62991fe4e4e2d5ad247a739be2687e04ab73fd9ff75e62ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:13:25 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:17:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:17:23 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:17:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4179bceab43ab8ae00ac2ba1c4ed220c48900fa641cc1551acf71ca295f4c672`  
		Last Modified: Wed, 09 Dec 2020 23:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb10d60d9a12b779c42e4a99ea514a9fb61a28f6f12d85483c85613aa6026b`  
		Last Modified: Wed, 09 Dec 2020 23:48:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca09872376df90935f8bb12c53e1991a91f3a4b8aaa81162eea0dc1580a4fae`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358aa22558f72dd990a3e140f71fc85a27574161f5feb066f1663cb20123c916`  
		Last Modified: Wed, 09 Dec 2020 23:48:47 GMT  
		Size: 229.7 MB (229722737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1968a12cbf437f67e090d087025ad0b94eaeabcd022bcf177ffc9069e88fa012`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920c6ce559fd25e6e36594f06fc92428726ead8e5c443139d364c53551458cb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0015d144ab29b7f665c678c239bcad042874fb85fe853c56b42f85bb8b7c23bb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21`

```console
$ docker pull mongo@sha256:f415d7b5214792ddaff20b7a1bd88e581081a56befd75b66c19abba96984dc96
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:3.6.21` - linux; amd64

```console
$ docker pull mongo@sha256:3beff045471469bd82e8d072ef1729487a6a5a6f71eaeb6d9751b8a3b44c89f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (167954867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27d3bb28c66354b180c0c6e59580567321da9cee0d85c1ca67f3460f1825d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:27 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 26 Nov 2020 01:26:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_MAJOR=3.6
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 26 Nov 2020 01:26:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:26:46 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:26:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:26:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:08 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:09 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b67cb953c65f1761bc5fa7c37f51b8f9ae4d0028d3735814c28c1ed91e0a2a`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ef1c541d5d070f57546e35a709bbf08f369d0ebe0ef5a7b45f8545001b5e58`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34397889ad3a6209e4a57d2f618f57ffea691fbf53b55ac03d901baf32021a1f`  
		Last Modified: Thu, 26 Nov 2020 01:29:29 GMT  
		Size: 117.9 MB (117880402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d302d4d0319793b0358b6b1de9f6a8b2c0a795b04fdcdca13bdce2ccc8d9c61`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1415a65717211c59ba95b9d57bcebdcf2509a82c1910897e396996a37bd748c`  
		Last Modified: Fri, 11 Dec 2020 01:58:54 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:087797229526eab31efff922d996391bef0b78df6d8bc032e1f4d1cc0c179262
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156502318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38bca6ed6549495a380593103095d3b6aed6851d834f77b53b7c3fa5d5c9bde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:41:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 25 Nov 2020 23:41:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:41:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:41:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_MAJOR=3.6
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 25 Nov 2020 23:41:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:41:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:41:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:41:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:01 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:03 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b103e7401748c14934ea0b4164488d4b7a1586ae2c8a2d4c8ad93aeeb197df88`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1e51c370ae94e12adb627e0396ee1d7b2bc1e0254b2872a4718f232fdfa33`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b10bd75e0c79f031be4487cea6281a8328dfa962ad7e40d34a839d58b585804`  
		Last Modified: Wed, 25 Nov 2020 23:46:22 GMT  
		Size: 112.0 MB (111985589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f340d30b716234febde243893f1a5c20fdcd89555cd505fb7e7eb38eb222203`  
		Last Modified: Wed, 25 Nov 2020 23:45:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341288380326c947b67478074194a43b44a6dc7000b14cc5f31ad10f2b51614`  
		Last Modified: Wed, 13 Jan 2021 20:41:14 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:54c7ce51f0af2b0587ad66afb923a76f96c9a2d0d26a0f3baf097d844e9dcb10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619839732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5afb6190bd36553890eb55361abb2286f0043115b23f76641f0a61fbb6e4e692`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:09:58 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:13:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:13:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:13:19 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:13:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878add6b0813dc6422bfd5ea871624225078e96cd1d575f903d71534d4f1566`  
		Last Modified: Wed, 09 Dec 2020 23:43:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525f836c622f2833b82d00895554d4f2d099ac23abf95cb7c63698c948edd4fb`  
		Last Modified: Wed, 09 Dec 2020 23:43:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fe26e358f2b188b72a25f4e9205fd0110bd55b6f597aabf1961efac4ff7d37`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cde74370bc78d963b82fc925bd231f648457d7d5d0a3ddd1c7a4230bf35a8`  
		Last Modified: Wed, 09 Dec 2020 23:47:45 GMT  
		Size: 229.0 MB (228957311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c45215b7949fa3793d90dea9b18347c146135d1f781c5d5681df807b9e6ac3`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9c071c2e219cfebd610eac7db602ed3b07ca82a7e0a21bd387442db5a785a`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b3dfe0e400f47311228e8af998b4bc00ceed2d759e747422d62a200fba83`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:7084610676e296ea8210535e44c1e9982ac864877eb6c0330f3ddf4d3e09e0fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5998574744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e37f9306838934f62991fe4e4e2d5ad247a739be2687e04ab73fd9ff75e62ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:13:25 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:17:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:17:23 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:17:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4179bceab43ab8ae00ac2ba1c4ed220c48900fa641cc1551acf71ca295f4c672`  
		Last Modified: Wed, 09 Dec 2020 23:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb10d60d9a12b779c42e4a99ea514a9fb61a28f6f12d85483c85613aa6026b`  
		Last Modified: Wed, 09 Dec 2020 23:48:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca09872376df90935f8bb12c53e1991a91f3a4b8aaa81162eea0dc1580a4fae`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358aa22558f72dd990a3e140f71fc85a27574161f5feb066f1663cb20123c916`  
		Last Modified: Wed, 09 Dec 2020 23:48:47 GMT  
		Size: 229.7 MB (229722737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1968a12cbf437f67e090d087025ad0b94eaeabcd022bcf177ffc9069e88fa012`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920c6ce559fd25e6e36594f06fc92428726ead8e5c443139d364c53551458cb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0015d144ab29b7f665c678c239bcad042874fb85fe853c56b42f85bb8b7c23bb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21-windowsservercore`

```console
$ docker pull mongo@sha256:dd1fe67d392e594ee68b15ff5d1088e1b9e2a42ef3a82693a785c89aae37dc1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:3.6.21-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:54c7ce51f0af2b0587ad66afb923a76f96c9a2d0d26a0f3baf097d844e9dcb10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619839732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5afb6190bd36553890eb55361abb2286f0043115b23f76641f0a61fbb6e4e692`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:09:58 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:13:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:13:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:13:19 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:13:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878add6b0813dc6422bfd5ea871624225078e96cd1d575f903d71534d4f1566`  
		Last Modified: Wed, 09 Dec 2020 23:43:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525f836c622f2833b82d00895554d4f2d099ac23abf95cb7c63698c948edd4fb`  
		Last Modified: Wed, 09 Dec 2020 23:43:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fe26e358f2b188b72a25f4e9205fd0110bd55b6f597aabf1961efac4ff7d37`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cde74370bc78d963b82fc925bd231f648457d7d5d0a3ddd1c7a4230bf35a8`  
		Last Modified: Wed, 09 Dec 2020 23:47:45 GMT  
		Size: 229.0 MB (228957311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c45215b7949fa3793d90dea9b18347c146135d1f781c5d5681df807b9e6ac3`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9c071c2e219cfebd610eac7db602ed3b07ca82a7e0a21bd387442db5a785a`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b3dfe0e400f47311228e8af998b4bc00ceed2d759e747422d62a200fba83`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:7084610676e296ea8210535e44c1e9982ac864877eb6c0330f3ddf4d3e09e0fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5998574744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e37f9306838934f62991fe4e4e2d5ad247a739be2687e04ab73fd9ff75e62ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:13:25 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:17:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:17:23 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:17:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4179bceab43ab8ae00ac2ba1c4ed220c48900fa641cc1551acf71ca295f4c672`  
		Last Modified: Wed, 09 Dec 2020 23:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb10d60d9a12b779c42e4a99ea514a9fb61a28f6f12d85483c85613aa6026b`  
		Last Modified: Wed, 09 Dec 2020 23:48:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca09872376df90935f8bb12c53e1991a91f3a4b8aaa81162eea0dc1580a4fae`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358aa22558f72dd990a3e140f71fc85a27574161f5feb066f1663cb20123c916`  
		Last Modified: Wed, 09 Dec 2020 23:48:47 GMT  
		Size: 229.7 MB (229722737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1968a12cbf437f67e090d087025ad0b94eaeabcd022bcf177ffc9069e88fa012`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920c6ce559fd25e6e36594f06fc92428726ead8e5c443139d364c53551458cb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0015d144ab29b7f665c678c239bcad042874fb85fe853c56b42f85bb8b7c23bb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a22b898c46e55f29aa79689da5000bfb4e4b4ef9b2896054f2179ca0453b6a3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:3.6.21-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:54c7ce51f0af2b0587ad66afb923a76f96c9a2d0d26a0f3baf097d844e9dcb10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619839732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5afb6190bd36553890eb55361abb2286f0043115b23f76641f0a61fbb6e4e692`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:09:58 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:13:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:13:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:13:19 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:13:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878add6b0813dc6422bfd5ea871624225078e96cd1d575f903d71534d4f1566`  
		Last Modified: Wed, 09 Dec 2020 23:43:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525f836c622f2833b82d00895554d4f2d099ac23abf95cb7c63698c948edd4fb`  
		Last Modified: Wed, 09 Dec 2020 23:43:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fe26e358f2b188b72a25f4e9205fd0110bd55b6f597aabf1961efac4ff7d37`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cde74370bc78d963b82fc925bd231f648457d7d5d0a3ddd1c7a4230bf35a8`  
		Last Modified: Wed, 09 Dec 2020 23:47:45 GMT  
		Size: 229.0 MB (228957311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c45215b7949fa3793d90dea9b18347c146135d1f781c5d5681df807b9e6ac3`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9c071c2e219cfebd610eac7db602ed3b07ca82a7e0a21bd387442db5a785a`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b3dfe0e400f47311228e8af998b4bc00ceed2d759e747422d62a200fba83`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:d0d930cb8ce902603f622bcbe51ce3374bb2612e677bd4e73b771cdc979724b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:3.6.21-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:7084610676e296ea8210535e44c1e9982ac864877eb6c0330f3ddf4d3e09e0fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5998574744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e37f9306838934f62991fe4e4e2d5ad247a739be2687e04ab73fd9ff75e62ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:13:25 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:17:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:17:23 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:17:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4179bceab43ab8ae00ac2ba1c4ed220c48900fa641cc1551acf71ca295f4c672`  
		Last Modified: Wed, 09 Dec 2020 23:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb10d60d9a12b779c42e4a99ea514a9fb61a28f6f12d85483c85613aa6026b`  
		Last Modified: Wed, 09 Dec 2020 23:48:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca09872376df90935f8bb12c53e1991a91f3a4b8aaa81162eea0dc1580a4fae`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358aa22558f72dd990a3e140f71fc85a27574161f5feb066f1663cb20123c916`  
		Last Modified: Wed, 09 Dec 2020 23:48:47 GMT  
		Size: 229.7 MB (229722737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1968a12cbf437f67e090d087025ad0b94eaeabcd022bcf177ffc9069e88fa012`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920c6ce559fd25e6e36594f06fc92428726ead8e5c443139d364c53551458cb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0015d144ab29b7f665c678c239bcad042874fb85fe853c56b42f85bb8b7c23bb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.21-xenial`

```console
$ docker pull mongo@sha256:3e6242d6ef4fe91a2d135da19adba03ccfcb4c1ad9fbda151f83c2f0dd178843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.21-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:3beff045471469bd82e8d072ef1729487a6a5a6f71eaeb6d9751b8a3b44c89f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (167954867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27d3bb28c66354b180c0c6e59580567321da9cee0d85c1ca67f3460f1825d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:27 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 26 Nov 2020 01:26:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_MAJOR=3.6
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 26 Nov 2020 01:26:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:26:46 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:26:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:26:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:08 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:09 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b67cb953c65f1761bc5fa7c37f51b8f9ae4d0028d3735814c28c1ed91e0a2a`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ef1c541d5d070f57546e35a709bbf08f369d0ebe0ef5a7b45f8545001b5e58`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34397889ad3a6209e4a57d2f618f57ffea691fbf53b55ac03d901baf32021a1f`  
		Last Modified: Thu, 26 Nov 2020 01:29:29 GMT  
		Size: 117.9 MB (117880402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d302d4d0319793b0358b6b1de9f6a8b2c0a795b04fdcdca13bdce2ccc8d9c61`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1415a65717211c59ba95b9d57bcebdcf2509a82c1910897e396996a37bd748c`  
		Last Modified: Fri, 11 Dec 2020 01:58:54 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.21-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:087797229526eab31efff922d996391bef0b78df6d8bc032e1f4d1cc0c179262
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156502318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38bca6ed6549495a380593103095d3b6aed6851d834f77b53b7c3fa5d5c9bde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:41:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 25 Nov 2020 23:41:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:41:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:41:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_MAJOR=3.6
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 25 Nov 2020 23:41:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:41:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:41:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:41:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:01 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:03 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b103e7401748c14934ea0b4164488d4b7a1586ae2c8a2d4c8ad93aeeb197df88`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1e51c370ae94e12adb627e0396ee1d7b2bc1e0254b2872a4718f232fdfa33`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b10bd75e0c79f031be4487cea6281a8328dfa962ad7e40d34a839d58b585804`  
		Last Modified: Wed, 25 Nov 2020 23:46:22 GMT  
		Size: 112.0 MB (111985589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f340d30b716234febde243893f1a5c20fdcd89555cd505fb7e7eb38eb222203`  
		Last Modified: Wed, 25 Nov 2020 23:45:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341288380326c947b67478074194a43b44a6dc7000b14cc5f31ad10f2b51614`  
		Last Modified: Wed, 13 Jan 2021 20:41:14 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:dd1fe67d392e594ee68b15ff5d1088e1b9e2a42ef3a82693a785c89aae37dc1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:54c7ce51f0af2b0587ad66afb923a76f96c9a2d0d26a0f3baf097d844e9dcb10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619839732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5afb6190bd36553890eb55361abb2286f0043115b23f76641f0a61fbb6e4e692`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:09:58 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:13:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:13:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:13:19 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:13:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878add6b0813dc6422bfd5ea871624225078e96cd1d575f903d71534d4f1566`  
		Last Modified: Wed, 09 Dec 2020 23:43:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525f836c622f2833b82d00895554d4f2d099ac23abf95cb7c63698c948edd4fb`  
		Last Modified: Wed, 09 Dec 2020 23:43:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fe26e358f2b188b72a25f4e9205fd0110bd55b6f597aabf1961efac4ff7d37`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cde74370bc78d963b82fc925bd231f648457d7d5d0a3ddd1c7a4230bf35a8`  
		Last Modified: Wed, 09 Dec 2020 23:47:45 GMT  
		Size: 229.0 MB (228957311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c45215b7949fa3793d90dea9b18347c146135d1f781c5d5681df807b9e6ac3`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9c071c2e219cfebd610eac7db602ed3b07ca82a7e0a21bd387442db5a785a`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b3dfe0e400f47311228e8af998b4bc00ceed2d759e747422d62a200fba83`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:7084610676e296ea8210535e44c1e9982ac864877eb6c0330f3ddf4d3e09e0fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5998574744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e37f9306838934f62991fe4e4e2d5ad247a739be2687e04ab73fd9ff75e62ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:13:25 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:17:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:17:23 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:17:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4179bceab43ab8ae00ac2ba1c4ed220c48900fa641cc1551acf71ca295f4c672`  
		Last Modified: Wed, 09 Dec 2020 23:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb10d60d9a12b779c42e4a99ea514a9fb61a28f6f12d85483c85613aa6026b`  
		Last Modified: Wed, 09 Dec 2020 23:48:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca09872376df90935f8bb12c53e1991a91f3a4b8aaa81162eea0dc1580a4fae`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358aa22558f72dd990a3e140f71fc85a27574161f5feb066f1663cb20123c916`  
		Last Modified: Wed, 09 Dec 2020 23:48:47 GMT  
		Size: 229.7 MB (229722737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1968a12cbf437f67e090d087025ad0b94eaeabcd022bcf177ffc9069e88fa012`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920c6ce559fd25e6e36594f06fc92428726ead8e5c443139d364c53551458cb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0015d144ab29b7f665c678c239bcad042874fb85fe853c56b42f85bb8b7c23bb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a22b898c46e55f29aa79689da5000bfb4e4b4ef9b2896054f2179ca0453b6a3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:54c7ce51f0af2b0587ad66afb923a76f96c9a2d0d26a0f3baf097d844e9dcb10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619839732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5afb6190bd36553890eb55361abb2286f0043115b23f76641f0a61fbb6e4e692`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:09:58 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:13:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:13:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:13:19 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:13:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878add6b0813dc6422bfd5ea871624225078e96cd1d575f903d71534d4f1566`  
		Last Modified: Wed, 09 Dec 2020 23:43:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525f836c622f2833b82d00895554d4f2d099ac23abf95cb7c63698c948edd4fb`  
		Last Modified: Wed, 09 Dec 2020 23:43:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fe26e358f2b188b72a25f4e9205fd0110bd55b6f597aabf1961efac4ff7d37`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cde74370bc78d963b82fc925bd231f648457d7d5d0a3ddd1c7a4230bf35a8`  
		Last Modified: Wed, 09 Dec 2020 23:47:45 GMT  
		Size: 229.0 MB (228957311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c45215b7949fa3793d90dea9b18347c146135d1f781c5d5681df807b9e6ac3`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9c071c2e219cfebd610eac7db602ed3b07ca82a7e0a21bd387442db5a785a`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b3dfe0e400f47311228e8af998b4bc00ceed2d759e747422d62a200fba83`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:d0d930cb8ce902603f622bcbe51ce3374bb2612e677bd4e73b771cdc979724b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:7084610676e296ea8210535e44c1e9982ac864877eb6c0330f3ddf4d3e09e0fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5998574744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e37f9306838934f62991fe4e4e2d5ad247a739be2687e04ab73fd9ff75e62ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:13:25 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:17:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:17:23 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:17:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4179bceab43ab8ae00ac2ba1c4ed220c48900fa641cc1551acf71ca295f4c672`  
		Last Modified: Wed, 09 Dec 2020 23:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb10d60d9a12b779c42e4a99ea514a9fb61a28f6f12d85483c85613aa6026b`  
		Last Modified: Wed, 09 Dec 2020 23:48:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca09872376df90935f8bb12c53e1991a91f3a4b8aaa81162eea0dc1580a4fae`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358aa22558f72dd990a3e140f71fc85a27574161f5feb066f1663cb20123c916`  
		Last Modified: Wed, 09 Dec 2020 23:48:47 GMT  
		Size: 229.7 MB (229722737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1968a12cbf437f67e090d087025ad0b94eaeabcd022bcf177ffc9069e88fa012`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920c6ce559fd25e6e36594f06fc92428726ead8e5c443139d364c53551458cb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0015d144ab29b7f665c678c239bcad042874fb85fe853c56b42f85bb8b7c23bb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:3e6242d6ef4fe91a2d135da19adba03ccfcb4c1ad9fbda151f83c2f0dd178843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:3beff045471469bd82e8d072ef1729487a6a5a6f71eaeb6d9751b8a3b44c89f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (167954867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27d3bb28c66354b180c0c6e59580567321da9cee0d85c1ca67f3460f1825d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:27 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 26 Nov 2020 01:26:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_MAJOR=3.6
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 26 Nov 2020 01:26:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:26:46 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:26:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:26:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:08 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:09 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b67cb953c65f1761bc5fa7c37f51b8f9ae4d0028d3735814c28c1ed91e0a2a`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ef1c541d5d070f57546e35a709bbf08f369d0ebe0ef5a7b45f8545001b5e58`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34397889ad3a6209e4a57d2f618f57ffea691fbf53b55ac03d901baf32021a1f`  
		Last Modified: Thu, 26 Nov 2020 01:29:29 GMT  
		Size: 117.9 MB (117880402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d302d4d0319793b0358b6b1de9f6a8b2c0a795b04fdcdca13bdce2ccc8d9c61`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1415a65717211c59ba95b9d57bcebdcf2509a82c1910897e396996a37bd748c`  
		Last Modified: Fri, 11 Dec 2020 01:58:54 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:087797229526eab31efff922d996391bef0b78df6d8bc032e1f4d1cc0c179262
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156502318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38bca6ed6549495a380593103095d3b6aed6851d834f77b53b7c3fa5d5c9bde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:41:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 25 Nov 2020 23:41:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:41:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:41:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_MAJOR=3.6
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 25 Nov 2020 23:41:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:41:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:41:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:41:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:01 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:03 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b103e7401748c14934ea0b4164488d4b7a1586ae2c8a2d4c8ad93aeeb197df88`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1e51c370ae94e12adb627e0396ee1d7b2bc1e0254b2872a4718f232fdfa33`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b10bd75e0c79f031be4487cea6281a8328dfa962ad7e40d34a839d58b585804`  
		Last Modified: Wed, 25 Nov 2020 23:46:22 GMT  
		Size: 112.0 MB (111985589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f340d30b716234febde243893f1a5c20fdcd89555cd505fb7e7eb38eb222203`  
		Last Modified: Wed, 25 Nov 2020 23:45:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341288380326c947b67478074194a43b44a6dc7000b14cc5f31ad10f2b51614`  
		Last Modified: Wed, 13 Jan 2021 20:41:14 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:dd1fe67d392e594ee68b15ff5d1088e1b9e2a42ef3a82693a785c89aae37dc1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:3-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:54c7ce51f0af2b0587ad66afb923a76f96c9a2d0d26a0f3baf097d844e9dcb10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619839732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5afb6190bd36553890eb55361abb2286f0043115b23f76641f0a61fbb6e4e692`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:09:58 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:13:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:13:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:13:19 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:13:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878add6b0813dc6422bfd5ea871624225078e96cd1d575f903d71534d4f1566`  
		Last Modified: Wed, 09 Dec 2020 23:43:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525f836c622f2833b82d00895554d4f2d099ac23abf95cb7c63698c948edd4fb`  
		Last Modified: Wed, 09 Dec 2020 23:43:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fe26e358f2b188b72a25f4e9205fd0110bd55b6f597aabf1961efac4ff7d37`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cde74370bc78d963b82fc925bd231f648457d7d5d0a3ddd1c7a4230bf35a8`  
		Last Modified: Wed, 09 Dec 2020 23:47:45 GMT  
		Size: 229.0 MB (228957311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c45215b7949fa3793d90dea9b18347c146135d1f781c5d5681df807b9e6ac3`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9c071c2e219cfebd610eac7db602ed3b07ca82a7e0a21bd387442db5a785a`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b3dfe0e400f47311228e8af998b4bc00ceed2d759e747422d62a200fba83`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:7084610676e296ea8210535e44c1e9982ac864877eb6c0330f3ddf4d3e09e0fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5998574744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e37f9306838934f62991fe4e4e2d5ad247a739be2687e04ab73fd9ff75e62ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:13:25 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:17:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:17:23 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:17:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4179bceab43ab8ae00ac2ba1c4ed220c48900fa641cc1551acf71ca295f4c672`  
		Last Modified: Wed, 09 Dec 2020 23:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb10d60d9a12b779c42e4a99ea514a9fb61a28f6f12d85483c85613aa6026b`  
		Last Modified: Wed, 09 Dec 2020 23:48:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca09872376df90935f8bb12c53e1991a91f3a4b8aaa81162eea0dc1580a4fae`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358aa22558f72dd990a3e140f71fc85a27574161f5feb066f1663cb20123c916`  
		Last Modified: Wed, 09 Dec 2020 23:48:47 GMT  
		Size: 229.7 MB (229722737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1968a12cbf437f67e090d087025ad0b94eaeabcd022bcf177ffc9069e88fa012`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920c6ce559fd25e6e36594f06fc92428726ead8e5c443139d364c53551458cb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0015d144ab29b7f665c678c239bcad042874fb85fe853c56b42f85bb8b7c23bb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a22b898c46e55f29aa79689da5000bfb4e4b4ef9b2896054f2179ca0453b6a3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:54c7ce51f0af2b0587ad66afb923a76f96c9a2d0d26a0f3baf097d844e9dcb10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2619839732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5afb6190bd36553890eb55361abb2286f0043115b23f76641f0a61fbb6e4e692`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:09:58 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:09:59 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:13:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:13:19 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:13:19 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:13:20 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878add6b0813dc6422bfd5ea871624225078e96cd1d575f903d71534d4f1566`  
		Last Modified: Wed, 09 Dec 2020 23:43:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525f836c622f2833b82d00895554d4f2d099ac23abf95cb7c63698c948edd4fb`  
		Last Modified: Wed, 09 Dec 2020 23:43:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fe26e358f2b188b72a25f4e9205fd0110bd55b6f597aabf1961efac4ff7d37`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cde74370bc78d963b82fc925bd231f648457d7d5d0a3ddd1c7a4230bf35a8`  
		Last Modified: Wed, 09 Dec 2020 23:47:45 GMT  
		Size: 229.0 MB (228957311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c45215b7949fa3793d90dea9b18347c146135d1f781c5d5681df807b9e6ac3`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e9c071c2e219cfebd610eac7db602ed3b07ca82a7e0a21bd387442db5a785a`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922b3dfe0e400f47311228e8af998b4bc00ceed2d759e747422d62a200fba83`  
		Last Modified: Wed, 09 Dec 2020 23:43:39 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:d0d930cb8ce902603f622bcbe51ce3374bb2612e677bd4e73b771cdc979724b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:7084610676e296ea8210535e44c1e9982ac864877eb6c0330f3ddf4d3e09e0fa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5998574744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e37f9306838934f62991fe4e4e2d5ad247a739be2687e04ab73fd9ff75e62ee`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:13:25 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.21-signed.msi
# Wed, 09 Dec 2020 23:13:26 GMT
ENV MONGO_DOWNLOAD_SHA256=0b64db8d8a615976b76617c3425c9fc0500e18324be0de878a6c6143d1e8b5e2
# Wed, 09 Dec 2020 23:17:22 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Server,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:17:23 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:17:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4179bceab43ab8ae00ac2ba1c4ed220c48900fa641cc1551acf71ca295f4c672`  
		Last Modified: Wed, 09 Dec 2020 23:48:03 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb10d60d9a12b779c42e4a99ea514a9fb61a28f6f12d85483c85613aa6026b`  
		Last Modified: Wed, 09 Dec 2020 23:48:04 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca09872376df90935f8bb12c53e1991a91f3a4b8aaa81162eea0dc1580a4fae`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358aa22558f72dd990a3e140f71fc85a27574161f5feb066f1663cb20123c916`  
		Last Modified: Wed, 09 Dec 2020 23:48:47 GMT  
		Size: 229.7 MB (229722737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1968a12cbf437f67e090d087025ad0b94eaeabcd022bcf177ffc9069e88fa012`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4920c6ce559fd25e6e36594f06fc92428726ead8e5c443139d364c53551458cb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0015d144ab29b7f665c678c239bcad042874fb85fe853c56b42f85bb8b7c23bb`  
		Last Modified: Wed, 09 Dec 2020 23:48:00 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:3e6242d6ef4fe91a2d135da19adba03ccfcb4c1ad9fbda151f83c2f0dd178843
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:3beff045471469bd82e8d072ef1729487a6a5a6f71eaeb6d9751b8a3b44c89f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (167954867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27d3bb28c66354b180c0c6e59580567321da9cee0d85c1ca67f3460f1825d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:27 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 26 Nov 2020 01:26:28 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:26:28 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_MAJOR=3.6
# Thu, 26 Nov 2020 01:26:29 GMT
ENV MONGO_VERSION=3.6.21
# Thu, 26 Nov 2020 01:26:30 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:26:46 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:26:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:26:48 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:08 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:09 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:09 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b67cb953c65f1761bc5fa7c37f51b8f9ae4d0028d3735814c28c1ed91e0a2a`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ef1c541d5d070f57546e35a709bbf08f369d0ebe0ef5a7b45f8545001b5e58`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34397889ad3a6209e4a57d2f618f57ffea691fbf53b55ac03d901baf32021a1f`  
		Last Modified: Thu, 26 Nov 2020 01:29:29 GMT  
		Size: 117.9 MB (117880402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d302d4d0319793b0358b6b1de9f6a8b2c0a795b04fdcdca13bdce2ccc8d9c61`  
		Last Modified: Thu, 26 Nov 2020 01:29:11 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1415a65717211c59ba95b9d57bcebdcf2509a82c1910897e396996a37bd748c`  
		Last Modified: Fri, 11 Dec 2020 01:58:54 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:087797229526eab31efff922d996391bef0b78df6d8bc032e1f4d1cc0c179262
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156502318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38bca6ed6549495a380593103095d3b6aed6851d834f77b53b7c3fa5d5c9bde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:41:07 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 25 Nov 2020 23:41:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:41:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:41:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:12 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_MAJOR=3.6
# Wed, 25 Nov 2020 23:41:13 GMT
ENV MONGO_VERSION=3.6.21
# Wed, 25 Nov 2020 23:41:17 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:41:39 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:41:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:41:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:01 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:03 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b103e7401748c14934ea0b4164488d4b7a1586ae2c8a2d4c8ad93aeeb197df88`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 2.0 KB (1995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a1e51c370ae94e12adb627e0396ee1d7b2bc1e0254b2872a4718f232fdfa33`  
		Last Modified: Wed, 25 Nov 2020 23:45:56 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b10bd75e0c79f031be4487cea6281a8328dfa962ad7e40d34a839d58b585804`  
		Last Modified: Wed, 25 Nov 2020 23:46:22 GMT  
		Size: 112.0 MB (111985589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f340d30b716234febde243893f1a5c20fdcd89555cd505fb7e7eb38eb222203`  
		Last Modified: Wed, 25 Nov 2020 23:45:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2341288380326c947b67478074194a43b44a6dc7000b14cc5f31ad10f2b51614`  
		Last Modified: Wed, 13 Jan 2021 20:41:14 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:094f04532c279cb96da991692896e5a013939e2471e4a98791aa5cd7a196981c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:c46e1f6dd8ac3f8592b53fa2dfdc0f7e26055929e6bf30975838ca0406c5bc2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178220204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97feb3412a387d4d3bbd8653b09ef26683263a192e0e8dc6554e65bfb637a86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:28:23 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 01:28:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:28:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:28:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:20:44 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:20:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:21:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:21:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:21:11 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:21:11 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:21:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:21:12 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:21:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e4e43cb0003675e06e2e17e30cb17e0e9a990abc8a107f259c93be84ccc4f`  
		Last Modified: Thu, 26 Nov 2020 01:30:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50e71d834e14ca61531dcce8e5e52860ea3b03769e5e68cf77ac07e941f6d6`  
		Last Modified: Mon, 04 Jan 2021 22:22:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27768a0d0c674b5175f704d585df68ad33f9bd5be976bd669801075e8ca63526`  
		Last Modified: Mon, 04 Jan 2021 22:22:36 GMT  
		Size: 142.7 MB (142684977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4e0bd8b992a6db5b94cd268f50463e33f8a470bd7b8b3772a177714ce8ccd7`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c887415d06431f09f31175932c083142d41a7de019c848489c1e5412e4b14635`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:66fd4f8f09e92de8744c76702e836f0fc5831255318373435935bc3d589b5f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168150811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25db05811c760dc9c9ba32746c241a6e8a67669179651b91931ba04adf1076d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:44:48 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 25 Nov 2020 23:44:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:44:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:44:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:56 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:43:16 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:43:19 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:43:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:31 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:32 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4913f11c494a00e3d77d01b9364c56f69482ffaeddf32e87f424acd659acff9`  
		Last Modified: Wed, 25 Nov 2020 23:47:35 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17fffdaae13eded3257e5cef69f19565cb07b9602919924393e099e88d56ab9`  
		Last Modified: Mon, 04 Jan 2021 22:44:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c65f20a6385ac5b1be7e719820d32fe6d98175958ee48624f07341afba641aa`  
		Last Modified: Mon, 04 Jan 2021 22:45:23 GMT  
		Size: 136.4 MB (136379637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0fec39db28299b0b7d33a9a2f3a99f3bd9c0cc78ac9190d5c5a33f780ae566`  
		Last Modified: Mon, 04 Jan 2021 22:44:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7c251da439065584411bea56b6288812cbae60767613397e8960289dceaeed`  
		Last Modified: Wed, 13 Jan 2021 20:41:45 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:543de10da111411668affef0a4572320b1a53aad1afd2fd2fec58b4de13cadb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173130142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f718506b8817f58d5917d2b4c2b344ffda20b91739e3701d5b277100d7a8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:54 GMT
ADD file:aa0063276274c9f3ba9308c3cdfd911449966c87546f28ceb3122d6fbd995d52 in / 
# Wed, 25 Nov 2020 22:45:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:07:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 00:08:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:08:17 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 00:08:18 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 00:08:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 00:08:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 00:08:44 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 00:08:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 00:08:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 00:08:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:41:47 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:41:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:11 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:41:41 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:41:42 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:41:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2269433521a3f2e95508abd4fa29a3de21226eed5a09ad3959a689b066151bca`  
		Last Modified: Mon, 23 Nov 2020 18:41:52 GMT  
		Size: 25.4 MB (25381722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442687b9aa7dcd6b97d4f9ce9562774788922b94571cd3a7ea85185cd76cbd3`  
		Last Modified: Wed, 25 Nov 2020 22:47:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6efa602a92c53f638f3667fa4400f2fdb32c5aaae3d112e33f15a12cb2bb3b`  
		Last Modified: Wed, 25 Nov 2020 22:47:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a5fb2071960493a99805bac4506cb07225b998113d5ae9b344509442f9e542`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8d2ce236c235c465ef891cd59df829a91e12d07301f95cdc23d077c44d81a`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 2.7 MB (2720968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ce7bbcb36617017b697c1cedd0f4dad2273643f9315dcb5665c9731e031b3`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 5.7 MB (5746421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621599eddf8a561bdfb15886b7a9609c02a01369e9bd02c9937cdaa7b3ccc212`  
		Last Modified: Thu, 26 Nov 2020 00:10:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0760577d520065d34f4c5a7340b154a10776867a6448a2f6a8692ffe23ea21e`  
		Last Modified: Thu, 26 Nov 2020 00:10:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd26d3d155865f99e5f9f9cc78acd78b78951980e96b704a3d6fc62125f266`  
		Last Modified: Mon, 04 Jan 2021 22:43:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b55cdba3dc093e0f2f23a688d26ebfd23bcbda7c077566297ac179280a6568`  
		Last Modified: Mon, 04 Jan 2021 22:43:51 GMT  
		Size: 139.3 MB (139271674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0584912549af62baba56b0311441340f5a45f758f1c3a96d739b4ca98eb7a8`  
		Last Modified: Mon, 04 Jan 2021 22:43:30 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b0b7d81cfea5fa13c01706f15f9a99a732d4faa0ab0b3637fd26fccd72864`  
		Last Modified: Wed, 13 Jan 2021 20:42:29 GMT  
		Size: 4.5 KB (4450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:827f7b634519ea7587320b90833353c8fdec392f2e7eed7384a540f3c96a38f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:9b7750d3e671e5419cf49a36b362fdf19c88fd9f6781682b962d67d23534d772
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155983661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ea882cfd09a8ce18a192e71efb5ff2a37f69bca43493ac6ba235af9b472e53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 26 Nov 2020 01:27:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:27:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:27:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:01 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:01 GMT
ENV MONGO_MAJOR=4.0
# Mon, 04 Jan 2021 22:20:01 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:20:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:20:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:20:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:20:33 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:20:34 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:20:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:20:34 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:20:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280988dec1a3155a03caf131e2769e632618ff813a510c4923b1d5d7a1853129`  
		Last Modified: Thu, 26 Nov 2020 01:29:37 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca33adca074bb86f5c45495fdcd8697f1b8f70261911e6cb330ff0bfc09cd6`  
		Last Modified: Mon, 04 Jan 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c9034c7cc4611dc84447285ab11ae7cb11c35b207ad6f97649aa76b9b78e3d`  
		Last Modified: Mon, 04 Jan 2021 22:22:04 GMT  
		Size: 105.9 MB (105909754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3c28517e24476cab8b84546b302ef5a327a9d81f549344ddcbbaf09f33728e`  
		Last Modified: Mon, 04 Jan 2021 22:21:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca257e88866d1dbd59b885992283e4102d4c4c1952460d7a5fa8f51caf1725`  
		Last Modified: Mon, 04 Jan 2021 22:21:48 GMT  
		Size: 4.4 KB (4417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f3a469a016cdafd5fca08a136d366de2d6848a51e69e6cab57641e52ebde79e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144799170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52e4e38a99f161576ea59cd0848ef73d56bdbe16c59b791a01f8db05ea1221b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:42:01 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 25 Nov 2020 23:42:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:42:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:42:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:42:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:42:09 GMT
ENV MONGO_MAJOR=4.0
# Mon, 04 Jan 2021 22:42:03 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:42:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:42:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:42:56 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:10 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:12 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e042cf744a51f09bc81674c76d7372f171390e3336b518b92a7631a982454b8a`  
		Last Modified: Wed, 25 Nov 2020 23:46:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38689b92944ec46aefd60d27b80ef65c9c7dcd9e964fe70caaa448f8f2c4de60`  
		Last Modified: Mon, 04 Jan 2021 22:44:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a70b249c328f7fd5fea295c4d389cece12b68aedd12bd59ad8fb087787a942`  
		Last Modified: Mon, 04 Jan 2021 22:44:44 GMT  
		Size: 100.3 MB (100283009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3fceb4b5f13e4d8d64c2f037784e379e38e3fbe4ffa111791090a3c528c370`  
		Last Modified: Mon, 04 Jan 2021 22:44:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7232000012564fe447a421334d246324591d2761f91817c304e4c88d11de7eb1`  
		Last Modified: Wed, 13 Jan 2021 20:41:27 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:1d8f6d1374c3ec0cf0f292d0dd12a540dfca978441e1897c35e0f5e7ea76fad8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2625604028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815d950bd8a50355a2a3ae9f6ba73648c3de4c9d63246564090b8afcf3fef8ff`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:15:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:18:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:18:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:18:49 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:18:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda55b5434f58c392948319f4824c671a57bccbe837bd20ef509b8d76a17dea8`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc3afde0716cc5054d204db7b56ea2d57d9aba2fd89422b78d8fec456731c21`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d448a9d7d05f8a6ac1863e6533717fbb720c0cc92bb2958e83e534f9d9a20ec`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b135f58a92dad445e70a98d48be40b1b8f7e4f1d287e933b749d8ffa6b55a145`  
		Last Modified: Mon, 04 Jan 2021 22:33:07 GMT  
		Size: 234.7 MB (234721580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f689a15d2e41de84dfb4ed477eb2e96a305851f711c5b3f789b67a55b5848c35`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e065ff5f2f970d6c1c8d7dfcb2747f247e69c03863c210458630d838ab345c`  
		Last Modified: Mon, 04 Jan 2021 22:32:24 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c659d398be9011941c4d24317feeade7c1268129065dfd91075f128049e1aac`  
		Last Modified: Mon, 04 Jan 2021 22:32:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:b97dc28560810f6b066119df1de1a99b6c77e0f5038c6f0b81c833a1baf0666f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004324338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4f040def8979869848e2a23c7cee1f2a90184b7c1cff955a9281c9d4a2d046`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:18:57 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:18:58 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:18:59 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:23:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:23:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:23:11 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:23:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed66930b820455a6fdf31a61dbc20e320ea98c1daef7013bc2f9463ce2fa4a9`  
		Last Modified: Mon, 04 Jan 2021 22:33:25 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b453ac56054c282d5ed7259ed6ad635abd89bf89d5a504819fa931c5ffb76b`  
		Last Modified: Mon, 04 Jan 2021 22:33:24 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed139acc33b8502d2bb360df9bad74e0df5dc589d6beccc51a8b2c364e7a6a0`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90893da25c32736113f02d42b199b011e398fd21cdb69ac8409b1a96c295ab`  
		Last Modified: Mon, 04 Jan 2021 22:34:06 GMT  
		Size: 235.5 MB (235472517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d640ebc1f91b2ab2ecaf6ddfad7163db7d5bfe4f5992b3e2d858699e70db05d9`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6895d4abade85e015816246b1dab1b9c10e1b77de34ef79739a0dd4fb441187`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8adf7e49b83e9707d033b5d9a68a0b9b5a9ddb062cf9827e022fad9822ac6`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22`

```console
$ docker pull mongo@sha256:827f7b634519ea7587320b90833353c8fdec392f2e7eed7384a540f3c96a38f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.0.22` - linux; amd64

```console
$ docker pull mongo@sha256:9b7750d3e671e5419cf49a36b362fdf19c88fd9f6781682b962d67d23534d772
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155983661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ea882cfd09a8ce18a192e71efb5ff2a37f69bca43493ac6ba235af9b472e53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 26 Nov 2020 01:27:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:27:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:27:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:01 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:01 GMT
ENV MONGO_MAJOR=4.0
# Mon, 04 Jan 2021 22:20:01 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:20:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:20:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:20:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:20:33 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:20:34 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:20:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:20:34 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:20:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280988dec1a3155a03caf131e2769e632618ff813a510c4923b1d5d7a1853129`  
		Last Modified: Thu, 26 Nov 2020 01:29:37 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca33adca074bb86f5c45495fdcd8697f1b8f70261911e6cb330ff0bfc09cd6`  
		Last Modified: Mon, 04 Jan 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c9034c7cc4611dc84447285ab11ae7cb11c35b207ad6f97649aa76b9b78e3d`  
		Last Modified: Mon, 04 Jan 2021 22:22:04 GMT  
		Size: 105.9 MB (105909754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3c28517e24476cab8b84546b302ef5a327a9d81f549344ddcbbaf09f33728e`  
		Last Modified: Mon, 04 Jan 2021 22:21:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca257e88866d1dbd59b885992283e4102d4c4c1952460d7a5fa8f51caf1725`  
		Last Modified: Mon, 04 Jan 2021 22:21:48 GMT  
		Size: 4.4 KB (4417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f3a469a016cdafd5fca08a136d366de2d6848a51e69e6cab57641e52ebde79e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144799170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52e4e38a99f161576ea59cd0848ef73d56bdbe16c59b791a01f8db05ea1221b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:42:01 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 25 Nov 2020 23:42:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:42:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:42:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:42:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:42:09 GMT
ENV MONGO_MAJOR=4.0
# Mon, 04 Jan 2021 22:42:03 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:42:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:42:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:42:56 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:10 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:12 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e042cf744a51f09bc81674c76d7372f171390e3336b518b92a7631a982454b8a`  
		Last Modified: Wed, 25 Nov 2020 23:46:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38689b92944ec46aefd60d27b80ef65c9c7dcd9e964fe70caaa448f8f2c4de60`  
		Last Modified: Mon, 04 Jan 2021 22:44:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a70b249c328f7fd5fea295c4d389cece12b68aedd12bd59ad8fb087787a942`  
		Last Modified: Mon, 04 Jan 2021 22:44:44 GMT  
		Size: 100.3 MB (100283009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3fceb4b5f13e4d8d64c2f037784e379e38e3fbe4ffa111791090a3c528c370`  
		Last Modified: Mon, 04 Jan 2021 22:44:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7232000012564fe447a421334d246324591d2761f91817c304e4c88d11de7eb1`  
		Last Modified: Wed, 13 Jan 2021 20:41:27 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:1d8f6d1374c3ec0cf0f292d0dd12a540dfca978441e1897c35e0f5e7ea76fad8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2625604028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815d950bd8a50355a2a3ae9f6ba73648c3de4c9d63246564090b8afcf3fef8ff`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:15:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:18:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:18:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:18:49 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:18:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda55b5434f58c392948319f4824c671a57bccbe837bd20ef509b8d76a17dea8`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc3afde0716cc5054d204db7b56ea2d57d9aba2fd89422b78d8fec456731c21`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d448a9d7d05f8a6ac1863e6533717fbb720c0cc92bb2958e83e534f9d9a20ec`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b135f58a92dad445e70a98d48be40b1b8f7e4f1d287e933b749d8ffa6b55a145`  
		Last Modified: Mon, 04 Jan 2021 22:33:07 GMT  
		Size: 234.7 MB (234721580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f689a15d2e41de84dfb4ed477eb2e96a305851f711c5b3f789b67a55b5848c35`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e065ff5f2f970d6c1c8d7dfcb2747f247e69c03863c210458630d838ab345c`  
		Last Modified: Mon, 04 Jan 2021 22:32:24 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c659d398be9011941c4d24317feeade7c1268129065dfd91075f128049e1aac`  
		Last Modified: Mon, 04 Jan 2021 22:32:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:b97dc28560810f6b066119df1de1a99b6c77e0f5038c6f0b81c833a1baf0666f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004324338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4f040def8979869848e2a23c7cee1f2a90184b7c1cff955a9281c9d4a2d046`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:18:57 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:18:58 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:18:59 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:23:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:23:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:23:11 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:23:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed66930b820455a6fdf31a61dbc20e320ea98c1daef7013bc2f9463ce2fa4a9`  
		Last Modified: Mon, 04 Jan 2021 22:33:25 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b453ac56054c282d5ed7259ed6ad635abd89bf89d5a504819fa931c5ffb76b`  
		Last Modified: Mon, 04 Jan 2021 22:33:24 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed139acc33b8502d2bb360df9bad74e0df5dc589d6beccc51a8b2c364e7a6a0`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90893da25c32736113f02d42b199b011e398fd21cdb69ac8409b1a96c295ab`  
		Last Modified: Mon, 04 Jan 2021 22:34:06 GMT  
		Size: 235.5 MB (235472517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d640ebc1f91b2ab2ecaf6ddfad7163db7d5bfe4f5992b3e2d858699e70db05d9`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6895d4abade85e015816246b1dab1b9c10e1b77de34ef79739a0dd4fb441187`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8adf7e49b83e9707d033b5d9a68a0b9b5a9ddb062cf9827e022fad9822ac6`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22-windowsservercore`

```console
$ docker pull mongo@sha256:17c93f68d1795be6f8c9e026742f00408fc7c5a146df1ffdadcc76ccb4a3b052
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.0.22-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:1d8f6d1374c3ec0cf0f292d0dd12a540dfca978441e1897c35e0f5e7ea76fad8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2625604028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815d950bd8a50355a2a3ae9f6ba73648c3de4c9d63246564090b8afcf3fef8ff`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:15:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:18:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:18:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:18:49 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:18:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda55b5434f58c392948319f4824c671a57bccbe837bd20ef509b8d76a17dea8`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc3afde0716cc5054d204db7b56ea2d57d9aba2fd89422b78d8fec456731c21`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d448a9d7d05f8a6ac1863e6533717fbb720c0cc92bb2958e83e534f9d9a20ec`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b135f58a92dad445e70a98d48be40b1b8f7e4f1d287e933b749d8ffa6b55a145`  
		Last Modified: Mon, 04 Jan 2021 22:33:07 GMT  
		Size: 234.7 MB (234721580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f689a15d2e41de84dfb4ed477eb2e96a305851f711c5b3f789b67a55b5848c35`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e065ff5f2f970d6c1c8d7dfcb2747f247e69c03863c210458630d838ab345c`  
		Last Modified: Mon, 04 Jan 2021 22:32:24 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c659d398be9011941c4d24317feeade7c1268129065dfd91075f128049e1aac`  
		Last Modified: Mon, 04 Jan 2021 22:32:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:b97dc28560810f6b066119df1de1a99b6c77e0f5038c6f0b81c833a1baf0666f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004324338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4f040def8979869848e2a23c7cee1f2a90184b7c1cff955a9281c9d4a2d046`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:18:57 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:18:58 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:18:59 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:23:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:23:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:23:11 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:23:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed66930b820455a6fdf31a61dbc20e320ea98c1daef7013bc2f9463ce2fa4a9`  
		Last Modified: Mon, 04 Jan 2021 22:33:25 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b453ac56054c282d5ed7259ed6ad635abd89bf89d5a504819fa931c5ffb76b`  
		Last Modified: Mon, 04 Jan 2021 22:33:24 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed139acc33b8502d2bb360df9bad74e0df5dc589d6beccc51a8b2c364e7a6a0`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90893da25c32736113f02d42b199b011e398fd21cdb69ac8409b1a96c295ab`  
		Last Modified: Mon, 04 Jan 2021 22:34:06 GMT  
		Size: 235.5 MB (235472517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d640ebc1f91b2ab2ecaf6ddfad7163db7d5bfe4f5992b3e2d858699e70db05d9`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6895d4abade85e015816246b1dab1b9c10e1b77de34ef79739a0dd4fb441187`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8adf7e49b83e9707d033b5d9a68a0b9b5a9ddb062cf9827e022fad9822ac6`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22-windowsservercore-1809`

```console
$ docker pull mongo@sha256:3c9ed60b2a1e5617db2bbb6b43c9e6270780bc352129669d3419c7eae68d89bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:4.0.22-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:1d8f6d1374c3ec0cf0f292d0dd12a540dfca978441e1897c35e0f5e7ea76fad8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2625604028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815d950bd8a50355a2a3ae9f6ba73648c3de4c9d63246564090b8afcf3fef8ff`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:15:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:18:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:18:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:18:49 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:18:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda55b5434f58c392948319f4824c671a57bccbe837bd20ef509b8d76a17dea8`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc3afde0716cc5054d204db7b56ea2d57d9aba2fd89422b78d8fec456731c21`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d448a9d7d05f8a6ac1863e6533717fbb720c0cc92bb2958e83e534f9d9a20ec`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b135f58a92dad445e70a98d48be40b1b8f7e4f1d287e933b749d8ffa6b55a145`  
		Last Modified: Mon, 04 Jan 2021 22:33:07 GMT  
		Size: 234.7 MB (234721580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f689a15d2e41de84dfb4ed477eb2e96a305851f711c5b3f789b67a55b5848c35`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e065ff5f2f970d6c1c8d7dfcb2747f247e69c03863c210458630d838ab345c`  
		Last Modified: Mon, 04 Jan 2021 22:32:24 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c659d398be9011941c4d24317feeade7c1268129065dfd91075f128049e1aac`  
		Last Modified: Mon, 04 Jan 2021 22:32:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9758c0ac80b856aa4354369059ba9f107205d14e26d9b10ebf7b4e71bd00657c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.0.22-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:b97dc28560810f6b066119df1de1a99b6c77e0f5038c6f0b81c833a1baf0666f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004324338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4f040def8979869848e2a23c7cee1f2a90184b7c1cff955a9281c9d4a2d046`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:18:57 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:18:58 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:18:59 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:23:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:23:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:23:11 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:23:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed66930b820455a6fdf31a61dbc20e320ea98c1daef7013bc2f9463ce2fa4a9`  
		Last Modified: Mon, 04 Jan 2021 22:33:25 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b453ac56054c282d5ed7259ed6ad635abd89bf89d5a504819fa931c5ffb76b`  
		Last Modified: Mon, 04 Jan 2021 22:33:24 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed139acc33b8502d2bb360df9bad74e0df5dc589d6beccc51a8b2c364e7a6a0`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90893da25c32736113f02d42b199b011e398fd21cdb69ac8409b1a96c295ab`  
		Last Modified: Mon, 04 Jan 2021 22:34:06 GMT  
		Size: 235.5 MB (235472517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d640ebc1f91b2ab2ecaf6ddfad7163db7d5bfe4f5992b3e2d858699e70db05d9`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6895d4abade85e015816246b1dab1b9c10e1b77de34ef79739a0dd4fb441187`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8adf7e49b83e9707d033b5d9a68a0b9b5a9ddb062cf9827e022fad9822ac6`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.22-xenial`

```console
$ docker pull mongo@sha256:b33f54aeec719117bd70767058b61240a744788aedf1ed6059ae8ca689c950aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.22-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:9b7750d3e671e5419cf49a36b362fdf19c88fd9f6781682b962d67d23534d772
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155983661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ea882cfd09a8ce18a192e71efb5ff2a37f69bca43493ac6ba235af9b472e53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 26 Nov 2020 01:27:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:27:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:27:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:01 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:01 GMT
ENV MONGO_MAJOR=4.0
# Mon, 04 Jan 2021 22:20:01 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:20:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:20:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:20:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:20:33 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:20:34 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:20:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:20:34 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:20:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280988dec1a3155a03caf131e2769e632618ff813a510c4923b1d5d7a1853129`  
		Last Modified: Thu, 26 Nov 2020 01:29:37 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca33adca074bb86f5c45495fdcd8697f1b8f70261911e6cb330ff0bfc09cd6`  
		Last Modified: Mon, 04 Jan 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c9034c7cc4611dc84447285ab11ae7cb11c35b207ad6f97649aa76b9b78e3d`  
		Last Modified: Mon, 04 Jan 2021 22:22:04 GMT  
		Size: 105.9 MB (105909754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3c28517e24476cab8b84546b302ef5a327a9d81f549344ddcbbaf09f33728e`  
		Last Modified: Mon, 04 Jan 2021 22:21:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca257e88866d1dbd59b885992283e4102d4c4c1952460d7a5fa8f51caf1725`  
		Last Modified: Mon, 04 Jan 2021 22:21:48 GMT  
		Size: 4.4 KB (4417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.22-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f3a469a016cdafd5fca08a136d366de2d6848a51e69e6cab57641e52ebde79e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144799170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52e4e38a99f161576ea59cd0848ef73d56bdbe16c59b791a01f8db05ea1221b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:42:01 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 25 Nov 2020 23:42:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:42:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:42:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:42:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:42:09 GMT
ENV MONGO_MAJOR=4.0
# Mon, 04 Jan 2021 22:42:03 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:42:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:42:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:42:56 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:10 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:12 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e042cf744a51f09bc81674c76d7372f171390e3336b518b92a7631a982454b8a`  
		Last Modified: Wed, 25 Nov 2020 23:46:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38689b92944ec46aefd60d27b80ef65c9c7dcd9e964fe70caaa448f8f2c4de60`  
		Last Modified: Mon, 04 Jan 2021 22:44:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a70b249c328f7fd5fea295c4d389cece12b68aedd12bd59ad8fb087787a942`  
		Last Modified: Mon, 04 Jan 2021 22:44:44 GMT  
		Size: 100.3 MB (100283009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3fceb4b5f13e4d8d64c2f037784e379e38e3fbe4ffa111791090a3c528c370`  
		Last Modified: Mon, 04 Jan 2021 22:44:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7232000012564fe447a421334d246324591d2761f91817c304e4c88d11de7eb1`  
		Last Modified: Wed, 13 Jan 2021 20:41:27 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:17c93f68d1795be6f8c9e026742f00408fc7c5a146df1ffdadcc76ccb4a3b052
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:1d8f6d1374c3ec0cf0f292d0dd12a540dfca978441e1897c35e0f5e7ea76fad8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2625604028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815d950bd8a50355a2a3ae9f6ba73648c3de4c9d63246564090b8afcf3fef8ff`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:15:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:18:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:18:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:18:49 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:18:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda55b5434f58c392948319f4824c671a57bccbe837bd20ef509b8d76a17dea8`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc3afde0716cc5054d204db7b56ea2d57d9aba2fd89422b78d8fec456731c21`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d448a9d7d05f8a6ac1863e6533717fbb720c0cc92bb2958e83e534f9d9a20ec`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b135f58a92dad445e70a98d48be40b1b8f7e4f1d287e933b749d8ffa6b55a145`  
		Last Modified: Mon, 04 Jan 2021 22:33:07 GMT  
		Size: 234.7 MB (234721580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f689a15d2e41de84dfb4ed477eb2e96a305851f711c5b3f789b67a55b5848c35`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e065ff5f2f970d6c1c8d7dfcb2747f247e69c03863c210458630d838ab345c`  
		Last Modified: Mon, 04 Jan 2021 22:32:24 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c659d398be9011941c4d24317feeade7c1268129065dfd91075f128049e1aac`  
		Last Modified: Mon, 04 Jan 2021 22:32:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:b97dc28560810f6b066119df1de1a99b6c77e0f5038c6f0b81c833a1baf0666f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004324338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4f040def8979869848e2a23c7cee1f2a90184b7c1cff955a9281c9d4a2d046`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:18:57 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:18:58 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:18:59 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:23:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:23:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:23:11 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:23:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed66930b820455a6fdf31a61dbc20e320ea98c1daef7013bc2f9463ce2fa4a9`  
		Last Modified: Mon, 04 Jan 2021 22:33:25 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b453ac56054c282d5ed7259ed6ad635abd89bf89d5a504819fa931c5ffb76b`  
		Last Modified: Mon, 04 Jan 2021 22:33:24 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed139acc33b8502d2bb360df9bad74e0df5dc589d6beccc51a8b2c364e7a6a0`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90893da25c32736113f02d42b199b011e398fd21cdb69ac8409b1a96c295ab`  
		Last Modified: Mon, 04 Jan 2021 22:34:06 GMT  
		Size: 235.5 MB (235472517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d640ebc1f91b2ab2ecaf6ddfad7163db7d5bfe4f5992b3e2d858699e70db05d9`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6895d4abade85e015816246b1dab1b9c10e1b77de34ef79739a0dd4fb441187`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8adf7e49b83e9707d033b5d9a68a0b9b5a9ddb062cf9827e022fad9822ac6`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:3c9ed60b2a1e5617db2bbb6b43c9e6270780bc352129669d3419c7eae68d89bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:1d8f6d1374c3ec0cf0f292d0dd12a540dfca978441e1897c35e0f5e7ea76fad8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2625604028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815d950bd8a50355a2a3ae9f6ba73648c3de4c9d63246564090b8afcf3fef8ff`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:15:16 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:15:17 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:18:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:18:48 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:18:49 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:18:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda55b5434f58c392948319f4824c671a57bccbe837bd20ef509b8d76a17dea8`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc3afde0716cc5054d204db7b56ea2d57d9aba2fd89422b78d8fec456731c21`  
		Last Modified: Mon, 04 Jan 2021 22:32:25 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d448a9d7d05f8a6ac1863e6533717fbb720c0cc92bb2958e83e534f9d9a20ec`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b135f58a92dad445e70a98d48be40b1b8f7e4f1d287e933b749d8ffa6b55a145`  
		Last Modified: Mon, 04 Jan 2021 22:33:07 GMT  
		Size: 234.7 MB (234721580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f689a15d2e41de84dfb4ed477eb2e96a305851f711c5b3f789b67a55b5848c35`  
		Last Modified: Mon, 04 Jan 2021 22:32:23 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e065ff5f2f970d6c1c8d7dfcb2747f247e69c03863c210458630d838ab345c`  
		Last Modified: Mon, 04 Jan 2021 22:32:24 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c659d398be9011941c4d24317feeade7c1268129065dfd91075f128049e1aac`  
		Last Modified: Mon, 04 Jan 2021 22:32:22 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:9758c0ac80b856aa4354369059ba9f107205d14e26d9b10ebf7b4e71bd00657c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:b97dc28560810f6b066119df1de1a99b6c77e0f5038c6f0b81c833a1baf0666f
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6004324338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4f040def8979869848e2a23c7cee1f2a90184b7c1cff955a9281c9d4a2d046`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:18:57 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:18:58 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.22-signed.msi
# Mon, 04 Jan 2021 22:18:59 GMT
ENV MONGO_DOWNLOAD_SHA256=e2145277031424a7e72084f94d8014146a119e3dce284da5140f66a113c5e473
# Mon, 04 Jan 2021 22:23:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:23:11 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:23:11 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:23:12 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed66930b820455a6fdf31a61dbc20e320ea98c1daef7013bc2f9463ce2fa4a9`  
		Last Modified: Mon, 04 Jan 2021 22:33:25 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b453ac56054c282d5ed7259ed6ad635abd89bf89d5a504819fa931c5ffb76b`  
		Last Modified: Mon, 04 Jan 2021 22:33:24 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed139acc33b8502d2bb360df9bad74e0df5dc589d6beccc51a8b2c364e7a6a0`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b90893da25c32736113f02d42b199b011e398fd21cdb69ac8409b1a96c295ab`  
		Last Modified: Mon, 04 Jan 2021 22:34:06 GMT  
		Size: 235.5 MB (235472517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d640ebc1f91b2ab2ecaf6ddfad7163db7d5bfe4f5992b3e2d858699e70db05d9`  
		Last Modified: Mon, 04 Jan 2021 22:33:23 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6895d4abade85e015816246b1dab1b9c10e1b77de34ef79739a0dd4fb441187`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa8adf7e49b83e9707d033b5d9a68a0b9b5a9ddb062cf9827e022fad9822ac6`  
		Last Modified: Mon, 04 Jan 2021 22:33:20 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:b33f54aeec719117bd70767058b61240a744788aedf1ed6059ae8ca689c950aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:9b7750d3e671e5419cf49a36b362fdf19c88fd9f6781682b962d67d23534d772
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (155983661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ea882cfd09a8ce18a192e71efb5ff2a37f69bca43493ac6ba235af9b472e53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:26:11 GMT
ADD file:8eef54430e581236e6d529a7d09df648f43c840e889d9ae132e5ed25d7bd2b88 in / 
# Wed, 25 Nov 2020 22:26:12 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:26:13 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:26:14 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:26:14 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:26:05 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:26:14 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:26:14 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:26:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:26:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:26:59 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 26 Nov 2020 01:27:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:27:00 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:27:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:01 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:01 GMT
ENV MONGO_MAJOR=4.0
# Mon, 04 Jan 2021 22:20:01 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:20:02 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:20:32 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:20:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:20:33 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:20:34 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:20:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:20:34 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:20:34 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:be8ec4e48d7f24a9a1c01063e5dfabb092c2c1ec73e125113848553c9b07eb8c`  
		Last Modified: Sat, 31 Oct 2020 14:20:23 GMT  
		Size: 45.8 MB (45838270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b8b485aff0509bb0fa67dff6a2aa82e9b7b17e5ef28c1673467ec83edb945d`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d887158cc58cbfc3d03cefd5c0b15175fae66ffbf6f28a56180c51cbb5062b8a`  
		Last Modified: Wed, 25 Nov 2020 22:27:14 GMT  
		Size: 533.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05895bb28c18264f614acd13e401b3c5594e12d9fe90d7e52929d3e810e11e97`  
		Last Modified: Wed, 25 Nov 2020 22:27:15 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554956c5520b91826f67a69c857085abe6308b305bf724001852f30444d1d240`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.0 KB (1989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129bf37b6f0e8c688cffb0577d721030022a07ff49f5ecf1b80879039bca187`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 2.9 MB (2920120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a961c831444b5f831645776d13caf4e607cc03e471e87ab6a68bd98dd55d3f4`  
		Last Modified: Thu, 26 Nov 2020 01:29:13 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002e342bfc39f4560472f645a1173cd67daa71236e97f479ab407ffa5b8e489d`  
		Last Modified: Thu, 26 Nov 2020 01:29:12 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280988dec1a3155a03caf131e2769e632618ff813a510c4923b1d5d7a1853129`  
		Last Modified: Thu, 26 Nov 2020 01:29:37 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ca33adca074bb86f5c45495fdcd8697f1b8f70261911e6cb330ff0bfc09cd6`  
		Last Modified: Mon, 04 Jan 2021 22:21:47 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c9034c7cc4611dc84447285ab11ae7cb11c35b207ad6f97649aa76b9b78e3d`  
		Last Modified: Mon, 04 Jan 2021 22:22:04 GMT  
		Size: 105.9 MB (105909754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3c28517e24476cab8b84546b302ef5a327a9d81f549344ddcbbaf09f33728e`  
		Last Modified: Mon, 04 Jan 2021 22:21:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ca257e88866d1dbd59b885992283e4102d4c4c1952460d7a5fa8f51caf1725`  
		Last Modified: Mon, 04 Jan 2021 22:21:48 GMT  
		Size: 4.4 KB (4417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:f3a469a016cdafd5fca08a136d366de2d6848a51e69e6cab57641e52ebde79e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144799170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b52e4e38a99f161576ea59cd0848ef73d56bdbe16c59b791a01f8db05ea1221b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:40:14 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:40:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:40:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:40:33 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:41:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:41:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:42:01 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 25 Nov 2020 23:42:04 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:42:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:42:07 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:42:08 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:42:09 GMT
ENV MONGO_MAJOR=4.0
# Mon, 04 Jan 2021 22:42:03 GMT
ENV MONGO_VERSION=4.0.22
# Mon, 04 Jan 2021 22:42:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:52 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:42:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:42:56 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:10 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:12 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e9126b813149c7bffbc15cc97f7c795aa0246b998c8bf5dc5a8a7ca129251e`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 2.0 KB (1993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94c06431efd0a6d59c01bbe2538ddf6804a7badaa0fed71a99f34d07f801bef`  
		Last Modified: Wed, 25 Nov 2020 23:46:00 GMT  
		Size: 2.4 MB (2447641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b29d68a07614dcc8898ca7982d168bef8d1772390fd5c1bf2fc0f907f57f06`  
		Last Modified: Wed, 25 Nov 2020 23:45:59 GMT  
		Size: 1.2 MB (1232502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9a549684af8d71bb84e6c8353b8ebe96560183b0499727ac815fa9048991b5`  
		Last Modified: Wed, 25 Nov 2020 23:45:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e042cf744a51f09bc81674c76d7372f171390e3336b518b92a7631a982454b8a`  
		Last Modified: Wed, 25 Nov 2020 23:46:32 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38689b92944ec46aefd60d27b80ef65c9c7dcd9e964fe70caaa448f8f2c4de60`  
		Last Modified: Mon, 04 Jan 2021 22:44:22 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a70b249c328f7fd5fea295c4d389cece12b68aedd12bd59ad8fb087787a942`  
		Last Modified: Mon, 04 Jan 2021 22:44:44 GMT  
		Size: 100.3 MB (100283009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3fceb4b5f13e4d8d64c2f037784e379e38e3fbe4ffa111791090a3c528c370`  
		Last Modified: Mon, 04 Jan 2021 22:44:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7232000012564fe447a421334d246324591d2761f91817c304e4c88d11de7eb1`  
		Last Modified: Wed, 13 Jan 2021 20:41:27 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:793ff08818edee0ae6c0c0be8b0542ce5a8521671e3915ee7b67bdfed7bb9a4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:890f506c2f919da36fb42d6a7de9874cc5d7adbe86a5e3b085e14ab39214d724
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165061323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511fe7789ae9bcedbe831171699aa524af2d4d3de37b5b7afdca74510c2a3d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:27:51 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 26 Nov 2020 01:27:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:27:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:27:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_MAJOR=4.2
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 26 Nov 2020 01:27:56 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:28:14 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:28:15 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:28:16 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:19 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:20 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b974c007ba520e60343cf372d76ee97bebb73b634e1a5e5936cb40e735cab`  
		Last Modified: Thu, 26 Nov 2020 01:29:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a6135ee562c5ce4407869bcbc6ed7d49517519277c55f6de2aac9dd00c9d6e`  
		Last Modified: Thu, 26 Nov 2020 01:30:00 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a5cbea1a515622883b9979af49f22b729488bf95873dd2aba3704100ce4d9d`  
		Last Modified: Thu, 26 Nov 2020 01:30:33 GMT  
		Size: 129.5 MB (129526094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9176a2e7afd6cfcde6349939b5d402049a11f7b1b4e53ed7306ea551483d0e05`  
		Last Modified: Thu, 26 Nov 2020 01:29:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b94f239e8a0dd7dd56508f1d94df3e0c1d066ace3a01f46c5dd612cf18c81e`  
		Last Modified: Fri, 11 Dec 2020 01:59:06 GMT  
		Size: 4.4 KB (4411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ce71251a85fdd9a4d93f45073f1ca55be867648e6187546ccf08cfee642d0624
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155046521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8309fe7dd97337eb1ba9d1e8ed4e18e3a19f617217d7f4c195ae3fbc78a7a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:43:45 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 25 Nov 2020 23:43:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:43:49 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:43:50 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:43:51 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:43:52 GMT
ENV MONGO_MAJOR=4.2
# Wed, 25 Nov 2020 23:43:53 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 25 Nov 2020 23:43:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:44:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:44:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:44:25 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:22 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:23 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:24 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244d5d8425ae8bd01528b5941f9d98e600443eeb7d1ef78f1f0569555fd89075`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05339f1902e2eff54eac65e727a1c398e7b51fd444661e28946229c1d57fcd4f`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8db58f0b3460af59d37fc0b84ad4cc8dedfe508211268c102f1a9718b4c65c`  
		Last Modified: Wed, 25 Nov 2020 23:47:28 GMT  
		Size: 123.3 MB (123275334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8cf676ac5fef9b9a7a315c81b8cc72ed78a78a13a52fe9b21491cfb4a062ff`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4741ed0d09dcf55d3516b68b2ddf4b63e0e970f028f5204ef142c434b51e85`  
		Last Modified: Wed, 13 Jan 2021 20:41:38 GMT  
		Size: 4.4 KB (4448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:dcefd7f962f48e6a4627c27ba97bd819f0f37e55cd1f0f62bf2dc42e05d2adfb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2680916723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41d3f5654c52e69e21353e0c7b1b550e3748baf9d690b3b3b62577d8308f457`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:25:32 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:25:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:25:34 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:29:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:29:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:29:34 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:29:35 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41e7469900c0ac7da3620dfbe2f5cd1e281feb422d64cd58bf8825fd6c6fc4c`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1390950323f021776c3d0a461c28da38769b24c6eed4eb9911d044f5ae44cf`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5807586a9ff452b6e8d4ca9d2ef5ba4ffcc7751bd5b6ceab00e83e82f42c5d`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2689feedd974646a4ca3157295f3885b8e5da9d4c9c1f32314d35f70adf2a60`  
		Last Modified: Wed, 09 Dec 2020 23:51:59 GMT  
		Size: 290.0 MB (290034274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa53b1dd26ac111c77db9676e6092a5808d04a429c0f21356cc7ed84dec3c9f8`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481011d1197b79a1fa6ab6ac2b9bd74a88a91352e53ea72873cec54498c302a5`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8005529dbcf4218034a1ab1b1a72fc59b16f7c4f86376957b3c5f98dc48bc5c`  
		Last Modified: Wed, 09 Dec 2020 23:51:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:06948ffd05d9f106584a346f0ccf558b15d081979542ab33217020d1fd25af19
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6059632609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4045a03bcfca39fc002d6bfdcbb0a23d24c1149c29b2ddbe87961355eaa5613d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:29:44 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:29:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:29:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:34:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:34:26 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:34:27 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:34:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b951c1832bd371f29d7a9603e489724a320aa5b724c854bbfbf3bc18bc7434`  
		Last Modified: Wed, 09 Dec 2020 23:52:15 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e23c58b620021a4d59b2c9ce9dac475c122995ab1910f2528de8a3279c04f9e`  
		Last Modified: Wed, 09 Dec 2020 23:52:14 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5cbe21cc145247737842b2dd6988280e3d074f49c7ca2a7beaf3229417a039`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77884de364a9402818c45945edf6a2b6720eef409d764510eec7b6d554de4bee`  
		Last Modified: Wed, 09 Dec 2020 23:53:21 GMT  
		Size: 290.8 MB (290780591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8828745057dfdfbd30c1111fd3a25c5a274461910202a06c5a55f23fa2a5c7d`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f295aa5627a1d386769071decd61368f5ef72bfe35bf0beb96c2ad6c7777ec3`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37eb8760369bbfc74a9eb0873bd05d8761e93957f2e9cb55eb493d0e850c7220`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.11`

```console
$ docker pull mongo@sha256:793ff08818edee0ae6c0c0be8b0542ce5a8521671e3915ee7b67bdfed7bb9a4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.2.11` - linux; amd64

```console
$ docker pull mongo@sha256:890f506c2f919da36fb42d6a7de9874cc5d7adbe86a5e3b085e14ab39214d724
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165061323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511fe7789ae9bcedbe831171699aa524af2d4d3de37b5b7afdca74510c2a3d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:27:51 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 26 Nov 2020 01:27:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:27:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:27:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_MAJOR=4.2
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 26 Nov 2020 01:27:56 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:28:14 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:28:15 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:28:16 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:19 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:20 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b974c007ba520e60343cf372d76ee97bebb73b634e1a5e5936cb40e735cab`  
		Last Modified: Thu, 26 Nov 2020 01:29:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a6135ee562c5ce4407869bcbc6ed7d49517519277c55f6de2aac9dd00c9d6e`  
		Last Modified: Thu, 26 Nov 2020 01:30:00 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a5cbea1a515622883b9979af49f22b729488bf95873dd2aba3704100ce4d9d`  
		Last Modified: Thu, 26 Nov 2020 01:30:33 GMT  
		Size: 129.5 MB (129526094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9176a2e7afd6cfcde6349939b5d402049a11f7b1b4e53ed7306ea551483d0e05`  
		Last Modified: Thu, 26 Nov 2020 01:29:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b94f239e8a0dd7dd56508f1d94df3e0c1d066ace3a01f46c5dd612cf18c81e`  
		Last Modified: Fri, 11 Dec 2020 01:59:06 GMT  
		Size: 4.4 KB (4411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.11` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ce71251a85fdd9a4d93f45073f1ca55be867648e6187546ccf08cfee642d0624
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155046521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8309fe7dd97337eb1ba9d1e8ed4e18e3a19f617217d7f4c195ae3fbc78a7a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:43:45 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 25 Nov 2020 23:43:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:43:49 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:43:50 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:43:51 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:43:52 GMT
ENV MONGO_MAJOR=4.2
# Wed, 25 Nov 2020 23:43:53 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 25 Nov 2020 23:43:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:44:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:44:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:44:25 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:22 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:23 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:24 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244d5d8425ae8bd01528b5941f9d98e600443eeb7d1ef78f1f0569555fd89075`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05339f1902e2eff54eac65e727a1c398e7b51fd444661e28946229c1d57fcd4f`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8db58f0b3460af59d37fc0b84ad4cc8dedfe508211268c102f1a9718b4c65c`  
		Last Modified: Wed, 25 Nov 2020 23:47:28 GMT  
		Size: 123.3 MB (123275334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8cf676ac5fef9b9a7a315c81b8cc72ed78a78a13a52fe9b21491cfb4a062ff`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4741ed0d09dcf55d3516b68b2ddf4b63e0e970f028f5204ef142c434b51e85`  
		Last Modified: Wed, 13 Jan 2021 20:41:38 GMT  
		Size: 4.4 KB (4448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.11` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:dcefd7f962f48e6a4627c27ba97bd819f0f37e55cd1f0f62bf2dc42e05d2adfb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2680916723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41d3f5654c52e69e21353e0c7b1b550e3748baf9d690b3b3b62577d8308f457`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:25:32 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:25:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:25:34 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:29:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:29:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:29:34 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:29:35 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41e7469900c0ac7da3620dfbe2f5cd1e281feb422d64cd58bf8825fd6c6fc4c`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1390950323f021776c3d0a461c28da38769b24c6eed4eb9911d044f5ae44cf`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5807586a9ff452b6e8d4ca9d2ef5ba4ffcc7751bd5b6ceab00e83e82f42c5d`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2689feedd974646a4ca3157295f3885b8e5da9d4c9c1f32314d35f70adf2a60`  
		Last Modified: Wed, 09 Dec 2020 23:51:59 GMT  
		Size: 290.0 MB (290034274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa53b1dd26ac111c77db9676e6092a5808d04a429c0f21356cc7ed84dec3c9f8`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481011d1197b79a1fa6ab6ac2b9bd74a88a91352e53ea72873cec54498c302a5`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8005529dbcf4218034a1ab1b1a72fc59b16f7c4f86376957b3c5f98dc48bc5c`  
		Last Modified: Wed, 09 Dec 2020 23:51:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.11` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:06948ffd05d9f106584a346f0ccf558b15d081979542ab33217020d1fd25af19
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6059632609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4045a03bcfca39fc002d6bfdcbb0a23d24c1149c29b2ddbe87961355eaa5613d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:29:44 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:29:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:29:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:34:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:34:26 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:34:27 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:34:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b951c1832bd371f29d7a9603e489724a320aa5b724c854bbfbf3bc18bc7434`  
		Last Modified: Wed, 09 Dec 2020 23:52:15 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e23c58b620021a4d59b2c9ce9dac475c122995ab1910f2528de8a3279c04f9e`  
		Last Modified: Wed, 09 Dec 2020 23:52:14 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5cbe21cc145247737842b2dd6988280e3d074f49c7ca2a7beaf3229417a039`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77884de364a9402818c45945edf6a2b6720eef409d764510eec7b6d554de4bee`  
		Last Modified: Wed, 09 Dec 2020 23:53:21 GMT  
		Size: 290.8 MB (290780591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8828745057dfdfbd30c1111fd3a25c5a274461910202a06c5a55f23fa2a5c7d`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f295aa5627a1d386769071decd61368f5ef72bfe35bf0beb96c2ad6c7777ec3`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37eb8760369bbfc74a9eb0873bd05d8761e93957f2e9cb55eb493d0e850c7220`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.11-bionic`

```console
$ docker pull mongo@sha256:2de6f28468e78fe1f054d468f0cacba16792e2955ffbe977392ee46eba318ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2.11-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:890f506c2f919da36fb42d6a7de9874cc5d7adbe86a5e3b085e14ab39214d724
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165061323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511fe7789ae9bcedbe831171699aa524af2d4d3de37b5b7afdca74510c2a3d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:27:51 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 26 Nov 2020 01:27:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:27:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:27:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_MAJOR=4.2
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 26 Nov 2020 01:27:56 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:28:14 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:28:15 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:28:16 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:19 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:20 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b974c007ba520e60343cf372d76ee97bebb73b634e1a5e5936cb40e735cab`  
		Last Modified: Thu, 26 Nov 2020 01:29:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a6135ee562c5ce4407869bcbc6ed7d49517519277c55f6de2aac9dd00c9d6e`  
		Last Modified: Thu, 26 Nov 2020 01:30:00 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a5cbea1a515622883b9979af49f22b729488bf95873dd2aba3704100ce4d9d`  
		Last Modified: Thu, 26 Nov 2020 01:30:33 GMT  
		Size: 129.5 MB (129526094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9176a2e7afd6cfcde6349939b5d402049a11f7b1b4e53ed7306ea551483d0e05`  
		Last Modified: Thu, 26 Nov 2020 01:29:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b94f239e8a0dd7dd56508f1d94df3e0c1d066ace3a01f46c5dd612cf18c81e`  
		Last Modified: Fri, 11 Dec 2020 01:59:06 GMT  
		Size: 4.4 KB (4411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.11-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ce71251a85fdd9a4d93f45073f1ca55be867648e6187546ccf08cfee642d0624
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155046521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8309fe7dd97337eb1ba9d1e8ed4e18e3a19f617217d7f4c195ae3fbc78a7a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:43:45 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 25 Nov 2020 23:43:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:43:49 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:43:50 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:43:51 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:43:52 GMT
ENV MONGO_MAJOR=4.2
# Wed, 25 Nov 2020 23:43:53 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 25 Nov 2020 23:43:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:44:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:44:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:44:25 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:22 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:23 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:24 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244d5d8425ae8bd01528b5941f9d98e600443eeb7d1ef78f1f0569555fd89075`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05339f1902e2eff54eac65e727a1c398e7b51fd444661e28946229c1d57fcd4f`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8db58f0b3460af59d37fc0b84ad4cc8dedfe508211268c102f1a9718b4c65c`  
		Last Modified: Wed, 25 Nov 2020 23:47:28 GMT  
		Size: 123.3 MB (123275334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8cf676ac5fef9b9a7a315c81b8cc72ed78a78a13a52fe9b21491cfb4a062ff`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4741ed0d09dcf55d3516b68b2ddf4b63e0e970f028f5204ef142c434b51e85`  
		Last Modified: Wed, 13 Jan 2021 20:41:38 GMT  
		Size: 4.4 KB (4448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.11-windowsservercore`

```console
$ docker pull mongo@sha256:b813022f1cb9c38ae66557ddf99b2ac078094303ff6dca46debc271899b51902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.2.11-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:dcefd7f962f48e6a4627c27ba97bd819f0f37e55cd1f0f62bf2dc42e05d2adfb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2680916723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41d3f5654c52e69e21353e0c7b1b550e3748baf9d690b3b3b62577d8308f457`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:25:32 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:25:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:25:34 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:29:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:29:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:29:34 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:29:35 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41e7469900c0ac7da3620dfbe2f5cd1e281feb422d64cd58bf8825fd6c6fc4c`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1390950323f021776c3d0a461c28da38769b24c6eed4eb9911d044f5ae44cf`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5807586a9ff452b6e8d4ca9d2ef5ba4ffcc7751bd5b6ceab00e83e82f42c5d`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2689feedd974646a4ca3157295f3885b8e5da9d4c9c1f32314d35f70adf2a60`  
		Last Modified: Wed, 09 Dec 2020 23:51:59 GMT  
		Size: 290.0 MB (290034274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa53b1dd26ac111c77db9676e6092a5808d04a429c0f21356cc7ed84dec3c9f8`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481011d1197b79a1fa6ab6ac2b9bd74a88a91352e53ea72873cec54498c302a5`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8005529dbcf4218034a1ab1b1a72fc59b16f7c4f86376957b3c5f98dc48bc5c`  
		Last Modified: Wed, 09 Dec 2020 23:51:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.11-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:06948ffd05d9f106584a346f0ccf558b15d081979542ab33217020d1fd25af19
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6059632609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4045a03bcfca39fc002d6bfdcbb0a23d24c1149c29b2ddbe87961355eaa5613d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:29:44 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:29:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:29:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:34:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:34:26 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:34:27 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:34:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b951c1832bd371f29d7a9603e489724a320aa5b724c854bbfbf3bc18bc7434`  
		Last Modified: Wed, 09 Dec 2020 23:52:15 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e23c58b620021a4d59b2c9ce9dac475c122995ab1910f2528de8a3279c04f9e`  
		Last Modified: Wed, 09 Dec 2020 23:52:14 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5cbe21cc145247737842b2dd6988280e3d074f49c7ca2a7beaf3229417a039`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77884de364a9402818c45945edf6a2b6720eef409d764510eec7b6d554de4bee`  
		Last Modified: Wed, 09 Dec 2020 23:53:21 GMT  
		Size: 290.8 MB (290780591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8828745057dfdfbd30c1111fd3a25c5a274461910202a06c5a55f23fa2a5c7d`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f295aa5627a1d386769071decd61368f5ef72bfe35bf0beb96c2ad6c7777ec3`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37eb8760369bbfc74a9eb0873bd05d8761e93957f2e9cb55eb493d0e850c7220`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.11-windowsservercore-1809`

```console
$ docker pull mongo@sha256:9dac1f11dc50281968a25ceb02156d3e6f39528eed91ecfe5fe0513cd8898cc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:4.2.11-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:dcefd7f962f48e6a4627c27ba97bd819f0f37e55cd1f0f62bf2dc42e05d2adfb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2680916723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41d3f5654c52e69e21353e0c7b1b550e3748baf9d690b3b3b62577d8308f457`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:25:32 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:25:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:25:34 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:29:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:29:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:29:34 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:29:35 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41e7469900c0ac7da3620dfbe2f5cd1e281feb422d64cd58bf8825fd6c6fc4c`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1390950323f021776c3d0a461c28da38769b24c6eed4eb9911d044f5ae44cf`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5807586a9ff452b6e8d4ca9d2ef5ba4ffcc7751bd5b6ceab00e83e82f42c5d`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2689feedd974646a4ca3157295f3885b8e5da9d4c9c1f32314d35f70adf2a60`  
		Last Modified: Wed, 09 Dec 2020 23:51:59 GMT  
		Size: 290.0 MB (290034274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa53b1dd26ac111c77db9676e6092a5808d04a429c0f21356cc7ed84dec3c9f8`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481011d1197b79a1fa6ab6ac2b9bd74a88a91352e53ea72873cec54498c302a5`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8005529dbcf4218034a1ab1b1a72fc59b16f7c4f86376957b3c5f98dc48bc5c`  
		Last Modified: Wed, 09 Dec 2020 23:51:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.11-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:cda047e907222d713558e2be67e12ed0cfe42032e1ec22ed98f8faba2e321250
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.2.11-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:06948ffd05d9f106584a346f0ccf558b15d081979542ab33217020d1fd25af19
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6059632609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4045a03bcfca39fc002d6bfdcbb0a23d24c1149c29b2ddbe87961355eaa5613d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:29:44 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:29:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:29:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:34:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:34:26 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:34:27 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:34:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b951c1832bd371f29d7a9603e489724a320aa5b724c854bbfbf3bc18bc7434`  
		Last Modified: Wed, 09 Dec 2020 23:52:15 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e23c58b620021a4d59b2c9ce9dac475c122995ab1910f2528de8a3279c04f9e`  
		Last Modified: Wed, 09 Dec 2020 23:52:14 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5cbe21cc145247737842b2dd6988280e3d074f49c7ca2a7beaf3229417a039`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77884de364a9402818c45945edf6a2b6720eef409d764510eec7b6d554de4bee`  
		Last Modified: Wed, 09 Dec 2020 23:53:21 GMT  
		Size: 290.8 MB (290780591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8828745057dfdfbd30c1111fd3a25c5a274461910202a06c5a55f23fa2a5c7d`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f295aa5627a1d386769071decd61368f5ef72bfe35bf0beb96c2ad6c7777ec3`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37eb8760369bbfc74a9eb0873bd05d8761e93957f2e9cb55eb493d0e850c7220`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:2de6f28468e78fe1f054d468f0cacba16792e2955ffbe977392ee46eba318ea1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:890f506c2f919da36fb42d6a7de9874cc5d7adbe86a5e3b085e14ab39214d724
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.1 MB (165061323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511fe7789ae9bcedbe831171699aa524af2d4d3de37b5b7afdca74510c2a3d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:27:51 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 26 Nov 2020 01:27:54 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:27:54 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:27:55 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_MAJOR=4.2
# Thu, 26 Nov 2020 01:27:55 GMT
ENV MONGO_VERSION=4.2.11
# Thu, 26 Nov 2020 01:27:56 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 26 Nov 2020 01:28:14 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 26 Nov 2020 01:28:15 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 26 Nov 2020 01:28:16 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Dec 2020 01:58:19 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Fri, 11 Dec 2020 01:58:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 01:58:20 GMT
EXPOSE 27017
# Fri, 11 Dec 2020 01:58:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441b974c007ba520e60343cf372d76ee97bebb73b634e1a5e5936cb40e735cab`  
		Last Modified: Thu, 26 Nov 2020 01:29:59 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a6135ee562c5ce4407869bcbc6ed7d49517519277c55f6de2aac9dd00c9d6e`  
		Last Modified: Thu, 26 Nov 2020 01:30:00 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a5cbea1a515622883b9979af49f22b729488bf95873dd2aba3704100ce4d9d`  
		Last Modified: Thu, 26 Nov 2020 01:30:33 GMT  
		Size: 129.5 MB (129526094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9176a2e7afd6cfcde6349939b5d402049a11f7b1b4e53ed7306ea551483d0e05`  
		Last Modified: Thu, 26 Nov 2020 01:29:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b94f239e8a0dd7dd56508f1d94df3e0c1d066ace3a01f46c5dd612cf18c81e`  
		Last Modified: Fri, 11 Dec 2020 01:59:06 GMT  
		Size: 4.4 KB (4411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ce71251a85fdd9a4d93f45073f1ca55be867648e6187546ccf08cfee642d0624
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155046521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d8309fe7dd97337eb1ba9d1e8ed4e18e3a19f617217d7f4c195ae3fbc78a7a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:43:45 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 25 Nov 2020 23:43:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:43:49 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:43:50 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:43:51 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:43:52 GMT
ENV MONGO_MAJOR=4.2
# Wed, 25 Nov 2020 23:43:53 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 25 Nov 2020 23:43:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 25 Nov 2020 23:44:20 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 25 Nov 2020 23:44:24 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 25 Nov 2020 23:44:25 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:22 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:23 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:24 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244d5d8425ae8bd01528b5941f9d98e600443eeb7d1ef78f1f0569555fd89075`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05339f1902e2eff54eac65e727a1c398e7b51fd444661e28946229c1d57fcd4f`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8db58f0b3460af59d37fc0b84ad4cc8dedfe508211268c102f1a9718b4c65c`  
		Last Modified: Wed, 25 Nov 2020 23:47:28 GMT  
		Size: 123.3 MB (123275334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8cf676ac5fef9b9a7a315c81b8cc72ed78a78a13a52fe9b21491cfb4a062ff`  
		Last Modified: Wed, 25 Nov 2020 23:47:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4741ed0d09dcf55d3516b68b2ddf4b63e0e970f028f5204ef142c434b51e85`  
		Last Modified: Wed, 13 Jan 2021 20:41:38 GMT  
		Size: 4.4 KB (4448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:b813022f1cb9c38ae66557ddf99b2ac078094303ff6dca46debc271899b51902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:dcefd7f962f48e6a4627c27ba97bd819f0f37e55cd1f0f62bf2dc42e05d2adfb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2680916723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41d3f5654c52e69e21353e0c7b1b550e3748baf9d690b3b3b62577d8308f457`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:25:32 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:25:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:25:34 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:29:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:29:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:29:34 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:29:35 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41e7469900c0ac7da3620dfbe2f5cd1e281feb422d64cd58bf8825fd6c6fc4c`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1390950323f021776c3d0a461c28da38769b24c6eed4eb9911d044f5ae44cf`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5807586a9ff452b6e8d4ca9d2ef5ba4ffcc7751bd5b6ceab00e83e82f42c5d`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2689feedd974646a4ca3157295f3885b8e5da9d4c9c1f32314d35f70adf2a60`  
		Last Modified: Wed, 09 Dec 2020 23:51:59 GMT  
		Size: 290.0 MB (290034274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa53b1dd26ac111c77db9676e6092a5808d04a429c0f21356cc7ed84dec3c9f8`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481011d1197b79a1fa6ab6ac2b9bd74a88a91352e53ea72873cec54498c302a5`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8005529dbcf4218034a1ab1b1a72fc59b16f7c4f86376957b3c5f98dc48bc5c`  
		Last Modified: Wed, 09 Dec 2020 23:51:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:06948ffd05d9f106584a346f0ccf558b15d081979542ab33217020d1fd25af19
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6059632609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4045a03bcfca39fc002d6bfdcbb0a23d24c1149c29b2ddbe87961355eaa5613d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:29:44 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:29:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:29:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:34:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:34:26 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:34:27 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:34:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b951c1832bd371f29d7a9603e489724a320aa5b724c854bbfbf3bc18bc7434`  
		Last Modified: Wed, 09 Dec 2020 23:52:15 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e23c58b620021a4d59b2c9ce9dac475c122995ab1910f2528de8a3279c04f9e`  
		Last Modified: Wed, 09 Dec 2020 23:52:14 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5cbe21cc145247737842b2dd6988280e3d074f49c7ca2a7beaf3229417a039`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77884de364a9402818c45945edf6a2b6720eef409d764510eec7b6d554de4bee`  
		Last Modified: Wed, 09 Dec 2020 23:53:21 GMT  
		Size: 290.8 MB (290780591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8828745057dfdfbd30c1111fd3a25c5a274461910202a06c5a55f23fa2a5c7d`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f295aa5627a1d386769071decd61368f5ef72bfe35bf0beb96c2ad6c7777ec3`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37eb8760369bbfc74a9eb0873bd05d8761e93957f2e9cb55eb493d0e850c7220`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:9dac1f11dc50281968a25ceb02156d3e6f39528eed91ecfe5fe0513cd8898cc0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:dcefd7f962f48e6a4627c27ba97bd819f0f37e55cd1f0f62bf2dc42e05d2adfb
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2680916723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41d3f5654c52e69e21353e0c7b1b550e3748baf9d690b3b3b62577d8308f457`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:25:32 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:25:33 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:25:34 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:29:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:29:33 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:29:34 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:29:35 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41e7469900c0ac7da3620dfbe2f5cd1e281feb422d64cd58bf8825fd6c6fc4c`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1390950323f021776c3d0a461c28da38769b24c6eed4eb9911d044f5ae44cf`  
		Last Modified: Wed, 09 Dec 2020 23:51:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5807586a9ff452b6e8d4ca9d2ef5ba4ffcc7751bd5b6ceab00e83e82f42c5d`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2689feedd974646a4ca3157295f3885b8e5da9d4c9c1f32314d35f70adf2a60`  
		Last Modified: Wed, 09 Dec 2020 23:51:59 GMT  
		Size: 290.0 MB (290034274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa53b1dd26ac111c77db9676e6092a5808d04a429c0f21356cc7ed84dec3c9f8`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481011d1197b79a1fa6ab6ac2b9bd74a88a91352e53ea72873cec54498c302a5`  
		Last Modified: Wed, 09 Dec 2020 23:51:02 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8005529dbcf4218034a1ab1b1a72fc59b16f7c4f86376957b3c5f98dc48bc5c`  
		Last Modified: Wed, 09 Dec 2020 23:51:03 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:cda047e907222d713558e2be67e12ed0cfe42032e1ec22ed98f8faba2e321250
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:06948ffd05d9f106584a346f0ccf558b15d081979542ab33217020d1fd25af19
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6059632609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4045a03bcfca39fc002d6bfdcbb0a23d24c1149c29b2ddbe87961355eaa5613d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Dec 2020 23:29:44 GMT
ENV MONGO_VERSION=4.2.11
# Wed, 09 Dec 2020 23:29:45 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.11-signed.msi
# Wed, 09 Dec 2020 23:29:46 GMT
ENV MONGO_DOWNLOAD_SHA256=e8f60257d6f556225e085a8e5d0e33d78f16aaf97d421e4e565a7e96dd07d1ef
# Wed, 09 Dec 2020 23:34:25 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools,MonitoringTools,ImportExportTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Dec 2020 23:34:26 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Dec 2020 23:34:27 GMT
EXPOSE 27017
# Wed, 09 Dec 2020 23:34:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b951c1832bd371f29d7a9603e489724a320aa5b724c854bbfbf3bc18bc7434`  
		Last Modified: Wed, 09 Dec 2020 23:52:15 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e23c58b620021a4d59b2c9ce9dac475c122995ab1910f2528de8a3279c04f9e`  
		Last Modified: Wed, 09 Dec 2020 23:52:14 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5cbe21cc145247737842b2dd6988280e3d074f49c7ca2a7beaf3229417a039`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77884de364a9402818c45945edf6a2b6720eef409d764510eec7b6d554de4bee`  
		Last Modified: Wed, 09 Dec 2020 23:53:21 GMT  
		Size: 290.8 MB (290780591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8828745057dfdfbd30c1111fd3a25c5a274461910202a06c5a55f23fa2a5c7d`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f295aa5627a1d386769071decd61368f5ef72bfe35bf0beb96c2ad6c7777ec3`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37eb8760369bbfc74a9eb0873bd05d8761e93957f2e9cb55eb493d0e850c7220`  
		Last Modified: Wed, 09 Dec 2020 23:52:11 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4`

```console
$ docker pull mongo@sha256:094f04532c279cb96da991692896e5a013939e2471e4a98791aa5cd7a196981c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.4` - linux; amd64

```console
$ docker pull mongo@sha256:c46e1f6dd8ac3f8592b53fa2dfdc0f7e26055929e6bf30975838ca0406c5bc2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178220204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97feb3412a387d4d3bbd8653b09ef26683263a192e0e8dc6554e65bfb637a86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:28:23 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 01:28:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:28:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:28:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:20:44 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:20:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:21:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:21:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:21:11 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:21:11 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:21:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:21:12 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:21:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e4e43cb0003675e06e2e17e30cb17e0e9a990abc8a107f259c93be84ccc4f`  
		Last Modified: Thu, 26 Nov 2020 01:30:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50e71d834e14ca61531dcce8e5e52860ea3b03769e5e68cf77ac07e941f6d6`  
		Last Modified: Mon, 04 Jan 2021 22:22:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27768a0d0c674b5175f704d585df68ad33f9bd5be976bd669801075e8ca63526`  
		Last Modified: Mon, 04 Jan 2021 22:22:36 GMT  
		Size: 142.7 MB (142684977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4e0bd8b992a6db5b94cd268f50463e33f8a470bd7b8b3772a177714ce8ccd7`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c887415d06431f09f31175932c083142d41a7de019c848489c1e5412e4b14635`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:66fd4f8f09e92de8744c76702e836f0fc5831255318373435935bc3d589b5f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168150811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25db05811c760dc9c9ba32746c241a6e8a67669179651b91931ba04adf1076d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:44:48 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 25 Nov 2020 23:44:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:44:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:44:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:56 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:43:16 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:43:19 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:43:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:31 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:32 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4913f11c494a00e3d77d01b9364c56f69482ffaeddf32e87f424acd659acff9`  
		Last Modified: Wed, 25 Nov 2020 23:47:35 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17fffdaae13eded3257e5cef69f19565cb07b9602919924393e099e88d56ab9`  
		Last Modified: Mon, 04 Jan 2021 22:44:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c65f20a6385ac5b1be7e719820d32fe6d98175958ee48624f07341afba641aa`  
		Last Modified: Mon, 04 Jan 2021 22:45:23 GMT  
		Size: 136.4 MB (136379637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0fec39db28299b0b7d33a9a2f3a99f3bd9c0cc78ac9190d5c5a33f780ae566`  
		Last Modified: Mon, 04 Jan 2021 22:44:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7c251da439065584411bea56b6288812cbae60767613397e8960289dceaeed`  
		Last Modified: Wed, 13 Jan 2021 20:41:45 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; s390x

```console
$ docker pull mongo@sha256:543de10da111411668affef0a4572320b1a53aad1afd2fd2fec58b4de13cadb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173130142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f718506b8817f58d5917d2b4c2b344ffda20b91739e3701d5b277100d7a8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:54 GMT
ADD file:aa0063276274c9f3ba9308c3cdfd911449966c87546f28ceb3122d6fbd995d52 in / 
# Wed, 25 Nov 2020 22:45:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:07:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 00:08:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:08:17 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 00:08:18 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 00:08:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 00:08:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 00:08:44 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 00:08:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 00:08:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 00:08:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:41:47 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:41:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:11 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:41:41 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:41:42 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:41:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2269433521a3f2e95508abd4fa29a3de21226eed5a09ad3959a689b066151bca`  
		Last Modified: Mon, 23 Nov 2020 18:41:52 GMT  
		Size: 25.4 MB (25381722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442687b9aa7dcd6b97d4f9ce9562774788922b94571cd3a7ea85185cd76cbd3`  
		Last Modified: Wed, 25 Nov 2020 22:47:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6efa602a92c53f638f3667fa4400f2fdb32c5aaae3d112e33f15a12cb2bb3b`  
		Last Modified: Wed, 25 Nov 2020 22:47:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a5fb2071960493a99805bac4506cb07225b998113d5ae9b344509442f9e542`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8d2ce236c235c465ef891cd59df829a91e12d07301f95cdc23d077c44d81a`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 2.7 MB (2720968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ce7bbcb36617017b697c1cedd0f4dad2273643f9315dcb5665c9731e031b3`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 5.7 MB (5746421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621599eddf8a561bdfb15886b7a9609c02a01369e9bd02c9937cdaa7b3ccc212`  
		Last Modified: Thu, 26 Nov 2020 00:10:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0760577d520065d34f4c5a7340b154a10776867a6448a2f6a8692ffe23ea21e`  
		Last Modified: Thu, 26 Nov 2020 00:10:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd26d3d155865f99e5f9f9cc78acd78b78951980e96b704a3d6fc62125f266`  
		Last Modified: Mon, 04 Jan 2021 22:43:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b55cdba3dc093e0f2f23a688d26ebfd23bcbda7c077566297ac179280a6568`  
		Last Modified: Mon, 04 Jan 2021 22:43:51 GMT  
		Size: 139.3 MB (139271674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0584912549af62baba56b0311441340f5a45f758f1c3a96d739b4ca98eb7a8`  
		Last Modified: Mon, 04 Jan 2021 22:43:30 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b0b7d81cfea5fa13c01706f15f9a99a732d4faa0ab0b3637fd26fccd72864`  
		Last Modified: Wed, 13 Jan 2021 20:42:29 GMT  
		Size: 4.5 KB (4450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3`

```console
$ docker pull mongo@sha256:094f04532c279cb96da991692896e5a013939e2471e4a98791aa5cd7a196981c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.4.3` - linux; amd64

```console
$ docker pull mongo@sha256:c46e1f6dd8ac3f8592b53fa2dfdc0f7e26055929e6bf30975838ca0406c5bc2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178220204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97feb3412a387d4d3bbd8653b09ef26683263a192e0e8dc6554e65bfb637a86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:28:23 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 01:28:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:28:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:28:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:20:44 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:20:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:21:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:21:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:21:11 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:21:11 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:21:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:21:12 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:21:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e4e43cb0003675e06e2e17e30cb17e0e9a990abc8a107f259c93be84ccc4f`  
		Last Modified: Thu, 26 Nov 2020 01:30:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50e71d834e14ca61531dcce8e5e52860ea3b03769e5e68cf77ac07e941f6d6`  
		Last Modified: Mon, 04 Jan 2021 22:22:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27768a0d0c674b5175f704d585df68ad33f9bd5be976bd669801075e8ca63526`  
		Last Modified: Mon, 04 Jan 2021 22:22:36 GMT  
		Size: 142.7 MB (142684977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4e0bd8b992a6db5b94cd268f50463e33f8a470bd7b8b3772a177714ce8ccd7`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c887415d06431f09f31175932c083142d41a7de019c848489c1e5412e4b14635`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:66fd4f8f09e92de8744c76702e836f0fc5831255318373435935bc3d589b5f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168150811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25db05811c760dc9c9ba32746c241a6e8a67669179651b91931ba04adf1076d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:44:48 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 25 Nov 2020 23:44:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:44:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:44:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:56 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:43:16 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:43:19 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:43:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:31 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:32 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4913f11c494a00e3d77d01b9364c56f69482ffaeddf32e87f424acd659acff9`  
		Last Modified: Wed, 25 Nov 2020 23:47:35 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17fffdaae13eded3257e5cef69f19565cb07b9602919924393e099e88d56ab9`  
		Last Modified: Mon, 04 Jan 2021 22:44:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c65f20a6385ac5b1be7e719820d32fe6d98175958ee48624f07341afba641aa`  
		Last Modified: Mon, 04 Jan 2021 22:45:23 GMT  
		Size: 136.4 MB (136379637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0fec39db28299b0b7d33a9a2f3a99f3bd9c0cc78ac9190d5c5a33f780ae566`  
		Last Modified: Mon, 04 Jan 2021 22:44:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7c251da439065584411bea56b6288812cbae60767613397e8960289dceaeed`  
		Last Modified: Wed, 13 Jan 2021 20:41:45 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3` - linux; s390x

```console
$ docker pull mongo@sha256:543de10da111411668affef0a4572320b1a53aad1afd2fd2fec58b4de13cadb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173130142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f718506b8817f58d5917d2b4c2b344ffda20b91739e3701d5b277100d7a8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:54 GMT
ADD file:aa0063276274c9f3ba9308c3cdfd911449966c87546f28ceb3122d6fbd995d52 in / 
# Wed, 25 Nov 2020 22:45:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:07:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 00:08:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:08:17 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 00:08:18 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 00:08:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 00:08:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 00:08:44 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 00:08:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 00:08:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 00:08:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:41:47 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:41:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:11 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:41:41 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:41:42 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:41:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2269433521a3f2e95508abd4fa29a3de21226eed5a09ad3959a689b066151bca`  
		Last Modified: Mon, 23 Nov 2020 18:41:52 GMT  
		Size: 25.4 MB (25381722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442687b9aa7dcd6b97d4f9ce9562774788922b94571cd3a7ea85185cd76cbd3`  
		Last Modified: Wed, 25 Nov 2020 22:47:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6efa602a92c53f638f3667fa4400f2fdb32c5aaae3d112e33f15a12cb2bb3b`  
		Last Modified: Wed, 25 Nov 2020 22:47:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a5fb2071960493a99805bac4506cb07225b998113d5ae9b344509442f9e542`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8d2ce236c235c465ef891cd59df829a91e12d07301f95cdc23d077c44d81a`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 2.7 MB (2720968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ce7bbcb36617017b697c1cedd0f4dad2273643f9315dcb5665c9731e031b3`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 5.7 MB (5746421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621599eddf8a561bdfb15886b7a9609c02a01369e9bd02c9937cdaa7b3ccc212`  
		Last Modified: Thu, 26 Nov 2020 00:10:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0760577d520065d34f4c5a7340b154a10776867a6448a2f6a8692ffe23ea21e`  
		Last Modified: Thu, 26 Nov 2020 00:10:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd26d3d155865f99e5f9f9cc78acd78b78951980e96b704a3d6fc62125f266`  
		Last Modified: Mon, 04 Jan 2021 22:43:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b55cdba3dc093e0f2f23a688d26ebfd23bcbda7c077566297ac179280a6568`  
		Last Modified: Mon, 04 Jan 2021 22:43:51 GMT  
		Size: 139.3 MB (139271674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0584912549af62baba56b0311441340f5a45f758f1c3a96d739b4ca98eb7a8`  
		Last Modified: Mon, 04 Jan 2021 22:43:30 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b0b7d81cfea5fa13c01706f15f9a99a732d4faa0ab0b3637fd26fccd72864`  
		Last Modified: Wed, 13 Jan 2021 20:42:29 GMT  
		Size: 4.5 KB (4450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3-bionic`

```console
$ docker pull mongo@sha256:c9b0f40151cd56721707c875677b6df0805d406aeade0ffa52c072273c39a9cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4.3-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:c46e1f6dd8ac3f8592b53fa2dfdc0f7e26055929e6bf30975838ca0406c5bc2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178220204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97feb3412a387d4d3bbd8653b09ef26683263a192e0e8dc6554e65bfb637a86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:28:23 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 01:28:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:28:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:28:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:20:44 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:20:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:21:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:21:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:21:11 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:21:11 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:21:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:21:12 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:21:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e4e43cb0003675e06e2e17e30cb17e0e9a990abc8a107f259c93be84ccc4f`  
		Last Modified: Thu, 26 Nov 2020 01:30:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50e71d834e14ca61531dcce8e5e52860ea3b03769e5e68cf77ac07e941f6d6`  
		Last Modified: Mon, 04 Jan 2021 22:22:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27768a0d0c674b5175f704d585df68ad33f9bd5be976bd669801075e8ca63526`  
		Last Modified: Mon, 04 Jan 2021 22:22:36 GMT  
		Size: 142.7 MB (142684977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4e0bd8b992a6db5b94cd268f50463e33f8a470bd7b8b3772a177714ce8ccd7`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c887415d06431f09f31175932c083142d41a7de019c848489c1e5412e4b14635`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:66fd4f8f09e92de8744c76702e836f0fc5831255318373435935bc3d589b5f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168150811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25db05811c760dc9c9ba32746c241a6e8a67669179651b91931ba04adf1076d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:44:48 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 25 Nov 2020 23:44:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:44:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:44:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:56 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:43:16 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:43:19 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:43:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:31 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:32 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4913f11c494a00e3d77d01b9364c56f69482ffaeddf32e87f424acd659acff9`  
		Last Modified: Wed, 25 Nov 2020 23:47:35 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17fffdaae13eded3257e5cef69f19565cb07b9602919924393e099e88d56ab9`  
		Last Modified: Mon, 04 Jan 2021 22:44:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c65f20a6385ac5b1be7e719820d32fe6d98175958ee48624f07341afba641aa`  
		Last Modified: Mon, 04 Jan 2021 22:45:23 GMT  
		Size: 136.4 MB (136379637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0fec39db28299b0b7d33a9a2f3a99f3bd9c0cc78ac9190d5c5a33f780ae566`  
		Last Modified: Mon, 04 Jan 2021 22:44:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7c251da439065584411bea56b6288812cbae60767613397e8960289dceaeed`  
		Last Modified: Wed, 13 Jan 2021 20:41:45 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:543de10da111411668affef0a4572320b1a53aad1afd2fd2fec58b4de13cadb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173130142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f718506b8817f58d5917d2b4c2b344ffda20b91739e3701d5b277100d7a8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:54 GMT
ADD file:aa0063276274c9f3ba9308c3cdfd911449966c87546f28ceb3122d6fbd995d52 in / 
# Wed, 25 Nov 2020 22:45:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:07:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 00:08:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:08:17 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 00:08:18 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 00:08:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 00:08:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 00:08:44 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 00:08:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 00:08:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 00:08:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:41:47 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:41:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:11 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:41:41 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:41:42 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:41:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2269433521a3f2e95508abd4fa29a3de21226eed5a09ad3959a689b066151bca`  
		Last Modified: Mon, 23 Nov 2020 18:41:52 GMT  
		Size: 25.4 MB (25381722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442687b9aa7dcd6b97d4f9ce9562774788922b94571cd3a7ea85185cd76cbd3`  
		Last Modified: Wed, 25 Nov 2020 22:47:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6efa602a92c53f638f3667fa4400f2fdb32c5aaae3d112e33f15a12cb2bb3b`  
		Last Modified: Wed, 25 Nov 2020 22:47:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a5fb2071960493a99805bac4506cb07225b998113d5ae9b344509442f9e542`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8d2ce236c235c465ef891cd59df829a91e12d07301f95cdc23d077c44d81a`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 2.7 MB (2720968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ce7bbcb36617017b697c1cedd0f4dad2273643f9315dcb5665c9731e031b3`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 5.7 MB (5746421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621599eddf8a561bdfb15886b7a9609c02a01369e9bd02c9937cdaa7b3ccc212`  
		Last Modified: Thu, 26 Nov 2020 00:10:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0760577d520065d34f4c5a7340b154a10776867a6448a2f6a8692ffe23ea21e`  
		Last Modified: Thu, 26 Nov 2020 00:10:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd26d3d155865f99e5f9f9cc78acd78b78951980e96b704a3d6fc62125f266`  
		Last Modified: Mon, 04 Jan 2021 22:43:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b55cdba3dc093e0f2f23a688d26ebfd23bcbda7c077566297ac179280a6568`  
		Last Modified: Mon, 04 Jan 2021 22:43:51 GMT  
		Size: 139.3 MB (139271674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0584912549af62baba56b0311441340f5a45f758f1c3a96d739b4ca98eb7a8`  
		Last Modified: Mon, 04 Jan 2021 22:43:30 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b0b7d81cfea5fa13c01706f15f9a99a732d4faa0ab0b3637fd26fccd72864`  
		Last Modified: Wed, 13 Jan 2021 20:42:29 GMT  
		Size: 4.5 KB (4450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3-windowsservercore`

```console
$ docker pull mongo@sha256:ec3ea97c48dedf9707ec201072abde21fa34708c1f706781bb202916b97c64f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.4.3-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.3-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0d8e5d81f217e4c15a4155e19e0767d448d75f8274a0750941e7a13dc2a01aa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:4.4.3-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:7a3b42dd7e569fb530a7418a7b26420b7cca13c896e44ef7f77a34698a4bcef4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.4.3-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-bionic`

```console
$ docker pull mongo@sha256:c9b0f40151cd56721707c875677b6df0805d406aeade0ffa52c072273c39a9cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:c46e1f6dd8ac3f8592b53fa2dfdc0f7e26055929e6bf30975838ca0406c5bc2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178220204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97feb3412a387d4d3bbd8653b09ef26683263a192e0e8dc6554e65bfb637a86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:28:23 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 01:28:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:28:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:28:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:20:44 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:20:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:21:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:21:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:21:11 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:21:11 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:21:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:21:12 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:21:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e4e43cb0003675e06e2e17e30cb17e0e9a990abc8a107f259c93be84ccc4f`  
		Last Modified: Thu, 26 Nov 2020 01:30:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50e71d834e14ca61531dcce8e5e52860ea3b03769e5e68cf77ac07e941f6d6`  
		Last Modified: Mon, 04 Jan 2021 22:22:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27768a0d0c674b5175f704d585df68ad33f9bd5be976bd669801075e8ca63526`  
		Last Modified: Mon, 04 Jan 2021 22:22:36 GMT  
		Size: 142.7 MB (142684977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4e0bd8b992a6db5b94cd268f50463e33f8a470bd7b8b3772a177714ce8ccd7`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c887415d06431f09f31175932c083142d41a7de019c848489c1e5412e4b14635`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:66fd4f8f09e92de8744c76702e836f0fc5831255318373435935bc3d589b5f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168150811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25db05811c760dc9c9ba32746c241a6e8a67669179651b91931ba04adf1076d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:44:48 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 25 Nov 2020 23:44:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:44:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:44:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:56 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:43:16 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:43:19 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:43:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:31 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:32 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4913f11c494a00e3d77d01b9364c56f69482ffaeddf32e87f424acd659acff9`  
		Last Modified: Wed, 25 Nov 2020 23:47:35 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17fffdaae13eded3257e5cef69f19565cb07b9602919924393e099e88d56ab9`  
		Last Modified: Mon, 04 Jan 2021 22:44:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c65f20a6385ac5b1be7e719820d32fe6d98175958ee48624f07341afba641aa`  
		Last Modified: Mon, 04 Jan 2021 22:45:23 GMT  
		Size: 136.4 MB (136379637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0fec39db28299b0b7d33a9a2f3a99f3bd9c0cc78ac9190d5c5a33f780ae566`  
		Last Modified: Mon, 04 Jan 2021 22:44:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7c251da439065584411bea56b6288812cbae60767613397e8960289dceaeed`  
		Last Modified: Wed, 13 Jan 2021 20:41:45 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:543de10da111411668affef0a4572320b1a53aad1afd2fd2fec58b4de13cadb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173130142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f718506b8817f58d5917d2b4c2b344ffda20b91739e3701d5b277100d7a8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:54 GMT
ADD file:aa0063276274c9f3ba9308c3cdfd911449966c87546f28ceb3122d6fbd995d52 in / 
# Wed, 25 Nov 2020 22:45:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:07:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 00:08:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:08:17 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 00:08:18 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 00:08:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 00:08:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 00:08:44 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 00:08:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 00:08:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 00:08:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:41:47 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:41:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:11 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:41:41 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:41:42 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:41:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2269433521a3f2e95508abd4fa29a3de21226eed5a09ad3959a689b066151bca`  
		Last Modified: Mon, 23 Nov 2020 18:41:52 GMT  
		Size: 25.4 MB (25381722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442687b9aa7dcd6b97d4f9ce9562774788922b94571cd3a7ea85185cd76cbd3`  
		Last Modified: Wed, 25 Nov 2020 22:47:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6efa602a92c53f638f3667fa4400f2fdb32c5aaae3d112e33f15a12cb2bb3b`  
		Last Modified: Wed, 25 Nov 2020 22:47:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a5fb2071960493a99805bac4506cb07225b998113d5ae9b344509442f9e542`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8d2ce236c235c465ef891cd59df829a91e12d07301f95cdc23d077c44d81a`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 2.7 MB (2720968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ce7bbcb36617017b697c1cedd0f4dad2273643f9315dcb5665c9731e031b3`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 5.7 MB (5746421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621599eddf8a561bdfb15886b7a9609c02a01369e9bd02c9937cdaa7b3ccc212`  
		Last Modified: Thu, 26 Nov 2020 00:10:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0760577d520065d34f4c5a7340b154a10776867a6448a2f6a8692ffe23ea21e`  
		Last Modified: Thu, 26 Nov 2020 00:10:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd26d3d155865f99e5f9f9cc78acd78b78951980e96b704a3d6fc62125f266`  
		Last Modified: Mon, 04 Jan 2021 22:43:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b55cdba3dc093e0f2f23a688d26ebfd23bcbda7c077566297ac179280a6568`  
		Last Modified: Mon, 04 Jan 2021 22:43:51 GMT  
		Size: 139.3 MB (139271674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0584912549af62baba56b0311441340f5a45f758f1c3a96d739b4ca98eb7a8`  
		Last Modified: Mon, 04 Jan 2021 22:43:30 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b0b7d81cfea5fa13c01706f15f9a99a732d4faa0ab0b3637fd26fccd72864`  
		Last Modified: Wed, 13 Jan 2021 20:42:29 GMT  
		Size: 4.5 KB (4450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore`

```console
$ docker pull mongo@sha256:ec3ea97c48dedf9707ec201072abde21fa34708c1f706781bb202916b97c64f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.4-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0d8e5d81f217e4c15a4155e19e0767d448d75f8274a0750941e7a13dc2a01aa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:4.4-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:7a3b42dd7e569fb530a7418a7b26420b7cca13c896e44ef7f77a34698a4bcef4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:4.4-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:c9b0f40151cd56721707c875677b6df0805d406aeade0ffa52c072273c39a9cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:c46e1f6dd8ac3f8592b53fa2dfdc0f7e26055929e6bf30975838ca0406c5bc2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178220204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97feb3412a387d4d3bbd8653b09ef26683263a192e0e8dc6554e65bfb637a86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:28:23 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 01:28:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:28:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:28:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:20:44 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:20:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:21:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:21:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:21:11 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:21:11 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:21:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:21:12 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:21:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e4e43cb0003675e06e2e17e30cb17e0e9a990abc8a107f259c93be84ccc4f`  
		Last Modified: Thu, 26 Nov 2020 01:30:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50e71d834e14ca61531dcce8e5e52860ea3b03769e5e68cf77ac07e941f6d6`  
		Last Modified: Mon, 04 Jan 2021 22:22:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27768a0d0c674b5175f704d585df68ad33f9bd5be976bd669801075e8ca63526`  
		Last Modified: Mon, 04 Jan 2021 22:22:36 GMT  
		Size: 142.7 MB (142684977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4e0bd8b992a6db5b94cd268f50463e33f8a470bd7b8b3772a177714ce8ccd7`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c887415d06431f09f31175932c083142d41a7de019c848489c1e5412e4b14635`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:66fd4f8f09e92de8744c76702e836f0fc5831255318373435935bc3d589b5f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168150811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25db05811c760dc9c9ba32746c241a6e8a67669179651b91931ba04adf1076d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:44:48 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 25 Nov 2020 23:44:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:44:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:44:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:56 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:43:16 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:43:19 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:43:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:31 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:32 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4913f11c494a00e3d77d01b9364c56f69482ffaeddf32e87f424acd659acff9`  
		Last Modified: Wed, 25 Nov 2020 23:47:35 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17fffdaae13eded3257e5cef69f19565cb07b9602919924393e099e88d56ab9`  
		Last Modified: Mon, 04 Jan 2021 22:44:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c65f20a6385ac5b1be7e719820d32fe6d98175958ee48624f07341afba641aa`  
		Last Modified: Mon, 04 Jan 2021 22:45:23 GMT  
		Size: 136.4 MB (136379637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0fec39db28299b0b7d33a9a2f3a99f3bd9c0cc78ac9190d5c5a33f780ae566`  
		Last Modified: Mon, 04 Jan 2021 22:44:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7c251da439065584411bea56b6288812cbae60767613397e8960289dceaeed`  
		Last Modified: Wed, 13 Jan 2021 20:41:45 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:543de10da111411668affef0a4572320b1a53aad1afd2fd2fec58b4de13cadb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173130142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f718506b8817f58d5917d2b4c2b344ffda20b91739e3701d5b277100d7a8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:54 GMT
ADD file:aa0063276274c9f3ba9308c3cdfd911449966c87546f28ceb3122d6fbd995d52 in / 
# Wed, 25 Nov 2020 22:45:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:07:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 00:08:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:08:17 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 00:08:18 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 00:08:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 00:08:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 00:08:44 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 00:08:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 00:08:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 00:08:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:41:47 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:41:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:11 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:41:41 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:41:42 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:41:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2269433521a3f2e95508abd4fa29a3de21226eed5a09ad3959a689b066151bca`  
		Last Modified: Mon, 23 Nov 2020 18:41:52 GMT  
		Size: 25.4 MB (25381722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442687b9aa7dcd6b97d4f9ce9562774788922b94571cd3a7ea85185cd76cbd3`  
		Last Modified: Wed, 25 Nov 2020 22:47:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6efa602a92c53f638f3667fa4400f2fdb32c5aaae3d112e33f15a12cb2bb3b`  
		Last Modified: Wed, 25 Nov 2020 22:47:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a5fb2071960493a99805bac4506cb07225b998113d5ae9b344509442f9e542`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8d2ce236c235c465ef891cd59df829a91e12d07301f95cdc23d077c44d81a`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 2.7 MB (2720968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ce7bbcb36617017b697c1cedd0f4dad2273643f9315dcb5665c9731e031b3`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 5.7 MB (5746421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621599eddf8a561bdfb15886b7a9609c02a01369e9bd02c9937cdaa7b3ccc212`  
		Last Modified: Thu, 26 Nov 2020 00:10:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0760577d520065d34f4c5a7340b154a10776867a6448a2f6a8692ffe23ea21e`  
		Last Modified: Thu, 26 Nov 2020 00:10:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd26d3d155865f99e5f9f9cc78acd78b78951980e96b704a3d6fc62125f266`  
		Last Modified: Mon, 04 Jan 2021 22:43:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b55cdba3dc093e0f2f23a688d26ebfd23bcbda7c077566297ac179280a6568`  
		Last Modified: Mon, 04 Jan 2021 22:43:51 GMT  
		Size: 139.3 MB (139271674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0584912549af62baba56b0311441340f5a45f758f1c3a96d739b4ca98eb7a8`  
		Last Modified: Mon, 04 Jan 2021 22:43:30 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b0b7d81cfea5fa13c01706f15f9a99a732d4faa0ab0b3637fd26fccd72864`  
		Last Modified: Wed, 13 Jan 2021 20:42:29 GMT  
		Size: 4.5 KB (4450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:ec3ea97c48dedf9707ec201072abde21fa34708c1f706781bb202916b97c64f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:4-windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:0d8e5d81f217e4c15a4155e19e0767d448d75f8274a0750941e7a13dc2a01aa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:7a3b42dd7e569fb530a7418a7b26420b7cca13c896e44ef7f77a34698a4bcef4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:c9b0f40151cd56721707c875677b6df0805d406aeade0ffa52c072273c39a9cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:c46e1f6dd8ac3f8592b53fa2dfdc0f7e26055929e6bf30975838ca0406c5bc2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178220204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97feb3412a387d4d3bbd8653b09ef26683263a192e0e8dc6554e65bfb637a86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:28:23 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 01:28:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:28:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:28:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:20:44 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:20:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:21:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:21:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:21:11 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:21:11 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:21:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:21:12 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:21:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e4e43cb0003675e06e2e17e30cb17e0e9a990abc8a107f259c93be84ccc4f`  
		Last Modified: Thu, 26 Nov 2020 01:30:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50e71d834e14ca61531dcce8e5e52860ea3b03769e5e68cf77ac07e941f6d6`  
		Last Modified: Mon, 04 Jan 2021 22:22:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27768a0d0c674b5175f704d585df68ad33f9bd5be976bd669801075e8ca63526`  
		Last Modified: Mon, 04 Jan 2021 22:22:36 GMT  
		Size: 142.7 MB (142684977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4e0bd8b992a6db5b94cd268f50463e33f8a470bd7b8b3772a177714ce8ccd7`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c887415d06431f09f31175932c083142d41a7de019c848489c1e5412e4b14635`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:66fd4f8f09e92de8744c76702e836f0fc5831255318373435935bc3d589b5f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168150811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25db05811c760dc9c9ba32746c241a6e8a67669179651b91931ba04adf1076d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:44:48 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 25 Nov 2020 23:44:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:44:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:44:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:56 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:43:16 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:43:19 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:43:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:31 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:32 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4913f11c494a00e3d77d01b9364c56f69482ffaeddf32e87f424acd659acff9`  
		Last Modified: Wed, 25 Nov 2020 23:47:35 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17fffdaae13eded3257e5cef69f19565cb07b9602919924393e099e88d56ab9`  
		Last Modified: Mon, 04 Jan 2021 22:44:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c65f20a6385ac5b1be7e719820d32fe6d98175958ee48624f07341afba641aa`  
		Last Modified: Mon, 04 Jan 2021 22:45:23 GMT  
		Size: 136.4 MB (136379637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0fec39db28299b0b7d33a9a2f3a99f3bd9c0cc78ac9190d5c5a33f780ae566`  
		Last Modified: Mon, 04 Jan 2021 22:44:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7c251da439065584411bea56b6288812cbae60767613397e8960289dceaeed`  
		Last Modified: Wed, 13 Jan 2021 20:41:45 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:543de10da111411668affef0a4572320b1a53aad1afd2fd2fec58b4de13cadb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173130142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f718506b8817f58d5917d2b4c2b344ffda20b91739e3701d5b277100d7a8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:54 GMT
ADD file:aa0063276274c9f3ba9308c3cdfd911449966c87546f28ceb3122d6fbd995d52 in / 
# Wed, 25 Nov 2020 22:45:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:07:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 00:08:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:08:17 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 00:08:18 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 00:08:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 00:08:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 00:08:44 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 00:08:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 00:08:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 00:08:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:41:47 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:41:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:11 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:41:41 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:41:42 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:41:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2269433521a3f2e95508abd4fa29a3de21226eed5a09ad3959a689b066151bca`  
		Last Modified: Mon, 23 Nov 2020 18:41:52 GMT  
		Size: 25.4 MB (25381722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442687b9aa7dcd6b97d4f9ce9562774788922b94571cd3a7ea85185cd76cbd3`  
		Last Modified: Wed, 25 Nov 2020 22:47:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6efa602a92c53f638f3667fa4400f2fdb32c5aaae3d112e33f15a12cb2bb3b`  
		Last Modified: Wed, 25 Nov 2020 22:47:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a5fb2071960493a99805bac4506cb07225b998113d5ae9b344509442f9e542`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8d2ce236c235c465ef891cd59df829a91e12d07301f95cdc23d077c44d81a`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 2.7 MB (2720968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ce7bbcb36617017b697c1cedd0f4dad2273643f9315dcb5665c9731e031b3`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 5.7 MB (5746421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621599eddf8a561bdfb15886b7a9609c02a01369e9bd02c9937cdaa7b3ccc212`  
		Last Modified: Thu, 26 Nov 2020 00:10:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0760577d520065d34f4c5a7340b154a10776867a6448a2f6a8692ffe23ea21e`  
		Last Modified: Thu, 26 Nov 2020 00:10:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd26d3d155865f99e5f9f9cc78acd78b78951980e96b704a3d6fc62125f266`  
		Last Modified: Mon, 04 Jan 2021 22:43:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b55cdba3dc093e0f2f23a688d26ebfd23bcbda7c077566297ac179280a6568`  
		Last Modified: Mon, 04 Jan 2021 22:43:51 GMT  
		Size: 139.3 MB (139271674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0584912549af62baba56b0311441340f5a45f758f1c3a96d739b4ca98eb7a8`  
		Last Modified: Mon, 04 Jan 2021 22:43:30 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b0b7d81cfea5fa13c01706f15f9a99a732d4faa0ab0b3637fd26fccd72864`  
		Last Modified: Wed, 13 Jan 2021 20:42:29 GMT  
		Size: 4.5 KB (4450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:094f04532c279cb96da991692896e5a013939e2471e4a98791aa5cd7a196981c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:c46e1f6dd8ac3f8592b53fa2dfdc0f7e26055929e6bf30975838ca0406c5bc2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178220204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97feb3412a387d4d3bbd8653b09ef26683263a192e0e8dc6554e65bfb637a86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 01:27:29 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 01:27:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 01:27:39 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 01:27:39 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 01:27:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 01:27:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 01:28:23 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 01:28:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 01:28:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 01:28:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 01:28:25 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:20:44 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:20:45 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:21:10 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:21:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:21:11 GMT
VOLUME [/data/db /data/configdb]
# Mon, 04 Jan 2021 22:21:11 GMT
COPY file:fbcb6caf305364286a61ba398d76c231d29492455be8f3e3f619f24b45da0b7c in /usr/local/bin/ 
# Mon, 04 Jan 2021 22:21:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Jan 2021 22:21:12 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:21:12 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329e632c35b3e0f2c346e744e72a998b9c53acfae5b6a3a4c5ebc8d49fadfb0b`  
		Last Modified: Thu, 26 Nov 2020 01:30:03 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1bd1325a3d3a46e0aec7e41adaf16028a7d982064006b058917573bfbfa41f`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 3.0 MB (2990946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa6e3d64a4a2739c981152ad6b331547b0c66f324a5e4cf2e74a9595ada8512`  
		Last Modified: Thu, 26 Nov 2020 01:30:02 GMT  
		Size: 5.8 MB (5826997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035bca87b77801743e920b7bed66b07696505c4393b949f2680efd4f33a9f3d3`  
		Last Modified: Thu, 26 Nov 2020 01:30:01 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874e4e43cb0003675e06e2e17e30cb17e0e9a990abc8a107f259c93be84ccc4f`  
		Last Modified: Thu, 26 Nov 2020 01:30:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50e71d834e14ca61531dcce8e5e52860ea3b03769e5e68cf77ac07e941f6d6`  
		Last Modified: Mon, 04 Jan 2021 22:22:13 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27768a0d0c674b5175f704d585df68ad33f9bd5be976bd669801075e8ca63526`  
		Last Modified: Mon, 04 Jan 2021 22:22:36 GMT  
		Size: 142.7 MB (142684977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4e0bd8b992a6db5b94cd268f50463e33f8a470bd7b8b3772a177714ce8ccd7`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c887415d06431f09f31175932c083142d41a7de019c848489c1e5412e4b14635`  
		Last Modified: Mon, 04 Jan 2021 22:22:12 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:66fd4f8f09e92de8744c76702e836f0fc5831255318373435935bc3d589b5f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.2 MB (168150811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25db05811c760dc9c9ba32746c241a6e8a67669179651b91931ba04adf1076d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:42:53 GMT
ADD file:e5b221023382c9e42b8558f8887f8317fe7e9759f59feb1799548aed9236e99b in / 
# Wed, 25 Nov 2020 22:42:56 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:42:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:43:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:43:01 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:43:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 25 Nov 2020 23:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:43:18 GMT
ENV GOSU_VERSION=1.12
# Wed, 25 Nov 2020 23:43:19 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 25 Nov 2020 23:43:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 25 Nov 2020 23:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 25 Nov 2020 23:44:48 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 25 Nov 2020 23:44:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 25 Nov 2020 23:44:53 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 25 Nov 2020 23:44:54 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:55 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 25 Nov 2020 23:44:56 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:43:16 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:43:19 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:43:45 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:40:31 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:40:32 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:40:33 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:04da93b342eb651d6b94c74a934a3290697573a907fa0a06067b538095601745`  
		Last Modified: Thu, 19 Nov 2020 16:25:04 GMT  
		Size: 23.7 MB (23733196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b235194751dee33624fc154603f7e25ecdfbb02538fb7d55fa796df9afa95fee`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606a67bb8db9a1111022bdc6406442e11c1a66653136c5c777114bf67b61038a`  
		Last Modified: Wed, 25 Nov 2020 22:44:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6ea30360a0922b847ae4f3ef0880753d0b7ad22ce552a64e3be28b914a30d5`  
		Last Modified: Wed, 25 Nov 2020 23:47:04 GMT  
		Size: 1.9 KB (1885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5906b3a79ddb65390de38a20eeb2731a3dad958f7ee284c4874b0bdca0affc5`  
		Last Modified: Wed, 25 Nov 2020 23:47:05 GMT  
		Size: 2.7 MB (2681902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18019bad1da070a5b1a23dee98933fb1f17cacd3ef268d130d0cc079fd7fb3c4`  
		Last Modified: Wed, 25 Nov 2020 23:47:06 GMT  
		Size: 5.3 MB (5346719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0caaa340cac2acd66546fa698018ece05ab5af8d0964087cf4d9eef9ac536a`  
		Last Modified: Wed, 25 Nov 2020 23:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4913f11c494a00e3d77d01b9364c56f69482ffaeddf32e87f424acd659acff9`  
		Last Modified: Wed, 25 Nov 2020 23:47:35 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17fffdaae13eded3257e5cef69f19565cb07b9602919924393e099e88d56ab9`  
		Last Modified: Mon, 04 Jan 2021 22:44:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c65f20a6385ac5b1be7e719820d32fe6d98175958ee48624f07341afba641aa`  
		Last Modified: Mon, 04 Jan 2021 22:45:23 GMT  
		Size: 136.4 MB (136379637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0fec39db28299b0b7d33a9a2f3a99f3bd9c0cc78ac9190d5c5a33f780ae566`  
		Last Modified: Mon, 04 Jan 2021 22:44:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7c251da439065584411bea56b6288812cbae60767613397e8960289dceaeed`  
		Last Modified: Wed, 13 Jan 2021 20:41:45 GMT  
		Size: 4.4 KB (4445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:543de10da111411668affef0a4572320b1a53aad1afd2fd2fec58b4de13cadb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.1 MB (173130142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f718506b8817f58d5917d2b4c2b344ffda20b91739e3701d5b277100d7a8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:54 GMT
ADD file:aa0063276274c9f3ba9308c3cdfd911449966c87546f28ceb3122d6fbd995d52 in / 
# Wed, 25 Nov 2020 22:45:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:07:58 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 26 Nov 2020 00:08:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:08:17 GMT
ENV GOSU_VERSION=1.12
# Thu, 26 Nov 2020 00:08:18 GMT
ENV JSYAML_VERSION=3.13.1
# Thu, 26 Nov 2020 00:08:41 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 26 Nov 2020 00:08:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 26 Nov 2020 00:08:44 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Thu, 26 Nov 2020 00:08:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 26 Nov 2020 00:08:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 26 Nov 2020 00:08:53 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 26 Nov 2020 00:08:54 GMT
ENV MONGO_MAJOR=4.4
# Mon, 04 Jan 2021 22:41:47 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:41:49 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Mon, 04 Jan 2021 22:42:53 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Mon, 04 Jan 2021 22:43:11 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 04 Jan 2021 22:43:11 GMT
VOLUME [/data/db /data/configdb]
# Wed, 13 Jan 2021 20:41:41 GMT
COPY file:ca008e179d0bb2264ba7645bc5d3d6b341e0b06e43ae29359ad4f21e58135778 in /usr/local/bin/ 
# Wed, 13 Jan 2021 20:41:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 20:41:42 GMT
EXPOSE 27017
# Wed, 13 Jan 2021 20:41:42 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2269433521a3f2e95508abd4fa29a3de21226eed5a09ad3959a689b066151bca`  
		Last Modified: Mon, 23 Nov 2020 18:41:52 GMT  
		Size: 25.4 MB (25381722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442687b9aa7dcd6b97d4f9ce9562774788922b94571cd3a7ea85185cd76cbd3`  
		Last Modified: Wed, 25 Nov 2020 22:47:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6efa602a92c53f638f3667fa4400f2fdb32c5aaae3d112e33f15a12cb2bb3b`  
		Last Modified: Wed, 25 Nov 2020 22:47:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a5fb2071960493a99805bac4506cb07225b998113d5ae9b344509442f9e542`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 1.9 KB (1883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c8d2ce236c235c465ef891cd59df829a91e12d07301f95cdc23d077c44d81a`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 2.7 MB (2720968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2ce7bbcb36617017b697c1cedd0f4dad2273643f9315dcb5665c9731e031b3`  
		Last Modified: Thu, 26 Nov 2020 00:10:29 GMT  
		Size: 5.7 MB (5746421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621599eddf8a561bdfb15886b7a9609c02a01369e9bd02c9937cdaa7b3ccc212`  
		Last Modified: Thu, 26 Nov 2020 00:10:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0760577d520065d34f4c5a7340b154a10776867a6448a2f6a8692ffe23ea21e`  
		Last Modified: Thu, 26 Nov 2020 00:10:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd26d3d155865f99e5f9f9cc78acd78b78951980e96b704a3d6fc62125f266`  
		Last Modified: Mon, 04 Jan 2021 22:43:31 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b55cdba3dc093e0f2f23a688d26ebfd23bcbda7c077566297ac179280a6568`  
		Last Modified: Mon, 04 Jan 2021 22:43:51 GMT  
		Size: 139.3 MB (139271674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0584912549af62baba56b0311441340f5a45f758f1c3a96d739b4ca98eb7a8`  
		Last Modified: Mon, 04 Jan 2021 22:43:30 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b0b7d81cfea5fa13c01706f15f9a99a732d4faa0ab0b3637fd26fccd72864`  
		Last Modified: Wed, 13 Jan 2021 20:42:29 GMT  
		Size: 4.5 KB (4450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:ec3ea97c48dedf9707ec201072abde21fa34708c1f706781bb202916b97c64f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64
	-	windows version 10.0.14393.4104; amd64

### `mongo:windowsservercore` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:0d8e5d81f217e4c15a4155e19e0767d448d75f8274a0750941e7a13dc2a01aa1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1637; amd64

```console
$ docker pull mongo@sha256:44453059167806e68701c5f7f3a175862f0b5f875238674bb25c39daa218851c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2630730135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0ba2649cdb467ccd36fb65e7a285ae18d7d19d01c9485993e173038920f258a`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 04 Dec 2020 02:13:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Dec 2020 14:02:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:23:34 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:23:35 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:26:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:26:51 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:26:52 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:26:53 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:aa4f58cd6da1aaf1a0b44d443bd88e7fbe5b0a6f193995a1a61d6bd63990f314`  
		Size: 672.5 MB (672541583 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:240407eb82b6591b0574396ec829a4a5cd9a75257a4663f9876942995275965d`  
		Last Modified: Wed, 09 Dec 2020 17:10:14 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22061bafff402fecdcfdc393917a5e27f9b8eb154f2e9fbb62ed7fd1c804a98f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22bb8acd20531fd59b42a44f1dccaee8a63059c5ee8a56caffd08135c41b2f`  
		Last Modified: Mon, 04 Jan 2021 22:34:26 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0009b56252b87261ace9d78c1c3d436d96efa891747bf7f8136f712e3cdbb27`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09e7a998b53c1340ad67ce780b4ca0cd1e6d02bec1244b1a678b38cf13f3b27`  
		Last Modified: Mon, 04 Jan 2021 22:35:05 GMT  
		Size: 239.8 MB (239847774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74eb0c6548847cf74fe9f19063d7a41044da83d9b59f43ae2f82546b61c82e19`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84110c2b55ac75c1cbd9492fb995107756a4476863348846da2b56b57bb46`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f03299f3178458c7a31a86086503a2226c8454be9b1b8ccbd903303d0bc940f`  
		Last Modified: Mon, 04 Jan 2021 22:34:23 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:7a3b42dd7e569fb530a7418a7b26420b7cca13c896e44ef7f77a34698a4bcef4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull mongo@sha256:78ef64ede71474e410c48188797f133a162463abfe110c5b086b83a8d3b75878
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (6009434039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdcba5af7daaed9966caa30e82279cee5e2d348e806825b7a338520a3ab29f80`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 14:41:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Mon, 04 Jan 2021 22:27:02 GMT
ENV MONGO_VERSION=4.4.3
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.3-signed.msi
# Mon, 04 Jan 2021 22:27:03 GMT
ENV MONGO_DOWNLOAD_SHA256=d811282527bbdc3266244209ad0971c0d375dbb209bb8eb4ae66ba576b19e9f6
# Mon, 04 Jan 2021 22:31:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=ServerNoService,Client,Router,MiscellaneousTools' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Mon, 04 Jan 2021 22:31:06 GMT
VOLUME [C:\data\db C:\data\configdb]
# Mon, 04 Jan 2021 22:31:07 GMT
EXPOSE 27017
# Mon, 04 Jan 2021 22:31:08 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b5a79f8be42bf1c358ccc82f32c1481de95c393ef97e712a321c1440d132fda9`  
		Last Modified: Wed, 09 Dec 2020 17:11:03 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ed6eabbe0629def987ae9a59ab4143065625906ec580605b376f2965b80cec`  
		Last Modified: Mon, 04 Jan 2021 22:35:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcd8c68224aa353f236c72cd255b2c810310e6d1e2b18421bb4acbc59d2c08c`  
		Last Modified: Mon, 04 Jan 2021 22:35:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277e63f380b12813c6508f90e8dbc1fc120b66eca072cfa955ed3eada4dc5d2c`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924c1827532309ab811fe6c8237889ff0609cb18b38a25a616de7137faa2b305`  
		Last Modified: Mon, 04 Jan 2021 22:36:10 GMT  
		Size: 240.6 MB (240581996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b6f894aaab562049aa7a75e4634c6393b482d866481e175112102349f4b83`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b152601fa94b531b76e92551e4d579965e456e5b315f0289f784691512b806ac`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2d804f27797906f589ac7bc283c328314f27f95a9155f386b6768d9528cf3e`  
		Last Modified: Mon, 04 Jan 2021 22:35:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
