<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3.4`](#mongo34)
-	[`mongo:3.4.23`](#mongo3423)
-	[`mongo:3.4.23-windowsservercore`](#mongo3423-windowsservercore)
-	[`mongo:3.4.23-windowsservercore-ltsc2016`](#mongo3423-windowsservercore-ltsc2016)
-	[`mongo:3.4.23-xenial`](#mongo3423-xenial)
-	[`mongo:3.4-windowsservercore`](#mongo34-windowsservercore)
-	[`mongo:3.4-windowsservercore-ltsc2016`](#mongo34-windowsservercore-ltsc2016)
-	[`mongo:3.4-xenial`](#mongo34-xenial)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6.16`](#mongo3616)
-	[`mongo:3.6.16-windowsservercore`](#mongo3616-windowsservercore)
-	[`mongo:3.6.16-windowsservercore-ltsc2016`](#mongo3616-windowsservercore-ltsc2016)
-	[`mongo:3.6.16-xenial`](#mongo3616-xenial)
-	[`mongo:3.6-windowsservercore`](#mongo36-windowsservercore)
-	[`mongo:3.6-windowsservercore-ltsc2016`](#mongo36-windowsservercore-ltsc2016)
-	[`mongo:3.6-xenial`](#mongo36-xenial)
-	[`mongo:3-windowsservercore`](#mongo3-windowsservercore)
-	[`mongo:3-windowsservercore-ltsc2016`](#mongo3-windowsservercore-ltsc2016)
-	[`mongo:3-xenial`](#mongo3-xenial)
-	[`mongo:4`](#mongo4)
-	[`mongo:4.0`](#mongo40)
-	[`mongo:4.0.14`](#mongo4014)
-	[`mongo:4.0.14-windowsservercore`](#mongo4014-windowsservercore)
-	[`mongo:4.0.14-windowsservercore-1809`](#mongo4014-windowsservercore-1809)
-	[`mongo:4.0.14-windowsservercore-ltsc2016`](#mongo4014-windowsservercore-ltsc2016)
-	[`mongo:4.0.14-xenial`](#mongo4014-xenial)
-	[`mongo:4.0-windowsservercore`](#mongo40-windowsservercore)
-	[`mongo:4.0-windowsservercore-1809`](#mongo40-windowsservercore-1809)
-	[`mongo:4.0-windowsservercore-ltsc2016`](#mongo40-windowsservercore-ltsc2016)
-	[`mongo:4.0-xenial`](#mongo40-xenial)
-	[`mongo:4.2`](#mongo42)
-	[`mongo:4.2.2`](#mongo422)
-	[`mongo:4.2.2-bionic`](#mongo422-bionic)
-	[`mongo:4.2.2-windowsservercore`](#mongo422-windowsservercore)
-	[`mongo:4.2.2-windowsservercore-1809`](#mongo422-windowsservercore-1809)
-	[`mongo:4.2.2-windowsservercore-ltsc2016`](#mongo422-windowsservercore-ltsc2016)
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
$ docker pull mongo@sha256:5b5e8a1fe36a8a2b9abb7da88322f17a4388d1bd81479d0f02953621ba02da0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3384; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:5a2bbd4d98428560888ee895b9fdfe341ed6a2cba5dc5438e64abe2a3adba1f3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165551342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3745fa14a0ed421d031f79653eb1dcb28860988f00ac0ff7f8ae43f0f22f0588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:04 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 19 Dec 2019 07:55:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_MAJOR=3.6
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_VERSION=3.6.16
# Thu, 19 Dec 2019 07:55:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:27 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:27 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:27 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95d19a2f4396aed383bb89fdb2ac0adf5f6d9e4bb8ff3e43e04e7fa066602c`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25973630e92b3431c16828c8add3a7b5cce84c6d9f108d9402afbc1dc96f944b`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f773c926f5697a63c93194ac162c8b30dd710039b822407efdd281f586d2585e`  
		Last Modified: Thu, 19 Dec 2019 07:57:55 GMT  
		Size: 117.2 MB (117228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b4232d63033b58c91ed73644ccdc96aabecb91bf807ba9fd981b5bddb23ff5`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b7a63572970bb41931de8f074b3e4b6694054d7d97f287886f135c8f1bd50a`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:4d6093c2b1e85db9acfffcf152e936a481fac5af3a05a8d679a9fa1f9923b0b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155040149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ee79b405e7b46538372c16edc6a1549cd7e1f76907fb7070bef7ddc69937f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:49:52 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 Nov 2019 00:49:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:55 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:56 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:57 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:58 GMT
ENV MONGO_MAJOR=3.6
# Tue, 03 Dec 2019 23:47:18 GMT
ENV MONGO_VERSION=3.6.16
# Tue, 03 Dec 2019 23:47:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 03 Dec 2019 23:47:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 03 Dec 2019 23:47:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 03 Dec 2019 23:47:47 GMT
VOLUME [/data/db /data/configdb]
# Tue, 03 Dec 2019 23:47:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Tue, 03 Dec 2019 23:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Dec 2019 23:47:49 GMT
EXPOSE 27017
# Tue, 03 Dec 2019 23:47:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebea15061d7e2a3269c663f7ecb0d5b395e1e49c409b8d064dbe5f7d6e72172`  
		Last Modified: Wed, 27 Nov 2019 00:53:25 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2935a9205e0bef6cd51d522ccd870fe0dc3ffdea544e47c9ac26be8eb3122`  
		Last Modified: Tue, 03 Dec 2019 23:48:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9e65ee1a4b2ed96c6967fb16eb0de7c63da6bce0c47e3ec63d0c9bd5a237a`  
		Last Modified: Tue, 03 Dec 2019 23:48:49 GMT  
		Size: 111.4 MB (111433459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6a6b8b935e01daa47297ffcd098477b6928da4ffc96f92547c69d47479304f`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27528e779b9e619704d2f2e340fa917637a6413c6f864c8864405df4245b2a2a`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:1bdcfaae6aafbb14428a8892a23124a40f31bd9414e5d2c3b641904db525a5a8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816186803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23192a55795afdee48dc3b3724f1c8a7a93396e95bff38c432c3e559fb9ba27c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:57:29 GMT
ENV MONGO_VERSION=3.6.16
# Wed, 11 Dec 2019 22:57:30 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.16-signed.msi
# Wed, 11 Dec 2019 22:57:32 GMT
ENV MONGO_DOWNLOAD_SHA256=06d8b235702c6a2a4f1b721bbd4b59efbc67d0b9dcd5b4d31984c75946837a2e
# Wed, 11 Dec 2019 23:06:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 23:06:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 23:06:42 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 23:06:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628896678dbc43683e49f91e61271412aa1d97a90b65a2ed04e74157fa49532b`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f11a3aaf5933be1369a1954c04a62d6f707a9e9cde397a42e567f5648e768`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836437d81474147d2932b37b6634ea7d129614983deba273248aae15400c3d08`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c1a30da870a0715c3a3c01c9ab82079b1057836d8b6591a358b85f5c6b8339`  
		Last Modified: Thu, 12 Dec 2019 00:05:41 GMT  
		Size: 93.5 MB (93474561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ece9fda5ed7b5d814b85fdc19ec1154ec7939bc68330c399127bd4e855024`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3ecfc5eca20e232501e1be3e7bcd29af0358074cbe07316e39ff04be2c224`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2833f1058a943a474d0b1fb420d65ba0c50b5b30e8edf26032ec538ed6360beb`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4`

```console
$ docker pull mongo@sha256:20e954040e45907fccb8aba88c72b6ad79b3685807ef9e2ac4549fa115574fbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.4` - linux; amd64

```console
$ docker pull mongo@sha256:0d360783fe5d86eeec1adc31a90dd6fee8ab576381c77d82894c1e9fa05c7847
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (168014352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5705ea1f839c8808510a50c5beab55fc6f377d2f55a9417198f47db97ea78c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:54:33 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 19 Dec 2019 07:54:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:54:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:54:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:54:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:54:34 GMT
ENV MONGO_MAJOR=3.4
# Thu, 19 Dec 2019 07:54:35 GMT
ENV MONGO_VERSION=3.4.23
# Thu, 19 Dec 2019 07:54:35 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:54:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:54:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:54:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:54:54 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:54:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat (3.4)
# Thu, 19 Dec 2019 07:54:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:54:55 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:54:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc15de95098a27445966b629fb567784e2a45fe5f204e14796c948dbc193a0fa`  
		Last Modified: Thu, 19 Dec 2019 07:57:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4182c60a7c124c655a0185bce71bf66019ab5403d7b00b04488e2db42397669c`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6002019487be8777fc76c87f006fee622b973f6cc80d3f6dd9b07bc13a1e9c31`  
		Last Modified: Thu, 19 Dec 2019 07:57:24 GMT  
		Size: 119.7 MB (119690902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7f880ce0d5d99c3faca76573c3d92e43e65e888336db62f85fd7607703a97e`  
		Last Modified: Thu, 19 Dec 2019 07:57:03 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132ede0b4f0060c27c1f2df3745b676ffa1bd9ee6ca9c547657b9be8198d2aa2`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 4.0 KB (4012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286f318ee03142e4030a775085c8bbc24029cb106ad2fb0be1ad3dce615b7021`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fe85914cb2acfa4566f55e84020d0fec0928fe78278028641db565f22cbda373
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156509463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bec8fc74b4cc1dba49eedacd4bbb713ae3bd71d82f5254096bb551bf21c5e6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:48:58 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Wed, 27 Nov 2019 00:49:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:02 GMT
ENV MONGO_MAJOR=3.4
# Wed, 27 Nov 2019 00:49:03 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 27 Nov 2019 00:49:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 Nov 2019 00:49:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 Nov 2019 00:49:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 Nov 2019 00:49:34 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 Nov 2019 00:49:36 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Wed, 27 Nov 2019 00:49:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat (3.4)
# Wed, 27 Nov 2019 00:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Nov 2019 00:49:40 GMT
EXPOSE 27017
# Wed, 27 Nov 2019 00:49:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a584ca199e1f752345b7703fa96fc8e508d6a1f9356ff1aa9760b6fe8247a8e`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacdf9ff19e7305d7121240dfd9d1b49c56446a62c1a13dbc0ff974cf1d2fdb1`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c54bfa417fa777e458b4a690c984d42605c4ba2d9133b5ea4f3ed0f7883939`  
		Last Modified: Wed, 27 Nov 2019 00:53:10 GMT  
		Size: 112.9 MB (112902650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfb71c955fb087026c7ee53b62e51bf1e734704b8d1ad6cdf23ba533e3090fe`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631fade05419c01f5ca14bff6ecb12a246d75dbbb7358daa79afa37a7f87d878`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20da495cf7cbbe25ed9a76a9f58c07412036412ab9fc9f9b07550cc7a62246b2`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:e16c4d20c606d871234bdb0646a07fed96c7c00c6d611c851990d1f03d998088
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814790844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c474f0259ca30e23f0af22868e318fd2c390db53bbc09401d894347a029e297`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:54:10 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 11 Dec 2019 22:54:11 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.23-signed.msi
# Wed, 11 Dec 2019 22:54:12 GMT
ENV MONGO_DOWNLOAD_SHA256=7b43467dce18599d8f0fff3fe7f4e204e08598e09ecfcaf65fc83c69791792cf
# Wed, 11 Dec 2019 22:57:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 22:57:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 22:57:12 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 22:57:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9523a305809803867a7c8184c661ca8e07d09250d115f76a5afbfcecd86bb2`  
		Last Modified: Thu, 12 Dec 2019 00:04:23 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07a73e133029c5064cd425b52131222d21888abbf5e5f2de7cc8abdd80a1313`  
		Last Modified: Thu, 12 Dec 2019 00:04:22 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acbd03e1cbfaea390737c6ca0a9907094bbb5877915f9dc273d2e91c7cea6d5`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516dfd7d42b8e69b4e11e16ecc131d94667e51aff48da7e02a90d657122d2069`  
		Last Modified: Thu, 12 Dec 2019 00:04:50 GMT  
		Size: 92.1 MB (92078605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a941a3e4603ccf48c3ff03c56e6dedf804bc38b9c3b2f2afa278baeac58a95dd`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0568cf846cc19ce9b662894d626cf207ef84597e046927350daa419118e108`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f659f4fe3b4d95be807483b1882efdebb26a2d88608a43b0bdc613e40f4ec`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.23`

```console
$ docker pull mongo@sha256:20e954040e45907fccb8aba88c72b6ad79b3685807ef9e2ac4549fa115574fbd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.4.23` - linux; amd64

```console
$ docker pull mongo@sha256:0d360783fe5d86eeec1adc31a90dd6fee8ab576381c77d82894c1e9fa05c7847
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (168014352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5705ea1f839c8808510a50c5beab55fc6f377d2f55a9417198f47db97ea78c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:54:33 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 19 Dec 2019 07:54:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:54:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:54:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:54:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:54:34 GMT
ENV MONGO_MAJOR=3.4
# Thu, 19 Dec 2019 07:54:35 GMT
ENV MONGO_VERSION=3.4.23
# Thu, 19 Dec 2019 07:54:35 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:54:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:54:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:54:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:54:54 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:54:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat (3.4)
# Thu, 19 Dec 2019 07:54:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:54:55 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:54:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc15de95098a27445966b629fb567784e2a45fe5f204e14796c948dbc193a0fa`  
		Last Modified: Thu, 19 Dec 2019 07:57:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4182c60a7c124c655a0185bce71bf66019ab5403d7b00b04488e2db42397669c`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6002019487be8777fc76c87f006fee622b973f6cc80d3f6dd9b07bc13a1e9c31`  
		Last Modified: Thu, 19 Dec 2019 07:57:24 GMT  
		Size: 119.7 MB (119690902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7f880ce0d5d99c3faca76573c3d92e43e65e888336db62f85fd7607703a97e`  
		Last Modified: Thu, 19 Dec 2019 07:57:03 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132ede0b4f0060c27c1f2df3745b676ffa1bd9ee6ca9c547657b9be8198d2aa2`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 4.0 KB (4012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286f318ee03142e4030a775085c8bbc24029cb106ad2fb0be1ad3dce615b7021`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4.23` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fe85914cb2acfa4566f55e84020d0fec0928fe78278028641db565f22cbda373
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156509463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bec8fc74b4cc1dba49eedacd4bbb713ae3bd71d82f5254096bb551bf21c5e6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:48:58 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Wed, 27 Nov 2019 00:49:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:02 GMT
ENV MONGO_MAJOR=3.4
# Wed, 27 Nov 2019 00:49:03 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 27 Nov 2019 00:49:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 Nov 2019 00:49:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 Nov 2019 00:49:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 Nov 2019 00:49:34 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 Nov 2019 00:49:36 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Wed, 27 Nov 2019 00:49:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat (3.4)
# Wed, 27 Nov 2019 00:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Nov 2019 00:49:40 GMT
EXPOSE 27017
# Wed, 27 Nov 2019 00:49:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a584ca199e1f752345b7703fa96fc8e508d6a1f9356ff1aa9760b6fe8247a8e`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacdf9ff19e7305d7121240dfd9d1b49c56446a62c1a13dbc0ff974cf1d2fdb1`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c54bfa417fa777e458b4a690c984d42605c4ba2d9133b5ea4f3ed0f7883939`  
		Last Modified: Wed, 27 Nov 2019 00:53:10 GMT  
		Size: 112.9 MB (112902650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfb71c955fb087026c7ee53b62e51bf1e734704b8d1ad6cdf23ba533e3090fe`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631fade05419c01f5ca14bff6ecb12a246d75dbbb7358daa79afa37a7f87d878`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20da495cf7cbbe25ed9a76a9f58c07412036412ab9fc9f9b07550cc7a62246b2`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4.23` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:e16c4d20c606d871234bdb0646a07fed96c7c00c6d611c851990d1f03d998088
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814790844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c474f0259ca30e23f0af22868e318fd2c390db53bbc09401d894347a029e297`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:54:10 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 11 Dec 2019 22:54:11 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.23-signed.msi
# Wed, 11 Dec 2019 22:54:12 GMT
ENV MONGO_DOWNLOAD_SHA256=7b43467dce18599d8f0fff3fe7f4e204e08598e09ecfcaf65fc83c69791792cf
# Wed, 11 Dec 2019 22:57:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 22:57:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 22:57:12 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 22:57:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9523a305809803867a7c8184c661ca8e07d09250d115f76a5afbfcecd86bb2`  
		Last Modified: Thu, 12 Dec 2019 00:04:23 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07a73e133029c5064cd425b52131222d21888abbf5e5f2de7cc8abdd80a1313`  
		Last Modified: Thu, 12 Dec 2019 00:04:22 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acbd03e1cbfaea390737c6ca0a9907094bbb5877915f9dc273d2e91c7cea6d5`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516dfd7d42b8e69b4e11e16ecc131d94667e51aff48da7e02a90d657122d2069`  
		Last Modified: Thu, 12 Dec 2019 00:04:50 GMT  
		Size: 92.1 MB (92078605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a941a3e4603ccf48c3ff03c56e6dedf804bc38b9c3b2f2afa278baeac58a95dd`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0568cf846cc19ce9b662894d626cf207ef84597e046927350daa419118e108`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f659f4fe3b4d95be807483b1882efdebb26a2d88608a43b0bdc613e40f4ec`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.23-windowsservercore`

```console
$ docker pull mongo@sha256:db0fc781466d6c1630b0207c7a1d72c8c47c7a169c2fdc55dfb5637f078e0c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.4.23-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:e16c4d20c606d871234bdb0646a07fed96c7c00c6d611c851990d1f03d998088
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814790844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c474f0259ca30e23f0af22868e318fd2c390db53bbc09401d894347a029e297`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:54:10 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 11 Dec 2019 22:54:11 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.23-signed.msi
# Wed, 11 Dec 2019 22:54:12 GMT
ENV MONGO_DOWNLOAD_SHA256=7b43467dce18599d8f0fff3fe7f4e204e08598e09ecfcaf65fc83c69791792cf
# Wed, 11 Dec 2019 22:57:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 22:57:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 22:57:12 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 22:57:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9523a305809803867a7c8184c661ca8e07d09250d115f76a5afbfcecd86bb2`  
		Last Modified: Thu, 12 Dec 2019 00:04:23 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07a73e133029c5064cd425b52131222d21888abbf5e5f2de7cc8abdd80a1313`  
		Last Modified: Thu, 12 Dec 2019 00:04:22 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acbd03e1cbfaea390737c6ca0a9907094bbb5877915f9dc273d2e91c7cea6d5`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516dfd7d42b8e69b4e11e16ecc131d94667e51aff48da7e02a90d657122d2069`  
		Last Modified: Thu, 12 Dec 2019 00:04:50 GMT  
		Size: 92.1 MB (92078605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a941a3e4603ccf48c3ff03c56e6dedf804bc38b9c3b2f2afa278baeac58a95dd`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0568cf846cc19ce9b662894d626cf207ef84597e046927350daa419118e108`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f659f4fe3b4d95be807483b1882efdebb26a2d88608a43b0bdc613e40f4ec`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.23-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:db0fc781466d6c1630b0207c7a1d72c8c47c7a169c2fdc55dfb5637f078e0c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.4.23-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:e16c4d20c606d871234bdb0646a07fed96c7c00c6d611c851990d1f03d998088
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814790844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c474f0259ca30e23f0af22868e318fd2c390db53bbc09401d894347a029e297`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:54:10 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 11 Dec 2019 22:54:11 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.23-signed.msi
# Wed, 11 Dec 2019 22:54:12 GMT
ENV MONGO_DOWNLOAD_SHA256=7b43467dce18599d8f0fff3fe7f4e204e08598e09ecfcaf65fc83c69791792cf
# Wed, 11 Dec 2019 22:57:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 22:57:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 22:57:12 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 22:57:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9523a305809803867a7c8184c661ca8e07d09250d115f76a5afbfcecd86bb2`  
		Last Modified: Thu, 12 Dec 2019 00:04:23 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07a73e133029c5064cd425b52131222d21888abbf5e5f2de7cc8abdd80a1313`  
		Last Modified: Thu, 12 Dec 2019 00:04:22 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acbd03e1cbfaea390737c6ca0a9907094bbb5877915f9dc273d2e91c7cea6d5`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516dfd7d42b8e69b4e11e16ecc131d94667e51aff48da7e02a90d657122d2069`  
		Last Modified: Thu, 12 Dec 2019 00:04:50 GMT  
		Size: 92.1 MB (92078605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a941a3e4603ccf48c3ff03c56e6dedf804bc38b9c3b2f2afa278baeac58a95dd`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0568cf846cc19ce9b662894d626cf207ef84597e046927350daa419118e108`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f659f4fe3b4d95be807483b1882efdebb26a2d88608a43b0bdc613e40f4ec`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4.23-xenial`

```console
$ docker pull mongo@sha256:35f11cd21a5181bb5dcd4b8fffb62495917046053e846292a8d6e5f5cfae77bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.4.23-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:0d360783fe5d86eeec1adc31a90dd6fee8ab576381c77d82894c1e9fa05c7847
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (168014352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5705ea1f839c8808510a50c5beab55fc6f377d2f55a9417198f47db97ea78c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:54:33 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 19 Dec 2019 07:54:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:54:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:54:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:54:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:54:34 GMT
ENV MONGO_MAJOR=3.4
# Thu, 19 Dec 2019 07:54:35 GMT
ENV MONGO_VERSION=3.4.23
# Thu, 19 Dec 2019 07:54:35 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:54:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:54:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:54:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:54:54 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:54:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat (3.4)
# Thu, 19 Dec 2019 07:54:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:54:55 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:54:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc15de95098a27445966b629fb567784e2a45fe5f204e14796c948dbc193a0fa`  
		Last Modified: Thu, 19 Dec 2019 07:57:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4182c60a7c124c655a0185bce71bf66019ab5403d7b00b04488e2db42397669c`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6002019487be8777fc76c87f006fee622b973f6cc80d3f6dd9b07bc13a1e9c31`  
		Last Modified: Thu, 19 Dec 2019 07:57:24 GMT  
		Size: 119.7 MB (119690902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7f880ce0d5d99c3faca76573c3d92e43e65e888336db62f85fd7607703a97e`  
		Last Modified: Thu, 19 Dec 2019 07:57:03 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132ede0b4f0060c27c1f2df3745b676ffa1bd9ee6ca9c547657b9be8198d2aa2`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 4.0 KB (4012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286f318ee03142e4030a775085c8bbc24029cb106ad2fb0be1ad3dce615b7021`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4.23-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fe85914cb2acfa4566f55e84020d0fec0928fe78278028641db565f22cbda373
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156509463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bec8fc74b4cc1dba49eedacd4bbb713ae3bd71d82f5254096bb551bf21c5e6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:48:58 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Wed, 27 Nov 2019 00:49:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:02 GMT
ENV MONGO_MAJOR=3.4
# Wed, 27 Nov 2019 00:49:03 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 27 Nov 2019 00:49:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 Nov 2019 00:49:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 Nov 2019 00:49:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 Nov 2019 00:49:34 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 Nov 2019 00:49:36 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Wed, 27 Nov 2019 00:49:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat (3.4)
# Wed, 27 Nov 2019 00:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Nov 2019 00:49:40 GMT
EXPOSE 27017
# Wed, 27 Nov 2019 00:49:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a584ca199e1f752345b7703fa96fc8e508d6a1f9356ff1aa9760b6fe8247a8e`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacdf9ff19e7305d7121240dfd9d1b49c56446a62c1a13dbc0ff974cf1d2fdb1`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c54bfa417fa777e458b4a690c984d42605c4ba2d9133b5ea4f3ed0f7883939`  
		Last Modified: Wed, 27 Nov 2019 00:53:10 GMT  
		Size: 112.9 MB (112902650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfb71c955fb087026c7ee53b62e51bf1e734704b8d1ad6cdf23ba533e3090fe`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631fade05419c01f5ca14bff6ecb12a246d75dbbb7358daa79afa37a7f87d878`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20da495cf7cbbe25ed9a76a9f58c07412036412ab9fc9f9b07550cc7a62246b2`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4-windowsservercore`

```console
$ docker pull mongo@sha256:db0fc781466d6c1630b0207c7a1d72c8c47c7a169c2fdc55dfb5637f078e0c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.4-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:e16c4d20c606d871234bdb0646a07fed96c7c00c6d611c851990d1f03d998088
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814790844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c474f0259ca30e23f0af22868e318fd2c390db53bbc09401d894347a029e297`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:54:10 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 11 Dec 2019 22:54:11 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.23-signed.msi
# Wed, 11 Dec 2019 22:54:12 GMT
ENV MONGO_DOWNLOAD_SHA256=7b43467dce18599d8f0fff3fe7f4e204e08598e09ecfcaf65fc83c69791792cf
# Wed, 11 Dec 2019 22:57:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 22:57:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 22:57:12 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 22:57:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9523a305809803867a7c8184c661ca8e07d09250d115f76a5afbfcecd86bb2`  
		Last Modified: Thu, 12 Dec 2019 00:04:23 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07a73e133029c5064cd425b52131222d21888abbf5e5f2de7cc8abdd80a1313`  
		Last Modified: Thu, 12 Dec 2019 00:04:22 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acbd03e1cbfaea390737c6ca0a9907094bbb5877915f9dc273d2e91c7cea6d5`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516dfd7d42b8e69b4e11e16ecc131d94667e51aff48da7e02a90d657122d2069`  
		Last Modified: Thu, 12 Dec 2019 00:04:50 GMT  
		Size: 92.1 MB (92078605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a941a3e4603ccf48c3ff03c56e6dedf804bc38b9c3b2f2afa278baeac58a95dd`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0568cf846cc19ce9b662894d626cf207ef84597e046927350daa419118e108`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f659f4fe3b4d95be807483b1882efdebb26a2d88608a43b0bdc613e40f4ec`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:db0fc781466d6c1630b0207c7a1d72c8c47c7a169c2fdc55dfb5637f078e0c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.4-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:e16c4d20c606d871234bdb0646a07fed96c7c00c6d611c851990d1f03d998088
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5814790844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c474f0259ca30e23f0af22868e318fd2c390db53bbc09401d894347a029e297`
-	Default Command: `["mongod"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:54:10 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 11 Dec 2019 22:54:11 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.4.23-signed.msi
# Wed, 11 Dec 2019 22:54:12 GMT
ENV MONGO_DOWNLOAD_SHA256=7b43467dce18599d8f0fff3fe7f4e204e08598e09ecfcaf65fc83c69791792cf
# Wed, 11 Dec 2019 22:57:08 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 22:57:10 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 22:57:12 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 22:57:14 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9523a305809803867a7c8184c661ca8e07d09250d115f76a5afbfcecd86bb2`  
		Last Modified: Thu, 12 Dec 2019 00:04:23 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07a73e133029c5064cd425b52131222d21888abbf5e5f2de7cc8abdd80a1313`  
		Last Modified: Thu, 12 Dec 2019 00:04:22 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5acbd03e1cbfaea390737c6ca0a9907094bbb5877915f9dc273d2e91c7cea6d5`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516dfd7d42b8e69b4e11e16ecc131d94667e51aff48da7e02a90d657122d2069`  
		Last Modified: Thu, 12 Dec 2019 00:04:50 GMT  
		Size: 92.1 MB (92078605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a941a3e4603ccf48c3ff03c56e6dedf804bc38b9c3b2f2afa278baeac58a95dd`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0568cf846cc19ce9b662894d626cf207ef84597e046927350daa419118e108`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f659f4fe3b4d95be807483b1882efdebb26a2d88608a43b0bdc613e40f4ec`  
		Last Modified: Thu, 12 Dec 2019 00:04:20 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.4-xenial`

```console
$ docker pull mongo@sha256:35f11cd21a5181bb5dcd4b8fffb62495917046053e846292a8d6e5f5cfae77bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.4-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:0d360783fe5d86eeec1adc31a90dd6fee8ab576381c77d82894c1e9fa05c7847
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (168014352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5705ea1f839c8808510a50c5beab55fc6f377d2f55a9417198f47db97ea78c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:54:33 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Thu, 19 Dec 2019 07:54:34 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:54:34 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:54:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:54:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:54:34 GMT
ENV MONGO_MAJOR=3.4
# Thu, 19 Dec 2019 07:54:35 GMT
ENV MONGO_VERSION=3.4.23
# Thu, 19 Dec 2019 07:54:35 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:54:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:54:54 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:54:54 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:54:54 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:54:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat (3.4)
# Thu, 19 Dec 2019 07:54:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:54:55 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:54:55 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc15de95098a27445966b629fb567784e2a45fe5f204e14796c948dbc193a0fa`  
		Last Modified: Thu, 19 Dec 2019 07:57:03 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4182c60a7c124c655a0185bce71bf66019ab5403d7b00b04488e2db42397669c`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6002019487be8777fc76c87f006fee622b973f6cc80d3f6dd9b07bc13a1e9c31`  
		Last Modified: Thu, 19 Dec 2019 07:57:24 GMT  
		Size: 119.7 MB (119690902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7f880ce0d5d99c3faca76573c3d92e43e65e888336db62f85fd7607703a97e`  
		Last Modified: Thu, 19 Dec 2019 07:57:03 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132ede0b4f0060c27c1f2df3745b676ffa1bd9ee6ca9c547657b9be8198d2aa2`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 4.0 KB (4012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286f318ee03142e4030a775085c8bbc24029cb106ad2fb0be1ad3dce615b7021`  
		Last Modified: Thu, 19 Dec 2019 07:57:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.4-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:fe85914cb2acfa4566f55e84020d0fec0928fe78278028641db565f22cbda373
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156509463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bec8fc74b4cc1dba49eedacd4bbb713ae3bd71d82f5254096bb551bf21c5e6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:48:58 GMT
ENV GPG_KEYS=0C49F3730359A14518585931BC711F9BA15703C6
# Wed, 27 Nov 2019 00:49:00 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:01 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:01 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:02 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:02 GMT
ENV MONGO_MAJOR=3.4
# Wed, 27 Nov 2019 00:49:03 GMT
ENV MONGO_VERSION=3.4.23
# Wed, 27 Nov 2019 00:49:06 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 27 Nov 2019 00:49:29 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 27 Nov 2019 00:49:33 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 27 Nov 2019 00:49:34 GMT
VOLUME [/data/db /data/configdb]
# Wed, 27 Nov 2019 00:49:36 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Wed, 27 Nov 2019 00:49:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat (3.4)
# Wed, 27 Nov 2019 00:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Nov 2019 00:49:40 GMT
EXPOSE 27017
# Wed, 27 Nov 2019 00:49:41 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a584ca199e1f752345b7703fa96fc8e508d6a1f9356ff1aa9760b6fe8247a8e`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.0 KB (1998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacdf9ff19e7305d7121240dfd9d1b49c56446a62c1a13dbc0ff974cf1d2fdb1`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c54bfa417fa777e458b4a690c984d42605c4ba2d9133b5ea4f3ed0f7883939`  
		Last Modified: Wed, 27 Nov 2019 00:53:10 GMT  
		Size: 112.9 MB (112902650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfb71c955fb087026c7ee53b62e51bf1e734704b8d1ad6cdf23ba533e3090fe`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631fade05419c01f5ca14bff6ecb12a246d75dbbb7358daa79afa37a7f87d878`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20da495cf7cbbe25ed9a76a9f58c07412036412ab9fc9f9b07550cc7a62246b2`  
		Last Modified: Wed, 27 Nov 2019 00:52:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:5b5e8a1fe36a8a2b9abb7da88322f17a4388d1bd81479d0f02953621ba02da0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:5a2bbd4d98428560888ee895b9fdfe341ed6a2cba5dc5438e64abe2a3adba1f3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165551342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3745fa14a0ed421d031f79653eb1dcb28860988f00ac0ff7f8ae43f0f22f0588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:04 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 19 Dec 2019 07:55:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_MAJOR=3.6
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_VERSION=3.6.16
# Thu, 19 Dec 2019 07:55:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:27 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:27 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:27 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95d19a2f4396aed383bb89fdb2ac0adf5f6d9e4bb8ff3e43e04e7fa066602c`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25973630e92b3431c16828c8add3a7b5cce84c6d9f108d9402afbc1dc96f944b`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f773c926f5697a63c93194ac162c8b30dd710039b822407efdd281f586d2585e`  
		Last Modified: Thu, 19 Dec 2019 07:57:55 GMT  
		Size: 117.2 MB (117228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b4232d63033b58c91ed73644ccdc96aabecb91bf807ba9fd981b5bddb23ff5`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b7a63572970bb41931de8f074b3e4b6694054d7d97f287886f135c8f1bd50a`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:4d6093c2b1e85db9acfffcf152e936a481fac5af3a05a8d679a9fa1f9923b0b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155040149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ee79b405e7b46538372c16edc6a1549cd7e1f76907fb7070bef7ddc69937f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:49:52 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 Nov 2019 00:49:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:55 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:56 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:57 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:58 GMT
ENV MONGO_MAJOR=3.6
# Tue, 03 Dec 2019 23:47:18 GMT
ENV MONGO_VERSION=3.6.16
# Tue, 03 Dec 2019 23:47:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 03 Dec 2019 23:47:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 03 Dec 2019 23:47:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 03 Dec 2019 23:47:47 GMT
VOLUME [/data/db /data/configdb]
# Tue, 03 Dec 2019 23:47:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Tue, 03 Dec 2019 23:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Dec 2019 23:47:49 GMT
EXPOSE 27017
# Tue, 03 Dec 2019 23:47:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebea15061d7e2a3269c663f7ecb0d5b395e1e49c409b8d064dbe5f7d6e72172`  
		Last Modified: Wed, 27 Nov 2019 00:53:25 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2935a9205e0bef6cd51d522ccd870fe0dc3ffdea544e47c9ac26be8eb3122`  
		Last Modified: Tue, 03 Dec 2019 23:48:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9e65ee1a4b2ed96c6967fb16eb0de7c63da6bce0c47e3ec63d0c9bd5a237a`  
		Last Modified: Tue, 03 Dec 2019 23:48:49 GMT  
		Size: 111.4 MB (111433459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6a6b8b935e01daa47297ffcd098477b6928da4ffc96f92547c69d47479304f`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27528e779b9e619704d2f2e340fa917637a6413c6f864c8864405df4245b2a2a`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:1bdcfaae6aafbb14428a8892a23124a40f31bd9414e5d2c3b641904db525a5a8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816186803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23192a55795afdee48dc3b3724f1c8a7a93396e95bff38c432c3e559fb9ba27c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:57:29 GMT
ENV MONGO_VERSION=3.6.16
# Wed, 11 Dec 2019 22:57:30 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.16-signed.msi
# Wed, 11 Dec 2019 22:57:32 GMT
ENV MONGO_DOWNLOAD_SHA256=06d8b235702c6a2a4f1b721bbd4b59efbc67d0b9dcd5b4d31984c75946837a2e
# Wed, 11 Dec 2019 23:06:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 23:06:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 23:06:42 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 23:06:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628896678dbc43683e49f91e61271412aa1d97a90b65a2ed04e74157fa49532b`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f11a3aaf5933be1369a1954c04a62d6f707a9e9cde397a42e567f5648e768`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836437d81474147d2932b37b6634ea7d129614983deba273248aae15400c3d08`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c1a30da870a0715c3a3c01c9ab82079b1057836d8b6591a358b85f5c6b8339`  
		Last Modified: Thu, 12 Dec 2019 00:05:41 GMT  
		Size: 93.5 MB (93474561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ece9fda5ed7b5d814b85fdc19ec1154ec7939bc68330c399127bd4e855024`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3ecfc5eca20e232501e1be3e7bcd29af0358074cbe07316e39ff04be2c224`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2833f1058a943a474d0b1fb420d65ba0c50b5b30e8edf26032ec538ed6360beb`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.16`

```console
$ docker pull mongo@sha256:5b5e8a1fe36a8a2b9abb7da88322f17a4388d1bd81479d0f02953621ba02da0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.6.16` - linux; amd64

```console
$ docker pull mongo@sha256:5a2bbd4d98428560888ee895b9fdfe341ed6a2cba5dc5438e64abe2a3adba1f3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165551342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3745fa14a0ed421d031f79653eb1dcb28860988f00ac0ff7f8ae43f0f22f0588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:04 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 19 Dec 2019 07:55:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_MAJOR=3.6
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_VERSION=3.6.16
# Thu, 19 Dec 2019 07:55:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:27 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:27 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:27 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95d19a2f4396aed383bb89fdb2ac0adf5f6d9e4bb8ff3e43e04e7fa066602c`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25973630e92b3431c16828c8add3a7b5cce84c6d9f108d9402afbc1dc96f944b`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f773c926f5697a63c93194ac162c8b30dd710039b822407efdd281f586d2585e`  
		Last Modified: Thu, 19 Dec 2019 07:57:55 GMT  
		Size: 117.2 MB (117228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b4232d63033b58c91ed73644ccdc96aabecb91bf807ba9fd981b5bddb23ff5`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b7a63572970bb41931de8f074b3e4b6694054d7d97f287886f135c8f1bd50a`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.16` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:4d6093c2b1e85db9acfffcf152e936a481fac5af3a05a8d679a9fa1f9923b0b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155040149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ee79b405e7b46538372c16edc6a1549cd7e1f76907fb7070bef7ddc69937f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:49:52 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 Nov 2019 00:49:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:55 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:56 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:57 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:58 GMT
ENV MONGO_MAJOR=3.6
# Tue, 03 Dec 2019 23:47:18 GMT
ENV MONGO_VERSION=3.6.16
# Tue, 03 Dec 2019 23:47:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 03 Dec 2019 23:47:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 03 Dec 2019 23:47:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 03 Dec 2019 23:47:47 GMT
VOLUME [/data/db /data/configdb]
# Tue, 03 Dec 2019 23:47:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Tue, 03 Dec 2019 23:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Dec 2019 23:47:49 GMT
EXPOSE 27017
# Tue, 03 Dec 2019 23:47:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebea15061d7e2a3269c663f7ecb0d5b395e1e49c409b8d064dbe5f7d6e72172`  
		Last Modified: Wed, 27 Nov 2019 00:53:25 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2935a9205e0bef6cd51d522ccd870fe0dc3ffdea544e47c9ac26be8eb3122`  
		Last Modified: Tue, 03 Dec 2019 23:48:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9e65ee1a4b2ed96c6967fb16eb0de7c63da6bce0c47e3ec63d0c9bd5a237a`  
		Last Modified: Tue, 03 Dec 2019 23:48:49 GMT  
		Size: 111.4 MB (111433459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6a6b8b935e01daa47297ffcd098477b6928da4ffc96f92547c69d47479304f`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27528e779b9e619704d2f2e340fa917637a6413c6f864c8864405df4245b2a2a`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.16` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:1bdcfaae6aafbb14428a8892a23124a40f31bd9414e5d2c3b641904db525a5a8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816186803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23192a55795afdee48dc3b3724f1c8a7a93396e95bff38c432c3e559fb9ba27c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:57:29 GMT
ENV MONGO_VERSION=3.6.16
# Wed, 11 Dec 2019 22:57:30 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.16-signed.msi
# Wed, 11 Dec 2019 22:57:32 GMT
ENV MONGO_DOWNLOAD_SHA256=06d8b235702c6a2a4f1b721bbd4b59efbc67d0b9dcd5b4d31984c75946837a2e
# Wed, 11 Dec 2019 23:06:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 23:06:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 23:06:42 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 23:06:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628896678dbc43683e49f91e61271412aa1d97a90b65a2ed04e74157fa49532b`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f11a3aaf5933be1369a1954c04a62d6f707a9e9cde397a42e567f5648e768`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836437d81474147d2932b37b6634ea7d129614983deba273248aae15400c3d08`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c1a30da870a0715c3a3c01c9ab82079b1057836d8b6591a358b85f5c6b8339`  
		Last Modified: Thu, 12 Dec 2019 00:05:41 GMT  
		Size: 93.5 MB (93474561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ece9fda5ed7b5d814b85fdc19ec1154ec7939bc68330c399127bd4e855024`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3ecfc5eca20e232501e1be3e7bcd29af0358074cbe07316e39ff04be2c224`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2833f1058a943a474d0b1fb420d65ba0c50b5b30e8edf26032ec538ed6360beb`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.16-windowsservercore`

```console
$ docker pull mongo@sha256:99c034916b7aa0c476e0e2335038220070762cfec62cc661771ce56326b06404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.6.16-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:1bdcfaae6aafbb14428a8892a23124a40f31bd9414e5d2c3b641904db525a5a8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816186803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23192a55795afdee48dc3b3724f1c8a7a93396e95bff38c432c3e559fb9ba27c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:57:29 GMT
ENV MONGO_VERSION=3.6.16
# Wed, 11 Dec 2019 22:57:30 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.16-signed.msi
# Wed, 11 Dec 2019 22:57:32 GMT
ENV MONGO_DOWNLOAD_SHA256=06d8b235702c6a2a4f1b721bbd4b59efbc67d0b9dcd5b4d31984c75946837a2e
# Wed, 11 Dec 2019 23:06:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 23:06:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 23:06:42 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 23:06:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628896678dbc43683e49f91e61271412aa1d97a90b65a2ed04e74157fa49532b`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f11a3aaf5933be1369a1954c04a62d6f707a9e9cde397a42e567f5648e768`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836437d81474147d2932b37b6634ea7d129614983deba273248aae15400c3d08`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c1a30da870a0715c3a3c01c9ab82079b1057836d8b6591a358b85f5c6b8339`  
		Last Modified: Thu, 12 Dec 2019 00:05:41 GMT  
		Size: 93.5 MB (93474561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ece9fda5ed7b5d814b85fdc19ec1154ec7939bc68330c399127bd4e855024`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3ecfc5eca20e232501e1be3e7bcd29af0358074cbe07316e39ff04be2c224`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2833f1058a943a474d0b1fb420d65ba0c50b5b30e8edf26032ec538ed6360beb`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.16-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:99c034916b7aa0c476e0e2335038220070762cfec62cc661771ce56326b06404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.6.16-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:1bdcfaae6aafbb14428a8892a23124a40f31bd9414e5d2c3b641904db525a5a8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816186803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23192a55795afdee48dc3b3724f1c8a7a93396e95bff38c432c3e559fb9ba27c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:57:29 GMT
ENV MONGO_VERSION=3.6.16
# Wed, 11 Dec 2019 22:57:30 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.16-signed.msi
# Wed, 11 Dec 2019 22:57:32 GMT
ENV MONGO_DOWNLOAD_SHA256=06d8b235702c6a2a4f1b721bbd4b59efbc67d0b9dcd5b4d31984c75946837a2e
# Wed, 11 Dec 2019 23:06:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 23:06:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 23:06:42 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 23:06:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628896678dbc43683e49f91e61271412aa1d97a90b65a2ed04e74157fa49532b`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f11a3aaf5933be1369a1954c04a62d6f707a9e9cde397a42e567f5648e768`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836437d81474147d2932b37b6634ea7d129614983deba273248aae15400c3d08`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c1a30da870a0715c3a3c01c9ab82079b1057836d8b6591a358b85f5c6b8339`  
		Last Modified: Thu, 12 Dec 2019 00:05:41 GMT  
		Size: 93.5 MB (93474561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ece9fda5ed7b5d814b85fdc19ec1154ec7939bc68330c399127bd4e855024`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3ecfc5eca20e232501e1be3e7bcd29af0358074cbe07316e39ff04be2c224`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2833f1058a943a474d0b1fb420d65ba0c50b5b30e8edf26032ec538ed6360beb`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.16-xenial`

```console
$ docker pull mongo@sha256:5db68abf7b74eb658410e6eeda7d3f84405703fa932eb69c00373a5b93fad8b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.16-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:5a2bbd4d98428560888ee895b9fdfe341ed6a2cba5dc5438e64abe2a3adba1f3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165551342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3745fa14a0ed421d031f79653eb1dcb28860988f00ac0ff7f8ae43f0f22f0588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:04 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 19 Dec 2019 07:55:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_MAJOR=3.6
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_VERSION=3.6.16
# Thu, 19 Dec 2019 07:55:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:27 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:27 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:27 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95d19a2f4396aed383bb89fdb2ac0adf5f6d9e4bb8ff3e43e04e7fa066602c`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25973630e92b3431c16828c8add3a7b5cce84c6d9f108d9402afbc1dc96f944b`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f773c926f5697a63c93194ac162c8b30dd710039b822407efdd281f586d2585e`  
		Last Modified: Thu, 19 Dec 2019 07:57:55 GMT  
		Size: 117.2 MB (117228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b4232d63033b58c91ed73644ccdc96aabecb91bf807ba9fd981b5bddb23ff5`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b7a63572970bb41931de8f074b3e4b6694054d7d97f287886f135c8f1bd50a`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.16-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:4d6093c2b1e85db9acfffcf152e936a481fac5af3a05a8d679a9fa1f9923b0b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155040149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ee79b405e7b46538372c16edc6a1549cd7e1f76907fb7070bef7ddc69937f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:49:52 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 Nov 2019 00:49:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:55 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:56 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:57 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:58 GMT
ENV MONGO_MAJOR=3.6
# Tue, 03 Dec 2019 23:47:18 GMT
ENV MONGO_VERSION=3.6.16
# Tue, 03 Dec 2019 23:47:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 03 Dec 2019 23:47:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 03 Dec 2019 23:47:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 03 Dec 2019 23:47:47 GMT
VOLUME [/data/db /data/configdb]
# Tue, 03 Dec 2019 23:47:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Tue, 03 Dec 2019 23:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Dec 2019 23:47:49 GMT
EXPOSE 27017
# Tue, 03 Dec 2019 23:47:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebea15061d7e2a3269c663f7ecb0d5b395e1e49c409b8d064dbe5f7d6e72172`  
		Last Modified: Wed, 27 Nov 2019 00:53:25 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2935a9205e0bef6cd51d522ccd870fe0dc3ffdea544e47c9ac26be8eb3122`  
		Last Modified: Tue, 03 Dec 2019 23:48:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9e65ee1a4b2ed96c6967fb16eb0de7c63da6bce0c47e3ec63d0c9bd5a237a`  
		Last Modified: Tue, 03 Dec 2019 23:48:49 GMT  
		Size: 111.4 MB (111433459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6a6b8b935e01daa47297ffcd098477b6928da4ffc96f92547c69d47479304f`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27528e779b9e619704d2f2e340fa917637a6413c6f864c8864405df4245b2a2a`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:99c034916b7aa0c476e0e2335038220070762cfec62cc661771ce56326b06404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:1bdcfaae6aafbb14428a8892a23124a40f31bd9414e5d2c3b641904db525a5a8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816186803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23192a55795afdee48dc3b3724f1c8a7a93396e95bff38c432c3e559fb9ba27c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:57:29 GMT
ENV MONGO_VERSION=3.6.16
# Wed, 11 Dec 2019 22:57:30 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.16-signed.msi
# Wed, 11 Dec 2019 22:57:32 GMT
ENV MONGO_DOWNLOAD_SHA256=06d8b235702c6a2a4f1b721bbd4b59efbc67d0b9dcd5b4d31984c75946837a2e
# Wed, 11 Dec 2019 23:06:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 23:06:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 23:06:42 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 23:06:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628896678dbc43683e49f91e61271412aa1d97a90b65a2ed04e74157fa49532b`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f11a3aaf5933be1369a1954c04a62d6f707a9e9cde397a42e567f5648e768`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836437d81474147d2932b37b6634ea7d129614983deba273248aae15400c3d08`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c1a30da870a0715c3a3c01c9ab82079b1057836d8b6591a358b85f5c6b8339`  
		Last Modified: Thu, 12 Dec 2019 00:05:41 GMT  
		Size: 93.5 MB (93474561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ece9fda5ed7b5d814b85fdc19ec1154ec7939bc68330c399127bd4e855024`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3ecfc5eca20e232501e1be3e7bcd29af0358074cbe07316e39ff04be2c224`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2833f1058a943a474d0b1fb420d65ba0c50b5b30e8edf26032ec538ed6360beb`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:99c034916b7aa0c476e0e2335038220070762cfec62cc661771ce56326b06404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:1bdcfaae6aafbb14428a8892a23124a40f31bd9414e5d2c3b641904db525a5a8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816186803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23192a55795afdee48dc3b3724f1c8a7a93396e95bff38c432c3e559fb9ba27c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:57:29 GMT
ENV MONGO_VERSION=3.6.16
# Wed, 11 Dec 2019 22:57:30 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.16-signed.msi
# Wed, 11 Dec 2019 22:57:32 GMT
ENV MONGO_DOWNLOAD_SHA256=06d8b235702c6a2a4f1b721bbd4b59efbc67d0b9dcd5b4d31984c75946837a2e
# Wed, 11 Dec 2019 23:06:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 23:06:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 23:06:42 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 23:06:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628896678dbc43683e49f91e61271412aa1d97a90b65a2ed04e74157fa49532b`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f11a3aaf5933be1369a1954c04a62d6f707a9e9cde397a42e567f5648e768`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836437d81474147d2932b37b6634ea7d129614983deba273248aae15400c3d08`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c1a30da870a0715c3a3c01c9ab82079b1057836d8b6591a358b85f5c6b8339`  
		Last Modified: Thu, 12 Dec 2019 00:05:41 GMT  
		Size: 93.5 MB (93474561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ece9fda5ed7b5d814b85fdc19ec1154ec7939bc68330c399127bd4e855024`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3ecfc5eca20e232501e1be3e7bcd29af0358074cbe07316e39ff04be2c224`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2833f1058a943a474d0b1fb420d65ba0c50b5b30e8edf26032ec538ed6360beb`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:5db68abf7b74eb658410e6eeda7d3f84405703fa932eb69c00373a5b93fad8b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:5a2bbd4d98428560888ee895b9fdfe341ed6a2cba5dc5438e64abe2a3adba1f3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165551342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3745fa14a0ed421d031f79653eb1dcb28860988f00ac0ff7f8ae43f0f22f0588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:04 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 19 Dec 2019 07:55:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_MAJOR=3.6
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_VERSION=3.6.16
# Thu, 19 Dec 2019 07:55:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:27 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:27 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:27 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95d19a2f4396aed383bb89fdb2ac0adf5f6d9e4bb8ff3e43e04e7fa066602c`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25973630e92b3431c16828c8add3a7b5cce84c6d9f108d9402afbc1dc96f944b`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f773c926f5697a63c93194ac162c8b30dd710039b822407efdd281f586d2585e`  
		Last Modified: Thu, 19 Dec 2019 07:57:55 GMT  
		Size: 117.2 MB (117228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b4232d63033b58c91ed73644ccdc96aabecb91bf807ba9fd981b5bddb23ff5`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b7a63572970bb41931de8f074b3e4b6694054d7d97f287886f135c8f1bd50a`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:4d6093c2b1e85db9acfffcf152e936a481fac5af3a05a8d679a9fa1f9923b0b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155040149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ee79b405e7b46538372c16edc6a1549cd7e1f76907fb7070bef7ddc69937f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:49:52 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 Nov 2019 00:49:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:55 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:56 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:57 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:58 GMT
ENV MONGO_MAJOR=3.6
# Tue, 03 Dec 2019 23:47:18 GMT
ENV MONGO_VERSION=3.6.16
# Tue, 03 Dec 2019 23:47:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 03 Dec 2019 23:47:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 03 Dec 2019 23:47:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 03 Dec 2019 23:47:47 GMT
VOLUME [/data/db /data/configdb]
# Tue, 03 Dec 2019 23:47:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Tue, 03 Dec 2019 23:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Dec 2019 23:47:49 GMT
EXPOSE 27017
# Tue, 03 Dec 2019 23:47:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebea15061d7e2a3269c663f7ecb0d5b395e1e49c409b8d064dbe5f7d6e72172`  
		Last Modified: Wed, 27 Nov 2019 00:53:25 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2935a9205e0bef6cd51d522ccd870fe0dc3ffdea544e47c9ac26be8eb3122`  
		Last Modified: Tue, 03 Dec 2019 23:48:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9e65ee1a4b2ed96c6967fb16eb0de7c63da6bce0c47e3ec63d0c9bd5a237a`  
		Last Modified: Tue, 03 Dec 2019 23:48:49 GMT  
		Size: 111.4 MB (111433459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6a6b8b935e01daa47297ffcd098477b6928da4ffc96f92547c69d47479304f`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27528e779b9e619704d2f2e340fa917637a6413c6f864c8864405df4245b2a2a`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:99c034916b7aa0c476e0e2335038220070762cfec62cc661771ce56326b06404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:1bdcfaae6aafbb14428a8892a23124a40f31bd9414e5d2c3b641904db525a5a8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816186803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23192a55795afdee48dc3b3724f1c8a7a93396e95bff38c432c3e559fb9ba27c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:57:29 GMT
ENV MONGO_VERSION=3.6.16
# Wed, 11 Dec 2019 22:57:30 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.16-signed.msi
# Wed, 11 Dec 2019 22:57:32 GMT
ENV MONGO_DOWNLOAD_SHA256=06d8b235702c6a2a4f1b721bbd4b59efbc67d0b9dcd5b4d31984c75946837a2e
# Wed, 11 Dec 2019 23:06:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 23:06:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 23:06:42 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 23:06:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628896678dbc43683e49f91e61271412aa1d97a90b65a2ed04e74157fa49532b`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f11a3aaf5933be1369a1954c04a62d6f707a9e9cde397a42e567f5648e768`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836437d81474147d2932b37b6634ea7d129614983deba273248aae15400c3d08`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c1a30da870a0715c3a3c01c9ab82079b1057836d8b6591a358b85f5c6b8339`  
		Last Modified: Thu, 12 Dec 2019 00:05:41 GMT  
		Size: 93.5 MB (93474561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ece9fda5ed7b5d814b85fdc19ec1154ec7939bc68330c399127bd4e855024`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3ecfc5eca20e232501e1be3e7bcd29af0358074cbe07316e39ff04be2c224`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2833f1058a943a474d0b1fb420d65ba0c50b5b30e8edf26032ec538ed6360beb`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:99c034916b7aa0c476e0e2335038220070762cfec62cc661771ce56326b06404
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:1bdcfaae6aafbb14428a8892a23124a40f31bd9414e5d2c3b641904db525a5a8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5816186803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23192a55795afdee48dc3b3724f1c8a7a93396e95bff38c432c3e559fb9ba27c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 22:57:29 GMT
ENV MONGO_VERSION=3.6.16
# Wed, 11 Dec 2019 22:57:30 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.16-signed.msi
# Wed, 11 Dec 2019 22:57:32 GMT
ENV MONGO_DOWNLOAD_SHA256=06d8b235702c6a2a4f1b721bbd4b59efbc67d0b9dcd5b4d31984c75946837a2e
# Wed, 11 Dec 2019 23:06:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 23:06:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 11 Dec 2019 23:06:42 GMT
EXPOSE 27017
# Wed, 11 Dec 2019 23:06:44 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628896678dbc43683e49f91e61271412aa1d97a90b65a2ed04e74157fa49532b`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2f11a3aaf5933be1369a1954c04a62d6f707a9e9cde397a42e567f5648e768`  
		Last Modified: Thu, 12 Dec 2019 00:05:14 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836437d81474147d2932b37b6634ea7d129614983deba273248aae15400c3d08`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c1a30da870a0715c3a3c01c9ab82079b1057836d8b6591a358b85f5c6b8339`  
		Last Modified: Thu, 12 Dec 2019 00:05:41 GMT  
		Size: 93.5 MB (93474561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9ece9fda5ed7b5d814b85fdc19ec1154ec7939bc68330c399127bd4e855024`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d3ecfc5eca20e232501e1be3e7bcd29af0358074cbe07316e39ff04be2c224`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2833f1058a943a474d0b1fb420d65ba0c50b5b30e8edf26032ec538ed6360beb`  
		Last Modified: Thu, 12 Dec 2019 00:05:12 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:5db68abf7b74eb658410e6eeda7d3f84405703fa932eb69c00373a5b93fad8b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:5a2bbd4d98428560888ee895b9fdfe341ed6a2cba5dc5438e64abe2a3adba1f3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165551342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3745fa14a0ed421d031f79653eb1dcb28860988f00ac0ff7f8ae43f0f22f0588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:04 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Thu, 19 Dec 2019 07:55:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_MAJOR=3.6
# Thu, 19 Dec 2019 07:55:06 GMT
ENV MONGO_VERSION=3.6.16
# Thu, 19 Dec 2019 07:55:07 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:26 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:27 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:27 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:27 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:27 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:28 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b95d19a2f4396aed383bb89fdb2ac0adf5f6d9e4bb8ff3e43e04e7fa066602c`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 2.0 KB (1992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25973630e92b3431c16828c8add3a7b5cce84c6d9f108d9402afbc1dc96f944b`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f773c926f5697a63c93194ac162c8b30dd710039b822407efdd281f586d2585e`  
		Last Modified: Thu, 19 Dec 2019 07:57:55 GMT  
		Size: 117.2 MB (117228017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b4232d63033b58c91ed73644ccdc96aabecb91bf807ba9fd981b5bddb23ff5`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b7a63572970bb41931de8f074b3e4b6694054d7d97f287886f135c8f1bd50a`  
		Last Modified: Thu, 19 Dec 2019 07:57:28 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:4d6093c2b1e85db9acfffcf152e936a481fac5af3a05a8d679a9fa1f9923b0b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.0 MB (155040149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ee79b405e7b46538372c16edc6a1549cd7e1f76907fb7070bef7ddc69937f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:49:52 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 27 Nov 2019 00:49:55 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:49:55 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:49:56 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:57 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:49:58 GMT
ENV MONGO_MAJOR=3.6
# Tue, 03 Dec 2019 23:47:18 GMT
ENV MONGO_VERSION=3.6.16
# Tue, 03 Dec 2019 23:47:20 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 03 Dec 2019 23:47:44 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 03 Dec 2019 23:47:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 03 Dec 2019 23:47:47 GMT
VOLUME [/data/db /data/configdb]
# Tue, 03 Dec 2019 23:47:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Tue, 03 Dec 2019 23:47:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Dec 2019 23:47:49 GMT
EXPOSE 27017
# Tue, 03 Dec 2019 23:47:50 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebea15061d7e2a3269c663f7ecb0d5b395e1e49c409b8d064dbe5f7d6e72172`  
		Last Modified: Wed, 27 Nov 2019 00:53:25 GMT  
		Size: 2.0 KB (1997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa2935a9205e0bef6cd51d522ccd870fe0dc3ffdea544e47c9ac26be8eb3122`  
		Last Modified: Tue, 03 Dec 2019 23:48:20 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf9e65ee1a4b2ed96c6967fb16eb0de7c63da6bce0c47e3ec63d0c9bd5a237a`  
		Last Modified: Tue, 03 Dec 2019 23:48:49 GMT  
		Size: 111.4 MB (111433459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6a6b8b935e01daa47297ffcd098477b6928da4ffc96f92547c69d47479304f`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27528e779b9e619704d2f2e340fa917637a6413c6f864c8864405df4245b2a2a`  
		Last Modified: Tue, 03 Dec 2019 23:48:21 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:7a1406bfc05547b33a3b7b112eda6346f42ea93ee06b74d30c4c47dfeca0d5f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; s390x
	-	windows version 10.0.14393.3384; amd64

### `mongo:4` - linux; amd64

```console
$ docker pull mongo@sha256:6b0722ea9876f3ec2210c80d999d262375eb792d9d2fc3a9bd8e4b69af541dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147655657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2e64ac939a4f0c9b7aad9fee09f87f7d7f923f50ddcd9ed20f3f229b998f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:56:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:56:11 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:56:11 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:56:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:56:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:56:22 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 07:56:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 07:56:25 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:56:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:56:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:56:47 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:56:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:56:48 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:56:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3987a82b4c0bd362d09d1a7fd1edfc78a89137cbdacc50c5b6cd429b3ea62c`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f139e08362814e947b28f65ecb2fc0d0d8e148ee87670bfd18ae7eac72776`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 3.0 MB (2981946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acc9c8680b4ef34c307d6a242d3d44c890573e925530c26d87c90b956382fba`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 5.8 MB (5763250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb02df30d947f59d152b388e6103c06e4285c9196c2f843a0a66af4101852870`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae725ef3d2ce8f84a053894c9da91adb522610b8e19bfc1104f2a5d23917221b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f54ed6b43fc7f68e48867ed92aee2aa74f79ce6c1126abd9cbc8c73254a02`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca9e535ddb80ef9667099e120bad5ea344f0fdac99ac816609141cc627b68f6`  
		Last Modified: Thu, 19 Dec 2019 07:58:49 GMT  
		Size: 112.2 MB (112176728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3edad81b2a080bd31ff8ac56daffcad374c66b09429c0da61ab7ea8c7c2dc8`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcf78fe5ae3340460d6e71ffe8ccf750ed5797848fe7bf00644d2340c9589b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 4.0 KB (4007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:76cdaab6ec75306255226b0ba785dd113c2f264320382e88368ae1157f93ddbc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.5 MB (143531232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0000651cfa9056c242a341ec396f1b03a548a1d8486b039d3b6fd5d010751ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 31 Oct 2019 22:41:56 GMT
ADD file:6e6c5c69d7791dc0b62c8d03fc0c5051c6291e08dfc4e11abbdc333bc6f44359 in / 
# Thu, 31 Oct 2019 22:41:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:41:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:42:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:42:01 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:16:28 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 31 Oct 2019 23:16:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:16:46 GMT
ENV GOSU_VERSION=1.11
# Thu, 31 Oct 2019 23:16:46 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 31 Oct 2019 23:17:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 31 Oct 2019 23:17:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 31 Oct 2019 23:17:15 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 31 Oct 2019 23:17:18 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 31 Oct 2019 23:17:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 31 Oct 2019 23:17:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 31 Oct 2019 23:17:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 31 Oct 2019 23:17:19 GMT
ENV MONGO_MAJOR=4.2
# Thu, 31 Oct 2019 23:17:19 GMT
ENV MONGO_VERSION=4.2.1
# Thu, 31 Oct 2019 23:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 31 Oct 2019 23:18:04 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 31 Oct 2019 23:18:06 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 31 Oct 2019 23:18:06 GMT
VOLUME [/data/db /data/configdb]
# Thu, 31 Oct 2019 23:18:07 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 31 Oct 2019 23:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 31 Oct 2019 23:18:08 GMT
EXPOSE 27017
# Thu, 31 Oct 2019 23:18:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:617b55fd1ba95b3ed68226101c9b2568ed00a9b7c50959230d2124648f3a47d2`  
		Last Modified: Thu, 31 Oct 2019 22:43:47 GMT  
		Size: 25.4 MB (25364650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee6ed80b799b3b7d7d66e31ba7e61be1f8d02732bccb1a22d1f14c65f9cea21`  
		Last Modified: Thu, 31 Oct 2019 22:43:42 GMT  
		Size: 36.2 KB (36173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc71634b6bba51b68da661aedfd0876ba93b197653cc94323ca050369bef0bc`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e017bfda3869ce68902d01d6dfb0fe74964f8c598ea31bc77825772e58a122b`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ce05cccebf9f7a410bbace7582d3f6a8a6eb8f969e738365ff52fa41bef56`  
		Last Modified: Thu, 31 Oct 2019 23:18:26 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232ad1433592ae3e49689f9a399155d8cd4cb66e85d3e9a3371f64c5d3767ef5`  
		Last Modified: Thu, 31 Oct 2019 23:18:27 GMT  
		Size: 2.7 MB (2714202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfb83020b47608042582b07eac59bfe53f87d076f429e2030150fce7671fcfc`  
		Last Modified: Thu, 31 Oct 2019 23:18:28 GMT  
		Size: 5.7 MB (5684577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e67294f8ac41b2fbbb98389025f6a2934cd3e85f08b50641d96ce6fd42c5d4`  
		Last Modified: Thu, 31 Oct 2019 23:18:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10477e3f19872878bbd97b9b1d529a9cda966b6dab49c609ca17a815f56eaf03`  
		Last Modified: Thu, 31 Oct 2019 23:18:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd80e3c144d231663b9fc4f19de43fe431596d85adb3fd80db6e1965f649b99`  
		Last Modified: Thu, 31 Oct 2019 23:18:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390cef7a4233b0430f858343c7ffa603238382f6b3d57400fba4bc37dc1fc338`  
		Last Modified: Thu, 31 Oct 2019 23:18:49 GMT  
		Size: 109.7 MB (109722811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab2a7a00460c93578481306a6e5212441ae6f399678d3a0938105339ff3659`  
		Last Modified: Thu, 31 Oct 2019 23:18:24 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729e6c5603fe8d82346fcc9450f163fdd06d4f77ad73e59fca74447aa971f9ba`  
		Last Modified: Thu, 31 Oct 2019 23:18:23 GMT  
		Size: 4.0 KB (4005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:13ce6563c74fbc8f8ab03fe261a51aa437d195b4de031f7ab95f180d2b025721
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:087c8605d05455c2f09d32cd50f03eabc930447618cfadedbc79c14d0d5e6b65
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153377138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f00372ce468134a363f88377dc7446cc931b07f850af336c01de828249a3a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:32 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 19 Dec 2019 07:55:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_MAJOR=4.0
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_VERSION=4.0.14
# Thu, 19 Dec 2019 07:55:36 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:56 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:56 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:56 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700c88b5746a1d9f2e63c4a9ba12bb61a2db16ae76ad09ced51274018ecf3fd`  
		Last Modified: Thu, 19 Dec 2019 07:58:00 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ca6076314ef27db0ac4bf73436f4cdd21fd7deb4f4d53e12041a005c489d95`  
		Last Modified: Thu, 19 Dec 2019 07:58:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ebc88220eba1714e17c5a791a26e68907667581607dd120fa2953a88bc9ba`  
		Last Modified: Thu, 19 Dec 2019 07:58:21 GMT  
		Size: 105.1 MB (105054375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5420018e8c6969648a2df4ad25736ec1bf8f7a1c0ffad957ef018c134b185b4f`  
		Last Modified: Thu, 19 Dec 2019 07:58:01 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840e4807778bf0fe95868f5aee81f73d5038cdecf425e67ede29e07011a670d`  
		Last Modified: Thu, 19 Dec 2019 07:58:01 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:9ddf82530621aa03b5022d543a4bb65edab5fe7b4700f93c44d88661e41f97df
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143108117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da51e3f54231a10fb5cdeec11f4a49994a2d48220412eeefe74d58f999b27422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:50:57 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 27 Nov 2019 00:51:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:51:03 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:51:04 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:51:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:51:10 GMT
ENV MONGO_MAJOR=4.0
# Wed, 18 Dec 2019 00:46:54 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 00:46:58 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 18 Dec 2019 00:47:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 18 Dec 2019 00:47:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 18 Dec 2019 00:47:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 18 Dec 2019 00:47:50 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Wed, 18 Dec 2019 00:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 00:47:52 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 00:47:54 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b88de3f1a87007d7bccff5988808f14d2e9742aed390012fcccb4e6c30281`  
		Last Modified: Wed, 27 Nov 2019 00:54:01 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de33362d170a7c4ee9ae72be6291b36ca3ef68c0f98996b789ee74b69738ec29`  
		Last Modified: Wed, 18 Dec 2019 00:48:18 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d701d32afa1a51a014af1571ecf838ab0ad4360496c2ec6d4e811a76ee174102`  
		Last Modified: Wed, 18 Dec 2019 00:48:46 GMT  
		Size: 99.5 MB (99501992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4aad572d13884594c86616048c94e1ac3d002c4eced4e77acc6a376028e59a`  
		Last Modified: Wed, 18 Dec 2019 00:48:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b364c1fec57b6fbe0329b22e20ca30eedf14970c15391a6dc4589303fa64ebee`  
		Last Modified: Wed, 18 Dec 2019 00:48:18 GMT  
		Size: 4.0 KB (4008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:74565cccc2f0950f377d6160fe7d9b86bb6b1ada52ac51bc240080d7b1b6422b
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5809350991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5c356726d8de7cef78857e9b544ab2099d47798998618bab8382fbd77a051b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Dec 2019 02:39:35 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 02:39:36 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.14-signed.msi
# Wed, 18 Dec 2019 02:39:37 GMT
ENV MONGO_DOWNLOAD_SHA256=0e26339d19056ff6f207204c6c793924ea2579b94d662b00aa82e02f8dd414d1
# Wed, 18 Dec 2019 02:48:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 02:49:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Dec 2019 02:49:04 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 02:49:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1413caa57c145dff404864cbefb604d6918e230804f877fa0795845cb8d4c`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8230971852b457199c036cab528fff4e8d6bfb195113d7241228c089887cd58b`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f2d07bcf9bd4f315762c4314d03c231fd11573b875b2563939f09c6a4a05f`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0642c5f051abfe2943dfca330d79518d0c72fd6895c82663f8ab3f6da524fd`  
		Last Modified: Wed, 18 Dec 2019 02:50:40 GMT  
		Size: 86.6 MB (86638781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3716a2ab4150ccce3c775898a42e00ceb85ac3133f7dda135ab6bea2394ae5f`  
		Last Modified: Wed, 18 Dec 2019 02:50:14 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f02635c78c918e2cc18f550e31351772b4ea3d132c81d809d1285ec5e55e8b`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18e1239ea56e6cec408502d34f0f6480fc048a87fb137f0a71ca4edc8904778`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.14`

```console
$ docker pull mongo@sha256:13ce6563c74fbc8f8ab03fe261a51aa437d195b4de031f7ab95f180d2b025721
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.0.14` - linux; amd64

```console
$ docker pull mongo@sha256:087c8605d05455c2f09d32cd50f03eabc930447618cfadedbc79c14d0d5e6b65
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153377138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f00372ce468134a363f88377dc7446cc931b07f850af336c01de828249a3a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:32 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 19 Dec 2019 07:55:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_MAJOR=4.0
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_VERSION=4.0.14
# Thu, 19 Dec 2019 07:55:36 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:56 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:56 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:56 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700c88b5746a1d9f2e63c4a9ba12bb61a2db16ae76ad09ced51274018ecf3fd`  
		Last Modified: Thu, 19 Dec 2019 07:58:00 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ca6076314ef27db0ac4bf73436f4cdd21fd7deb4f4d53e12041a005c489d95`  
		Last Modified: Thu, 19 Dec 2019 07:58:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ebc88220eba1714e17c5a791a26e68907667581607dd120fa2953a88bc9ba`  
		Last Modified: Thu, 19 Dec 2019 07:58:21 GMT  
		Size: 105.1 MB (105054375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5420018e8c6969648a2df4ad25736ec1bf8f7a1c0ffad957ef018c134b185b4f`  
		Last Modified: Thu, 19 Dec 2019 07:58:01 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840e4807778bf0fe95868f5aee81f73d5038cdecf425e67ede29e07011a670d`  
		Last Modified: Thu, 19 Dec 2019 07:58:01 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.14` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:9ddf82530621aa03b5022d543a4bb65edab5fe7b4700f93c44d88661e41f97df
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143108117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da51e3f54231a10fb5cdeec11f4a49994a2d48220412eeefe74d58f999b27422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:50:57 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 27 Nov 2019 00:51:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:51:03 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:51:04 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:51:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:51:10 GMT
ENV MONGO_MAJOR=4.0
# Wed, 18 Dec 2019 00:46:54 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 00:46:58 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 18 Dec 2019 00:47:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 18 Dec 2019 00:47:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 18 Dec 2019 00:47:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 18 Dec 2019 00:47:50 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Wed, 18 Dec 2019 00:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 00:47:52 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 00:47:54 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b88de3f1a87007d7bccff5988808f14d2e9742aed390012fcccb4e6c30281`  
		Last Modified: Wed, 27 Nov 2019 00:54:01 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de33362d170a7c4ee9ae72be6291b36ca3ef68c0f98996b789ee74b69738ec29`  
		Last Modified: Wed, 18 Dec 2019 00:48:18 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d701d32afa1a51a014af1571ecf838ab0ad4360496c2ec6d4e811a76ee174102`  
		Last Modified: Wed, 18 Dec 2019 00:48:46 GMT  
		Size: 99.5 MB (99501992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4aad572d13884594c86616048c94e1ac3d002c4eced4e77acc6a376028e59a`  
		Last Modified: Wed, 18 Dec 2019 00:48:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b364c1fec57b6fbe0329b22e20ca30eedf14970c15391a6dc4589303fa64ebee`  
		Last Modified: Wed, 18 Dec 2019 00:48:18 GMT  
		Size: 4.0 KB (4008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.14` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:74565cccc2f0950f377d6160fe7d9b86bb6b1ada52ac51bc240080d7b1b6422b
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5809350991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5c356726d8de7cef78857e9b544ab2099d47798998618bab8382fbd77a051b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Dec 2019 02:39:35 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 02:39:36 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.14-signed.msi
# Wed, 18 Dec 2019 02:39:37 GMT
ENV MONGO_DOWNLOAD_SHA256=0e26339d19056ff6f207204c6c793924ea2579b94d662b00aa82e02f8dd414d1
# Wed, 18 Dec 2019 02:48:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 02:49:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Dec 2019 02:49:04 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 02:49:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1413caa57c145dff404864cbefb604d6918e230804f877fa0795845cb8d4c`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8230971852b457199c036cab528fff4e8d6bfb195113d7241228c089887cd58b`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f2d07bcf9bd4f315762c4314d03c231fd11573b875b2563939f09c6a4a05f`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0642c5f051abfe2943dfca330d79518d0c72fd6895c82663f8ab3f6da524fd`  
		Last Modified: Wed, 18 Dec 2019 02:50:40 GMT  
		Size: 86.6 MB (86638781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3716a2ab4150ccce3c775898a42e00ceb85ac3133f7dda135ab6bea2394ae5f`  
		Last Modified: Wed, 18 Dec 2019 02:50:14 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f02635c78c918e2cc18f550e31351772b4ea3d132c81d809d1285ec5e55e8b`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18e1239ea56e6cec408502d34f0f6480fc048a87fb137f0a71ca4edc8904778`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.14-windowsservercore`

```console
$ docker pull mongo@sha256:0a1e7f64ee5271c160df78f2ae0a9b06f799d88bf2e838d7321cc238f66adc5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.0.14-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:74565cccc2f0950f377d6160fe7d9b86bb6b1ada52ac51bc240080d7b1b6422b
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5809350991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5c356726d8de7cef78857e9b544ab2099d47798998618bab8382fbd77a051b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Dec 2019 02:39:35 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 02:39:36 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.14-signed.msi
# Wed, 18 Dec 2019 02:39:37 GMT
ENV MONGO_DOWNLOAD_SHA256=0e26339d19056ff6f207204c6c793924ea2579b94d662b00aa82e02f8dd414d1
# Wed, 18 Dec 2019 02:48:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 02:49:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Dec 2019 02:49:04 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 02:49:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1413caa57c145dff404864cbefb604d6918e230804f877fa0795845cb8d4c`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8230971852b457199c036cab528fff4e8d6bfb195113d7241228c089887cd58b`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f2d07bcf9bd4f315762c4314d03c231fd11573b875b2563939f09c6a4a05f`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0642c5f051abfe2943dfca330d79518d0c72fd6895c82663f8ab3f6da524fd`  
		Last Modified: Wed, 18 Dec 2019 02:50:40 GMT  
		Size: 86.6 MB (86638781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3716a2ab4150ccce3c775898a42e00ceb85ac3133f7dda135ab6bea2394ae5f`  
		Last Modified: Wed, 18 Dec 2019 02:50:14 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f02635c78c918e2cc18f550e31351772b4ea3d132c81d809d1285ec5e55e8b`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18e1239ea56e6cec408502d34f0f6480fc048a87fb137f0a71ca4edc8904778`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.14-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.0.14-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:0a1e7f64ee5271c160df78f2ae0a9b06f799d88bf2e838d7321cc238f66adc5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.0.14-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:74565cccc2f0950f377d6160fe7d9b86bb6b1ada52ac51bc240080d7b1b6422b
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5809350991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5c356726d8de7cef78857e9b544ab2099d47798998618bab8382fbd77a051b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Dec 2019 02:39:35 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 02:39:36 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.14-signed.msi
# Wed, 18 Dec 2019 02:39:37 GMT
ENV MONGO_DOWNLOAD_SHA256=0e26339d19056ff6f207204c6c793924ea2579b94d662b00aa82e02f8dd414d1
# Wed, 18 Dec 2019 02:48:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 02:49:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Dec 2019 02:49:04 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 02:49:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1413caa57c145dff404864cbefb604d6918e230804f877fa0795845cb8d4c`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8230971852b457199c036cab528fff4e8d6bfb195113d7241228c089887cd58b`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f2d07bcf9bd4f315762c4314d03c231fd11573b875b2563939f09c6a4a05f`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0642c5f051abfe2943dfca330d79518d0c72fd6895c82663f8ab3f6da524fd`  
		Last Modified: Wed, 18 Dec 2019 02:50:40 GMT  
		Size: 86.6 MB (86638781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3716a2ab4150ccce3c775898a42e00ceb85ac3133f7dda135ab6bea2394ae5f`  
		Last Modified: Wed, 18 Dec 2019 02:50:14 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f02635c78c918e2cc18f550e31351772b4ea3d132c81d809d1285ec5e55e8b`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18e1239ea56e6cec408502d34f0f6480fc048a87fb137f0a71ca4edc8904778`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.14-xenial`

```console
$ docker pull mongo@sha256:bea714e5c117c34566f015d4fbb05a7de1c38a0d42d9cc7c1e25b0ecb73bed02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0.14-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:087c8605d05455c2f09d32cd50f03eabc930447618cfadedbc79c14d0d5e6b65
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153377138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f00372ce468134a363f88377dc7446cc931b07f850af336c01de828249a3a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:32 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 19 Dec 2019 07:55:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_MAJOR=4.0
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_VERSION=4.0.14
# Thu, 19 Dec 2019 07:55:36 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:56 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:56 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:56 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700c88b5746a1d9f2e63c4a9ba12bb61a2db16ae76ad09ced51274018ecf3fd`  
		Last Modified: Thu, 19 Dec 2019 07:58:00 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ca6076314ef27db0ac4bf73436f4cdd21fd7deb4f4d53e12041a005c489d95`  
		Last Modified: Thu, 19 Dec 2019 07:58:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ebc88220eba1714e17c5a791a26e68907667581607dd120fa2953a88bc9ba`  
		Last Modified: Thu, 19 Dec 2019 07:58:21 GMT  
		Size: 105.1 MB (105054375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5420018e8c6969648a2df4ad25736ec1bf8f7a1c0ffad957ef018c134b185b4f`  
		Last Modified: Thu, 19 Dec 2019 07:58:01 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840e4807778bf0fe95868f5aee81f73d5038cdecf425e67ede29e07011a670d`  
		Last Modified: Thu, 19 Dec 2019 07:58:01 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0.14-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:9ddf82530621aa03b5022d543a4bb65edab5fe7b4700f93c44d88661e41f97df
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143108117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da51e3f54231a10fb5cdeec11f4a49994a2d48220412eeefe74d58f999b27422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:50:57 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 27 Nov 2019 00:51:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:51:03 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:51:04 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:51:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:51:10 GMT
ENV MONGO_MAJOR=4.0
# Wed, 18 Dec 2019 00:46:54 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 00:46:58 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 18 Dec 2019 00:47:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 18 Dec 2019 00:47:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 18 Dec 2019 00:47:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 18 Dec 2019 00:47:50 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Wed, 18 Dec 2019 00:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 00:47:52 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 00:47:54 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b88de3f1a87007d7bccff5988808f14d2e9742aed390012fcccb4e6c30281`  
		Last Modified: Wed, 27 Nov 2019 00:54:01 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de33362d170a7c4ee9ae72be6291b36ca3ef68c0f98996b789ee74b69738ec29`  
		Last Modified: Wed, 18 Dec 2019 00:48:18 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d701d32afa1a51a014af1571ecf838ab0ad4360496c2ec6d4e811a76ee174102`  
		Last Modified: Wed, 18 Dec 2019 00:48:46 GMT  
		Size: 99.5 MB (99501992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4aad572d13884594c86616048c94e1ac3d002c4eced4e77acc6a376028e59a`  
		Last Modified: Wed, 18 Dec 2019 00:48:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b364c1fec57b6fbe0329b22e20ca30eedf14970c15391a6dc4589303fa64ebee`  
		Last Modified: Wed, 18 Dec 2019 00:48:18 GMT  
		Size: 4.0 KB (4008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:0a1e7f64ee5271c160df78f2ae0a9b06f799d88bf2e838d7321cc238f66adc5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:74565cccc2f0950f377d6160fe7d9b86bb6b1ada52ac51bc240080d7b1b6422b
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5809350991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5c356726d8de7cef78857e9b544ab2099d47798998618bab8382fbd77a051b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Dec 2019 02:39:35 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 02:39:36 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.14-signed.msi
# Wed, 18 Dec 2019 02:39:37 GMT
ENV MONGO_DOWNLOAD_SHA256=0e26339d19056ff6f207204c6c793924ea2579b94d662b00aa82e02f8dd414d1
# Wed, 18 Dec 2019 02:48:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 02:49:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Dec 2019 02:49:04 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 02:49:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1413caa57c145dff404864cbefb604d6918e230804f877fa0795845cb8d4c`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8230971852b457199c036cab528fff4e8d6bfb195113d7241228c089887cd58b`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f2d07bcf9bd4f315762c4314d03c231fd11573b875b2563939f09c6a4a05f`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0642c5f051abfe2943dfca330d79518d0c72fd6895c82663f8ab3f6da524fd`  
		Last Modified: Wed, 18 Dec 2019 02:50:40 GMT  
		Size: 86.6 MB (86638781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3716a2ab4150ccce3c775898a42e00ceb85ac3133f7dda135ab6bea2394ae5f`  
		Last Modified: Wed, 18 Dec 2019 02:50:14 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f02635c78c918e2cc18f550e31351772b4ea3d132c81d809d1285ec5e55e8b`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18e1239ea56e6cec408502d34f0f6480fc048a87fb137f0a71ca4edc8904778`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:0a1e7f64ee5271c160df78f2ae0a9b06f799d88bf2e838d7321cc238f66adc5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:74565cccc2f0950f377d6160fe7d9b86bb6b1ada52ac51bc240080d7b1b6422b
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5809350991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5c356726d8de7cef78857e9b544ab2099d47798998618bab8382fbd77a051b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Dec 2019 02:39:35 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 02:39:36 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.14-signed.msi
# Wed, 18 Dec 2019 02:39:37 GMT
ENV MONGO_DOWNLOAD_SHA256=0e26339d19056ff6f207204c6c793924ea2579b94d662b00aa82e02f8dd414d1
# Wed, 18 Dec 2019 02:48:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 02:49:02 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 18 Dec 2019 02:49:04 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 02:49:05 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab1413caa57c145dff404864cbefb604d6918e230804f877fa0795845cb8d4c`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8230971852b457199c036cab528fff4e8d6bfb195113d7241228c089887cd58b`  
		Last Modified: Wed, 18 Dec 2019 02:50:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26f2d07bcf9bd4f315762c4314d03c231fd11573b875b2563939f09c6a4a05f`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0642c5f051abfe2943dfca330d79518d0c72fd6895c82663f8ab3f6da524fd`  
		Last Modified: Wed, 18 Dec 2019 02:50:40 GMT  
		Size: 86.6 MB (86638781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3716a2ab4150ccce3c775898a42e00ceb85ac3133f7dda135ab6bea2394ae5f`  
		Last Modified: Wed, 18 Dec 2019 02:50:14 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f02635c78c918e2cc18f550e31351772b4ea3d132c81d809d1285ec5e55e8b`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18e1239ea56e6cec408502d34f0f6480fc048a87fb137f0a71ca4edc8904778`  
		Last Modified: Wed, 18 Dec 2019 02:50:13 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:bea714e5c117c34566f015d4fbb05a7de1c38a0d42d9cc7c1e25b0ecb73bed02
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:087c8605d05455c2f09d32cd50f03eabc930447618cfadedbc79c14d0d5e6b65
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153377138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f00372ce468134a363f88377dc7446cc931b07f850af336c01de828249a3a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:24:35 GMT
ADD file:f0b8eaa718bc3965b1e8395f5a6bea97c16651b50614e676bb3eaf31335a0045 in / 
# Thu, 19 Dec 2019 04:24:36 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 04:24:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:24:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:24:38 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:54:11 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:54:20 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:54:21 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:54:32 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:54:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:55:32 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Thu, 19 Dec 2019 07:55:33 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:55:33 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:55:34 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_MAJOR=4.0
# Thu, 19 Dec 2019 07:55:34 GMT
ENV MONGO_VERSION=4.0.14
# Thu, 19 Dec 2019 07:55:36 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:55:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:55:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:55:56 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:55:56 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:55:56 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:55:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3386e6af03b043219225367632569465e5ecd47391d1f99a6d265e51bd463a83`  
		Last Modified: Thu, 12 Dec 2019 08:26:09 GMT  
		Size: 44.1 MB (44123254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ac0bbe6c8eeb959337b336ceaa5c3bbbae81e316025f9b94ede453540f2377`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1983a67e104e801fceb1850a375a71fe6b62636ba7a8403d9644f308a6a43f9`  
		Last Modified: Thu, 19 Dec 2019 04:26:00 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0f3a523f04f61db942018321ae122f90d8e3303e243b005e8de9817daf7028`  
		Last Modified: Thu, 19 Dec 2019 04:25:59 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f591f727e69c75104df7aeedd9a7a2ed78fb68362e195d7bf0fd81c76ddec49b`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 2.0 KB (1984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02280e7b7e079703984c5e333041bab0ed5f450e3eec6c2f286c6e112594588`  
		Last Modified: Thu, 19 Dec 2019 07:57:05 GMT  
		Size: 2.9 MB (2946148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54cf1550292608445b26241446d9bc18c06305a5cb573a80853a10009b297`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 1.2 MB (1243901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc6fdc3bb53680e4ecca5771b58ef4f271d8a3b9bf2aaaec4ad0a8c15b36259`  
		Last Modified: Thu, 19 Dec 2019 07:57:04 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700c88b5746a1d9f2e63c4a9ba12bb61a2db16ae76ad09ced51274018ecf3fd`  
		Last Modified: Thu, 19 Dec 2019 07:58:00 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ca6076314ef27db0ac4bf73436f4cdd21fd7deb4f4d53e12041a005c489d95`  
		Last Modified: Thu, 19 Dec 2019 07:58:00 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5ebc88220eba1714e17c5a791a26e68907667581607dd120fa2953a88bc9ba`  
		Last Modified: Thu, 19 Dec 2019 07:58:21 GMT  
		Size: 105.1 MB (105054375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5420018e8c6969648a2df4ad25736ec1bf8f7a1c0ffad957ef018c134b185b4f`  
		Last Modified: Thu, 19 Dec 2019 07:58:01 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6840e4807778bf0fe95868f5aee81f73d5038cdecf425e67ede29e07011a670d`  
		Last Modified: Thu, 19 Dec 2019 07:58:01 GMT  
		Size: 4.0 KB (4010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:9ddf82530621aa03b5022d543a4bb65edab5fe7b4700f93c44d88661e41f97df
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143108117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da51e3f54231a10fb5cdeec11f4a49994a2d48220412eeefe74d58f999b27422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Tue, 26 Nov 2019 23:51:57 GMT
ADD file:2aa99efceecb520e73ba3c7dc167a4fbe6143ce5e9a6499e85dbc75935b3dfab in / 
# Tue, 26 Nov 2019 23:52:01 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 26 Nov 2019 23:52:03 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 26 Nov 2019 23:52:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 26 Nov 2019 23:52:06 GMT
CMD ["/bin/bash"]
# Wed, 27 Nov 2019 00:48:07 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 27 Nov 2019 00:48:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Nov 2019 00:48:27 GMT
ENV GOSU_VERSION=1.11
# Wed, 27 Nov 2019 00:48:28 GMT
ENV JSYAML_VERSION=3.13.0
# Wed, 27 Nov 2019 00:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 27 Nov 2019 00:48:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 27 Nov 2019 00:50:57 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 27 Nov 2019 00:51:02 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 27 Nov 2019 00:51:03 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 27 Nov 2019 00:51:04 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:51:06 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 27 Nov 2019 00:51:10 GMT
ENV MONGO_MAJOR=4.0
# Wed, 18 Dec 2019 00:46:54 GMT
ENV MONGO_VERSION=4.0.14
# Wed, 18 Dec 2019 00:46:58 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 18 Dec 2019 00:47:43 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 18 Dec 2019 00:47:48 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 18 Dec 2019 00:47:49 GMT
VOLUME [/data/db /data/configdb]
# Wed, 18 Dec 2019 00:47:50 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Wed, 18 Dec 2019 00:47:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 00:47:52 GMT
EXPOSE 27017
# Wed, 18 Dec 2019 00:47:54 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:89276bd3590376dfedf96d27b310423c8a1d8c2fe92e4c5a2630aa704b1bb77f`  
		Last Modified: Mon, 11 Nov 2019 15:38:35 GMT  
		Size: 40.0 MB (39951577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a34d6b85b836a6bc6237d1912834f44592a792ab55d92f9ebe1d74973886c6`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bf847b434f33038cc426678c8640251706a59656ef4b0fec6fe3ba88854ab5`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc4652a1718a263f7195a62c1ca8bf0117bcced50af01ac046bd164f523e5e`  
		Last Modified: Tue, 26 Nov 2019 23:52:51 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29654a2b453807f2a2ab77da919c90f470b457feb09082017c2db0cb659cbae8`  
		Last Modified: Wed, 27 Nov 2019 00:52:48 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82801a5d252ba1ad5369119729d06933f6687427ec9b00ed3affee3d7d9e5a5b`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 2.5 MB (2475016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32596fb594dee26ddc2fff00de483a10c3a1e9d0596d9e175424080fd13f6222`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 1.2 MB (1170042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8df7b8db38cf122e5d4240be8c6a69443d07d574e37834d27d6a9316782df11`  
		Last Modified: Wed, 27 Nov 2019 00:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70b88de3f1a87007d7bccff5988808f14d2e9742aed390012fcccb4e6c30281`  
		Last Modified: Wed, 27 Nov 2019 00:54:01 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de33362d170a7c4ee9ae72be6291b36ca3ef68c0f98996b789ee74b69738ec29`  
		Last Modified: Wed, 18 Dec 2019 00:48:18 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d701d32afa1a51a014af1571ecf838ab0ad4360496c2ec6d4e811a76ee174102`  
		Last Modified: Wed, 18 Dec 2019 00:48:46 GMT  
		Size: 99.5 MB (99501992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4aad572d13884594c86616048c94e1ac3d002c4eced4e77acc6a376028e59a`  
		Last Modified: Wed, 18 Dec 2019 00:48:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b364c1fec57b6fbe0329b22e20ca30eedf14970c15391a6dc4589303fa64ebee`  
		Last Modified: Wed, 18 Dec 2019 00:48:18 GMT  
		Size: 4.0 KB (4008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:7a1406bfc05547b33a3b7b112eda6346f42ea93ee06b74d30c4c47dfeca0d5f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; s390x
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:6b0722ea9876f3ec2210c80d999d262375eb792d9d2fc3a9bd8e4b69af541dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147655657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2e64ac939a4f0c9b7aad9fee09f87f7d7f923f50ddcd9ed20f3f229b998f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:56:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:56:11 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:56:11 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:56:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:56:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:56:22 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 07:56:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 07:56:25 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:56:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:56:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:56:47 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:56:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:56:48 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:56:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3987a82b4c0bd362d09d1a7fd1edfc78a89137cbdacc50c5b6cd429b3ea62c`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f139e08362814e947b28f65ecb2fc0d0d8e148ee87670bfd18ae7eac72776`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 3.0 MB (2981946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acc9c8680b4ef34c307d6a242d3d44c890573e925530c26d87c90b956382fba`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 5.8 MB (5763250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb02df30d947f59d152b388e6103c06e4285c9196c2f843a0a66af4101852870`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae725ef3d2ce8f84a053894c9da91adb522610b8e19bfc1104f2a5d23917221b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f54ed6b43fc7f68e48867ed92aee2aa74f79ce6c1126abd9cbc8c73254a02`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca9e535ddb80ef9667099e120bad5ea344f0fdac99ac816609141cc627b68f6`  
		Last Modified: Thu, 19 Dec 2019 07:58:49 GMT  
		Size: 112.2 MB (112176728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3edad81b2a080bd31ff8ac56daffcad374c66b09429c0da61ab7ea8c7c2dc8`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcf78fe5ae3340460d6e71ffe8ccf750ed5797848fe7bf00644d2340c9589b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 4.0 KB (4007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; s390x

```console
$ docker pull mongo@sha256:76cdaab6ec75306255226b0ba785dd113c2f264320382e88368ae1157f93ddbc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.5 MB (143531232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0000651cfa9056c242a341ec396f1b03a548a1d8486b039d3b6fd5d010751ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 31 Oct 2019 22:41:56 GMT
ADD file:6e6c5c69d7791dc0b62c8d03fc0c5051c6291e08dfc4e11abbdc333bc6f44359 in / 
# Thu, 31 Oct 2019 22:41:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:41:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:42:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:42:01 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:16:28 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 31 Oct 2019 23:16:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:16:46 GMT
ENV GOSU_VERSION=1.11
# Thu, 31 Oct 2019 23:16:46 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 31 Oct 2019 23:17:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 31 Oct 2019 23:17:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 31 Oct 2019 23:17:15 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 31 Oct 2019 23:17:18 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 31 Oct 2019 23:17:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 31 Oct 2019 23:17:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 31 Oct 2019 23:17:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 31 Oct 2019 23:17:19 GMT
ENV MONGO_MAJOR=4.2
# Thu, 31 Oct 2019 23:17:19 GMT
ENV MONGO_VERSION=4.2.1
# Thu, 31 Oct 2019 23:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 31 Oct 2019 23:18:04 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 31 Oct 2019 23:18:06 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 31 Oct 2019 23:18:06 GMT
VOLUME [/data/db /data/configdb]
# Thu, 31 Oct 2019 23:18:07 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 31 Oct 2019 23:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 31 Oct 2019 23:18:08 GMT
EXPOSE 27017
# Thu, 31 Oct 2019 23:18:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:617b55fd1ba95b3ed68226101c9b2568ed00a9b7c50959230d2124648f3a47d2`  
		Last Modified: Thu, 31 Oct 2019 22:43:47 GMT  
		Size: 25.4 MB (25364650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee6ed80b799b3b7d7d66e31ba7e61be1f8d02732bccb1a22d1f14c65f9cea21`  
		Last Modified: Thu, 31 Oct 2019 22:43:42 GMT  
		Size: 36.2 KB (36173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc71634b6bba51b68da661aedfd0876ba93b197653cc94323ca050369bef0bc`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e017bfda3869ce68902d01d6dfb0fe74964f8c598ea31bc77825772e58a122b`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ce05cccebf9f7a410bbace7582d3f6a8a6eb8f969e738365ff52fa41bef56`  
		Last Modified: Thu, 31 Oct 2019 23:18:26 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232ad1433592ae3e49689f9a399155d8cd4cb66e85d3e9a3371f64c5d3767ef5`  
		Last Modified: Thu, 31 Oct 2019 23:18:27 GMT  
		Size: 2.7 MB (2714202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfb83020b47608042582b07eac59bfe53f87d076f429e2030150fce7671fcfc`  
		Last Modified: Thu, 31 Oct 2019 23:18:28 GMT  
		Size: 5.7 MB (5684577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e67294f8ac41b2fbbb98389025f6a2934cd3e85f08b50641d96ce6fd42c5d4`  
		Last Modified: Thu, 31 Oct 2019 23:18:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10477e3f19872878bbd97b9b1d529a9cda966b6dab49c609ca17a815f56eaf03`  
		Last Modified: Thu, 31 Oct 2019 23:18:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd80e3c144d231663b9fc4f19de43fe431596d85adb3fd80db6e1965f649b99`  
		Last Modified: Thu, 31 Oct 2019 23:18:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390cef7a4233b0430f858343c7ffa603238382f6b3d57400fba4bc37dc1fc338`  
		Last Modified: Thu, 31 Oct 2019 23:18:49 GMT  
		Size: 109.7 MB (109722811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab2a7a00460c93578481306a6e5212441ae6f399678d3a0938105339ff3659`  
		Last Modified: Thu, 31 Oct 2019 23:18:24 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729e6c5603fe8d82346fcc9450f163fdd06d4f77ad73e59fca74447aa971f9ba`  
		Last Modified: Thu, 31 Oct 2019 23:18:23 GMT  
		Size: 4.0 KB (4005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.2`

```console
$ docker pull mongo@sha256:7777c3fe69717ed5ae05cee81034f44bae025122ad182c0b52a2775660c89002
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.2.2` - linux; amd64

```console
$ docker pull mongo@sha256:6b0722ea9876f3ec2210c80d999d262375eb792d9d2fc3a9bd8e4b69af541dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147655657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2e64ac939a4f0c9b7aad9fee09f87f7d7f923f50ddcd9ed20f3f229b998f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:56:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:56:11 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:56:11 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:56:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:56:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:56:22 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 07:56:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 07:56:25 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:56:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:56:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:56:47 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:56:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:56:48 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:56:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3987a82b4c0bd362d09d1a7fd1edfc78a89137cbdacc50c5b6cd429b3ea62c`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f139e08362814e947b28f65ecb2fc0d0d8e148ee87670bfd18ae7eac72776`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 3.0 MB (2981946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acc9c8680b4ef34c307d6a242d3d44c890573e925530c26d87c90b956382fba`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 5.8 MB (5763250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb02df30d947f59d152b388e6103c06e4285c9196c2f843a0a66af4101852870`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae725ef3d2ce8f84a053894c9da91adb522610b8e19bfc1104f2a5d23917221b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f54ed6b43fc7f68e48867ed92aee2aa74f79ce6c1126abd9cbc8c73254a02`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca9e535ddb80ef9667099e120bad5ea344f0fdac99ac816609141cc627b68f6`  
		Last Modified: Thu, 19 Dec 2019 07:58:49 GMT  
		Size: 112.2 MB (112176728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3edad81b2a080bd31ff8ac56daffcad374c66b09429c0da61ab7ea8c7c2dc8`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcf78fe5ae3340460d6e71ffe8ccf750ed5797848fe7bf00644d2340c9589b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 4.0 KB (4007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.2` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.2-bionic`

```console
$ docker pull mongo@sha256:6ba3c15d697729516ad5df4ca8341afe370bbfc5cfa2a4bf200fe089057e8d2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; s390x

### `mongo:4.2.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:6b0722ea9876f3ec2210c80d999d262375eb792d9d2fc3a9bd8e4b69af541dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147655657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2e64ac939a4f0c9b7aad9fee09f87f7d7f923f50ddcd9ed20f3f229b998f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:56:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:56:11 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:56:11 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:56:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:56:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:56:22 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 07:56:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 07:56:25 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:56:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:56:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:56:47 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:56:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:56:48 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:56:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3987a82b4c0bd362d09d1a7fd1edfc78a89137cbdacc50c5b6cd429b3ea62c`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f139e08362814e947b28f65ecb2fc0d0d8e148ee87670bfd18ae7eac72776`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 3.0 MB (2981946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acc9c8680b4ef34c307d6a242d3d44c890573e925530c26d87c90b956382fba`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 5.8 MB (5763250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb02df30d947f59d152b388e6103c06e4285c9196c2f843a0a66af4101852870`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae725ef3d2ce8f84a053894c9da91adb522610b8e19bfc1104f2a5d23917221b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f54ed6b43fc7f68e48867ed92aee2aa74f79ce6c1126abd9cbc8c73254a02`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca9e535ddb80ef9667099e120bad5ea344f0fdac99ac816609141cc627b68f6`  
		Last Modified: Thu, 19 Dec 2019 07:58:49 GMT  
		Size: 112.2 MB (112176728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3edad81b2a080bd31ff8ac56daffcad374c66b09429c0da61ab7ea8c7c2dc8`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcf78fe5ae3340460d6e71ffe8ccf750ed5797848fe7bf00644d2340c9589b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 4.0 KB (4007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2.2-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:3d5e56c09566b0f95fd32f0bcfc99eee46f74da0ec41bc871e2735cbe9c09d97
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.9 MB (143894061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a605d6b671ea8ee2ae6821789152d9612b551058bd254d04c3a327a9fc032a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 01:18:53 GMT
ADD file:71a0e537d0c67d313ccdb48e99409227ca2b68d50d7b1c82b2d069057dd72491 in / 
# Thu, 19 Dec 2019 01:18:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 01:18:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 01:18:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 01:18:55 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 01:42:03 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 01:42:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 01:42:10 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 01:42:10 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 01:42:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 01:42:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 01:42:23 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 01:42:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 01:42:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 01:42:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 01:42:26 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 01:42:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 01:42:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 01:42:43 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 01:42:43 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 01:42:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 01:42:43 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 01:42:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9015d1e9fd5bbafd5a9ab0a774dfb9d9cc36c1bd9cb89822c3416ab04878e685`  
		Last Modified: Mon, 02 Dec 2019 15:31:08 GMT  
		Size: 25.4 MB (25365188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e1186eb2726687c98475f19f4d0ed50e2da9a171069c5fcfd2f5e04fc656c2`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 36.2 KB (36173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86643ed2fb70b22576aa6d06dc041dbc603accc3240237d6790312c954a872c`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2e9f669fe720fe3dae748411a09729a654978872e3f094ab10eff5c5d2d0cb`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4426b32ce385cc6caa40bc266237d6c1f0a0d58f568e34affb0061ffe9f7a4f3`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce557ed0eff06599219da1b78dab93aa7612a62b12745e6f85add6b13d8e4e5`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 2.7 MB (2714146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed273dfab55f9765527e9373d10e6fb37818316d6b8c44b96f97a7e6feafe90`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 5.7 MB (5684504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0e9d8d16bece187ec54a7319ef541ab58922296db3cc26462c11cc2f4bc952`  
		Last Modified: Thu, 19 Dec 2019 01:42:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22014f74f25ba3c822e2ce8912b84ad308c8dda1fd63abad35c8f4118dae943`  
		Last Modified: Thu, 19 Dec 2019 01:42:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523e2cddffb8908decfe3fb1a5cd9c13ec68c9b73a4eab9527aa9bf5d6d8e7d6`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80672bab6092a8553fd062af8dd1ccd5e02ed0a2923a5ba6c78cd94d9dcc2643`  
		Last Modified: Thu, 19 Dec 2019 01:43:08 GMT  
		Size: 110.1 MB (110085234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becbe2e4c5c090ac1e64a3fa614946a47dbd5ced5a96ce281e351cf60f9ef139`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f62c861a4187932296ed77c6ce3fa9db111bfd1125553946772b142c76beb0`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.2-windowsservercore`

```console
$ docker pull mongo@sha256:0b4c7287582725aa20fa2587f2c4e82bb4a351a36f2a396c4d3e1b43ee68bd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.2.2-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:0b4c7287582725aa20fa2587f2c4e82bb4a351a36f2a396c4d3e1b43ee68bd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.2.2-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:6ba3c15d697729516ad5df4ca8341afe370bbfc5cfa2a4bf200fe089057e8d2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; s390x

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:6b0722ea9876f3ec2210c80d999d262375eb792d9d2fc3a9bd8e4b69af541dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147655657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2e64ac939a4f0c9b7aad9fee09f87f7d7f923f50ddcd9ed20f3f229b998f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:56:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:56:11 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:56:11 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:56:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:56:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:56:22 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 07:56:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 07:56:25 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:56:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:56:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:56:47 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:56:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:56:48 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:56:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3987a82b4c0bd362d09d1a7fd1edfc78a89137cbdacc50c5b6cd429b3ea62c`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f139e08362814e947b28f65ecb2fc0d0d8e148ee87670bfd18ae7eac72776`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 3.0 MB (2981946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acc9c8680b4ef34c307d6a242d3d44c890573e925530c26d87c90b956382fba`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 5.8 MB (5763250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb02df30d947f59d152b388e6103c06e4285c9196c2f843a0a66af4101852870`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae725ef3d2ce8f84a053894c9da91adb522610b8e19bfc1104f2a5d23917221b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f54ed6b43fc7f68e48867ed92aee2aa74f79ce6c1126abd9cbc8c73254a02`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca9e535ddb80ef9667099e120bad5ea344f0fdac99ac816609141cc627b68f6`  
		Last Modified: Thu, 19 Dec 2019 07:58:49 GMT  
		Size: 112.2 MB (112176728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3edad81b2a080bd31ff8ac56daffcad374c66b09429c0da61ab7ea8c7c2dc8`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcf78fe5ae3340460d6e71ffe8ccf750ed5797848fe7bf00644d2340c9589b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 4.0 KB (4007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:3d5e56c09566b0f95fd32f0bcfc99eee46f74da0ec41bc871e2735cbe9c09d97
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.9 MB (143894061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a605d6b671ea8ee2ae6821789152d9612b551058bd254d04c3a327a9fc032a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 01:18:53 GMT
ADD file:71a0e537d0c67d313ccdb48e99409227ca2b68d50d7b1c82b2d069057dd72491 in / 
# Thu, 19 Dec 2019 01:18:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 01:18:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 01:18:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 01:18:55 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 01:42:03 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 01:42:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 01:42:10 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 01:42:10 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 01:42:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 01:42:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 01:42:23 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 01:42:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 01:42:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 01:42:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 01:42:26 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 01:42:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 01:42:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 01:42:43 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 01:42:43 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 01:42:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 01:42:43 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 01:42:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9015d1e9fd5bbafd5a9ab0a774dfb9d9cc36c1bd9cb89822c3416ab04878e685`  
		Last Modified: Mon, 02 Dec 2019 15:31:08 GMT  
		Size: 25.4 MB (25365188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e1186eb2726687c98475f19f4d0ed50e2da9a171069c5fcfd2f5e04fc656c2`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 36.2 KB (36173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86643ed2fb70b22576aa6d06dc041dbc603accc3240237d6790312c954a872c`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2e9f669fe720fe3dae748411a09729a654978872e3f094ab10eff5c5d2d0cb`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4426b32ce385cc6caa40bc266237d6c1f0a0d58f568e34affb0061ffe9f7a4f3`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce557ed0eff06599219da1b78dab93aa7612a62b12745e6f85add6b13d8e4e5`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 2.7 MB (2714146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed273dfab55f9765527e9373d10e6fb37818316d6b8c44b96f97a7e6feafe90`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 5.7 MB (5684504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0e9d8d16bece187ec54a7319ef541ab58922296db3cc26462c11cc2f4bc952`  
		Last Modified: Thu, 19 Dec 2019 01:42:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22014f74f25ba3c822e2ce8912b84ad308c8dda1fd63abad35c8f4118dae943`  
		Last Modified: Thu, 19 Dec 2019 01:42:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523e2cddffb8908decfe3fb1a5cd9c13ec68c9b73a4eab9527aa9bf5d6d8e7d6`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80672bab6092a8553fd062af8dd1ccd5e02ed0a2923a5ba6c78cd94d9dcc2643`  
		Last Modified: Thu, 19 Dec 2019 01:43:08 GMT  
		Size: 110.1 MB (110085234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becbe2e4c5c090ac1e64a3fa614946a47dbd5ced5a96ce281e351cf60f9ef139`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f62c861a4187932296ed77c6ce3fa9db111bfd1125553946772b142c76beb0`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:0b4c7287582725aa20fa2587f2c4e82bb4a351a36f2a396c4d3e1b43ee68bd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:0b4c7287582725aa20fa2587f2c4e82bb4a351a36f2a396c4d3e1b43ee68bd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:6ba3c15d697729516ad5df4ca8341afe370bbfc5cfa2a4bf200fe089057e8d2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:6b0722ea9876f3ec2210c80d999d262375eb792d9d2fc3a9bd8e4b69af541dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147655657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2e64ac939a4f0c9b7aad9fee09f87f7d7f923f50ddcd9ed20f3f229b998f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:56:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:56:11 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:56:11 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:56:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:56:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:56:22 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 07:56:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 07:56:25 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:56:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:56:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:56:47 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:56:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:56:48 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:56:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3987a82b4c0bd362d09d1a7fd1edfc78a89137cbdacc50c5b6cd429b3ea62c`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f139e08362814e947b28f65ecb2fc0d0d8e148ee87670bfd18ae7eac72776`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 3.0 MB (2981946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acc9c8680b4ef34c307d6a242d3d44c890573e925530c26d87c90b956382fba`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 5.8 MB (5763250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb02df30d947f59d152b388e6103c06e4285c9196c2f843a0a66af4101852870`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae725ef3d2ce8f84a053894c9da91adb522610b8e19bfc1104f2a5d23917221b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f54ed6b43fc7f68e48867ed92aee2aa74f79ce6c1126abd9cbc8c73254a02`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca9e535ddb80ef9667099e120bad5ea344f0fdac99ac816609141cc627b68f6`  
		Last Modified: Thu, 19 Dec 2019 07:58:49 GMT  
		Size: 112.2 MB (112176728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3edad81b2a080bd31ff8ac56daffcad374c66b09429c0da61ab7ea8c7c2dc8`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcf78fe5ae3340460d6e71ffe8ccf750ed5797848fe7bf00644d2340c9589b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 4.0 KB (4007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:3d5e56c09566b0f95fd32f0bcfc99eee46f74da0ec41bc871e2735cbe9c09d97
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.9 MB (143894061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a605d6b671ea8ee2ae6821789152d9612b551058bd254d04c3a327a9fc032a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 01:18:53 GMT
ADD file:71a0e537d0c67d313ccdb48e99409227ca2b68d50d7b1c82b2d069057dd72491 in / 
# Thu, 19 Dec 2019 01:18:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 01:18:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 01:18:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 01:18:55 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 01:42:03 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 01:42:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 01:42:10 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 01:42:10 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 01:42:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 01:42:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 01:42:23 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 01:42:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 01:42:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 01:42:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 01:42:26 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 01:42:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 01:42:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 01:42:43 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 01:42:43 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 01:42:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 01:42:43 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 01:42:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9015d1e9fd5bbafd5a9ab0a774dfb9d9cc36c1bd9cb89822c3416ab04878e685`  
		Last Modified: Mon, 02 Dec 2019 15:31:08 GMT  
		Size: 25.4 MB (25365188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e1186eb2726687c98475f19f4d0ed50e2da9a171069c5fcfd2f5e04fc656c2`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 36.2 KB (36173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86643ed2fb70b22576aa6d06dc041dbc603accc3240237d6790312c954a872c`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2e9f669fe720fe3dae748411a09729a654978872e3f094ab10eff5c5d2d0cb`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4426b32ce385cc6caa40bc266237d6c1f0a0d58f568e34affb0061ffe9f7a4f3`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce557ed0eff06599219da1b78dab93aa7612a62b12745e6f85add6b13d8e4e5`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 2.7 MB (2714146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed273dfab55f9765527e9373d10e6fb37818316d6b8c44b96f97a7e6feafe90`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 5.7 MB (5684504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0e9d8d16bece187ec54a7319ef541ab58922296db3cc26462c11cc2f4bc952`  
		Last Modified: Thu, 19 Dec 2019 01:42:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22014f74f25ba3c822e2ce8912b84ad308c8dda1fd63abad35c8f4118dae943`  
		Last Modified: Thu, 19 Dec 2019 01:42:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523e2cddffb8908decfe3fb1a5cd9c13ec68c9b73a4eab9527aa9bf5d6d8e7d6`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80672bab6092a8553fd062af8dd1ccd5e02ed0a2923a5ba6c78cd94d9dcc2643`  
		Last Modified: Thu, 19 Dec 2019 01:43:08 GMT  
		Size: 110.1 MB (110085234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becbe2e4c5c090ac1e64a3fa614946a47dbd5ced5a96ce281e351cf60f9ef139`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f62c861a4187932296ed77c6ce3fa9db111bfd1125553946772b142c76beb0`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:0b4c7287582725aa20fa2587f2c4e82bb4a351a36f2a396c4d3e1b43ee68bd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4-windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:0b4c7287582725aa20fa2587f2c4e82bb4a351a36f2a396c4d3e1b43ee68bd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:6ba3c15d697729516ad5df4ca8341afe370bbfc5cfa2a4bf200fe089057e8d2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:6b0722ea9876f3ec2210c80d999d262375eb792d9d2fc3a9bd8e4b69af541dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147655657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2e64ac939a4f0c9b7aad9fee09f87f7d7f923f50ddcd9ed20f3f229b998f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:56:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:56:11 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:56:11 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:56:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:56:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:56:22 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 07:56:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 07:56:25 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:56:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:56:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:56:47 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:56:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:56:48 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:56:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3987a82b4c0bd362d09d1a7fd1edfc78a89137cbdacc50c5b6cd429b3ea62c`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f139e08362814e947b28f65ecb2fc0d0d8e148ee87670bfd18ae7eac72776`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 3.0 MB (2981946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acc9c8680b4ef34c307d6a242d3d44c890573e925530c26d87c90b956382fba`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 5.8 MB (5763250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb02df30d947f59d152b388e6103c06e4285c9196c2f843a0a66af4101852870`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae725ef3d2ce8f84a053894c9da91adb522610b8e19bfc1104f2a5d23917221b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f54ed6b43fc7f68e48867ed92aee2aa74f79ce6c1126abd9cbc8c73254a02`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca9e535ddb80ef9667099e120bad5ea344f0fdac99ac816609141cc627b68f6`  
		Last Modified: Thu, 19 Dec 2019 07:58:49 GMT  
		Size: 112.2 MB (112176728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3edad81b2a080bd31ff8ac56daffcad374c66b09429c0da61ab7ea8c7c2dc8`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcf78fe5ae3340460d6e71ffe8ccf750ed5797848fe7bf00644d2340c9589b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 4.0 KB (4007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:3d5e56c09566b0f95fd32f0bcfc99eee46f74da0ec41bc871e2735cbe9c09d97
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.9 MB (143894061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a605d6b671ea8ee2ae6821789152d9612b551058bd254d04c3a327a9fc032a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 01:18:53 GMT
ADD file:71a0e537d0c67d313ccdb48e99409227ca2b68d50d7b1c82b2d069057dd72491 in / 
# Thu, 19 Dec 2019 01:18:54 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 01:18:55 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 01:18:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 01:18:55 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 01:42:03 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 01:42:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 01:42:10 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 01:42:10 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 01:42:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 01:42:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 01:42:23 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 01:42:24 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 01:42:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 01:42:25 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 01:42:25 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 01:42:26 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 01:42:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 01:42:42 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 01:42:43 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 01:42:43 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 01:42:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 01:42:43 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 01:42:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:9015d1e9fd5bbafd5a9ab0a774dfb9d9cc36c1bd9cb89822c3416ab04878e685`  
		Last Modified: Mon, 02 Dec 2019 15:31:08 GMT  
		Size: 25.4 MB (25365188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e1186eb2726687c98475f19f4d0ed50e2da9a171069c5fcfd2f5e04fc656c2`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 36.2 KB (36173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86643ed2fb70b22576aa6d06dc041dbc603accc3240237d6790312c954a872c`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2e9f669fe720fe3dae748411a09729a654978872e3f094ab10eff5c5d2d0cb`  
		Last Modified: Thu, 19 Dec 2019 01:19:51 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4426b32ce385cc6caa40bc266237d6c1f0a0d58f568e34affb0061ffe9f7a4f3`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 1.9 KB (1877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce557ed0eff06599219da1b78dab93aa7612a62b12745e6f85add6b13d8e4e5`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 2.7 MB (2714146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed273dfab55f9765527e9373d10e6fb37818316d6b8c44b96f97a7e6feafe90`  
		Last Modified: Thu, 19 Dec 2019 01:42:57 GMT  
		Size: 5.7 MB (5684504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0e9d8d16bece187ec54a7319ef541ab58922296db3cc26462c11cc2f4bc952`  
		Last Modified: Thu, 19 Dec 2019 01:42:56 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22014f74f25ba3c822e2ce8912b84ad308c8dda1fd63abad35c8f4118dae943`  
		Last Modified: Thu, 19 Dec 2019 01:42:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523e2cddffb8908decfe3fb1a5cd9c13ec68c9b73a4eab9527aa9bf5d6d8e7d6`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80672bab6092a8553fd062af8dd1ccd5e02ed0a2923a5ba6c78cd94d9dcc2643`  
		Last Modified: Thu, 19 Dec 2019 01:43:08 GMT  
		Size: 110.1 MB (110085234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:becbe2e4c5c090ac1e64a3fa614946a47dbd5ced5a96ce281e351cf60f9ef139`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f62c861a4187932296ed77c6ce3fa9db111bfd1125553946772b142c76beb0`  
		Last Modified: Thu, 19 Dec 2019 01:42:54 GMT  
		Size: 4.0 KB (4006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:7a1406bfc05547b33a3b7b112eda6346f42ea93ee06b74d30c4c47dfeca0d5f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; s390x
	-	windows version 10.0.14393.3384; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:6b0722ea9876f3ec2210c80d999d262375eb792d9d2fc3a9bd8e4b69af541dc5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147655657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0e2e64ac939a4f0c9b7aad9fee09f87f7d7f923f50ddcd9ed20f3f229b998f8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 19 Dec 2019 04:21:25 GMT
ADD file:53f100793e6c0adfca99977a42bb65cb7971c26e4d6e4499d1c30a1f51f06854 in / 
# Thu, 19 Dec 2019 04:21:26 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 19 Dec 2019 04:21:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 19 Dec 2019 04:21:28 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 19 Dec 2019 04:21:28 GMT
CMD ["/bin/bash"]
# Thu, 19 Dec 2019 07:56:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 19 Dec 2019 07:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Dec 2019 07:56:11 GMT
ENV GOSU_VERSION=1.11
# Thu, 19 Dec 2019 07:56:11 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 19 Dec 2019 07:56:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Dec 2019 07:56:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 19 Dec 2019 07:56:22 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 19 Dec 2019 07:56:23 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 19 Dec 2019 07:56:24 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_MAJOR=4.2
# Thu, 19 Dec 2019 07:56:24 GMT
ENV MONGO_VERSION=4.2.2
# Thu, 19 Dec 2019 07:56:25 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 19 Dec 2019 07:56:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 19 Dec 2019 07:56:47 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 19 Dec 2019 07:56:47 GMT
VOLUME [/data/db /data/configdb]
# Thu, 19 Dec 2019 07:56:48 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 19 Dec 2019 07:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 07:56:48 GMT
EXPOSE 27017
# Thu, 19 Dec 2019 07:56:48 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:2746a4a261c9e18bfd7ff0429c18fd7522acc14fa4c7ec8ab37ba5ebaadbc584`  
		Last Modified: Mon, 02 Dec 2019 13:22:09 GMT  
		Size: 26.7 MB (26689544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d20cdee96111c8acf1858b62655a37ce81ae48648993542b7ac363ac5c0e5`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 35.4 KB (35361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3160e1d0de4061b5b32ee09af687b898921d36ed9556df5910ddc3104449cd`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e37668deea784f47c8726d934adc12b8d20a2b1c50b0b0c18cb62771cd3684`  
		Last Modified: Thu, 19 Dec 2019 04:24:53 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3987a82b4c0bd362d09d1a7fd1edfc78a89137cbdacc50c5b6cd429b3ea62c`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 1.9 KB (1880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f139e08362814e947b28f65ecb2fc0d0d8e148ee87670bfd18ae7eac72776`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 3.0 MB (2981946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acc9c8680b4ef34c307d6a242d3d44c890573e925530c26d87c90b956382fba`  
		Last Modified: Thu, 19 Dec 2019 07:58:28 GMT  
		Size: 5.8 MB (5763250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb02df30d947f59d152b388e6103c06e4285c9196c2f843a0a66af4101852870`  
		Last Modified: Thu, 19 Dec 2019 07:58:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae725ef3d2ce8f84a053894c9da91adb522610b8e19bfc1104f2a5d23917221b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30f54ed6b43fc7f68e48867ed92aee2aa74f79ce6c1126abd9cbc8c73254a02`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca9e535ddb80ef9667099e120bad5ea344f0fdac99ac816609141cc627b68f6`  
		Last Modified: Thu, 19 Dec 2019 07:58:49 GMT  
		Size: 112.2 MB (112176728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3edad81b2a080bd31ff8ac56daffcad374c66b09429c0da61ab7ea8c7c2dc8`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbcf78fe5ae3340460d6e71ffe8ccf750ed5797848fe7bf00644d2340c9589b`  
		Last Modified: Thu, 19 Dec 2019 07:58:26 GMT  
		Size: 4.0 KB (4007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:76cdaab6ec75306255226b0ba785dd113c2f264320382e88368ae1157f93ddbc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.5 MB (143531232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0000651cfa9056c242a341ec396f1b03a548a1d8486b039d3b6fd5d010751ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 31 Oct 2019 22:41:56 GMT
ADD file:6e6c5c69d7791dc0b62c8d03fc0c5051c6291e08dfc4e11abbdc333bc6f44359 in / 
# Thu, 31 Oct 2019 22:41:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 31 Oct 2019 22:41:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 31 Oct 2019 22:42:01 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 31 Oct 2019 22:42:01 GMT
CMD ["/bin/bash"]
# Thu, 31 Oct 2019 23:16:28 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Thu, 31 Oct 2019 23:16:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Thu, 31 Oct 2019 23:16:46 GMT
ENV GOSU_VERSION=1.11
# Thu, 31 Oct 2019 23:16:46 GMT
ENV JSYAML_VERSION=3.13.0
# Thu, 31 Oct 2019 23:17:14 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 31 Oct 2019 23:17:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 31 Oct 2019 23:17:15 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Thu, 31 Oct 2019 23:17:18 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 31 Oct 2019 23:17:18 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 31 Oct 2019 23:17:18 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 31 Oct 2019 23:17:18 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 31 Oct 2019 23:17:19 GMT
ENV MONGO_MAJOR=4.2
# Thu, 31 Oct 2019 23:17:19 GMT
ENV MONGO_VERSION=4.2.1
# Thu, 31 Oct 2019 23:17:21 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 31 Oct 2019 23:18:04 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 31 Oct 2019 23:18:06 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 31 Oct 2019 23:18:06 GMT
VOLUME [/data/db /data/configdb]
# Thu, 31 Oct 2019 23:18:07 GMT
COPY file:021686a669d0d1d1cbb99d6ca84ff8de10577b78ea985b8cdab9d75b347a3bd0 in /usr/local/bin/ 
# Thu, 31 Oct 2019 23:18:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 31 Oct 2019 23:18:08 GMT
EXPOSE 27017
# Thu, 31 Oct 2019 23:18:08 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:617b55fd1ba95b3ed68226101c9b2568ed00a9b7c50959230d2124648f3a47d2`  
		Last Modified: Thu, 31 Oct 2019 22:43:47 GMT  
		Size: 25.4 MB (25364650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee6ed80b799b3b7d7d66e31ba7e61be1f8d02732bccb1a22d1f14c65f9cea21`  
		Last Modified: Thu, 31 Oct 2019 22:43:42 GMT  
		Size: 36.2 KB (36173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc71634b6bba51b68da661aedfd0876ba93b197653cc94323ca050369bef0bc`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e017bfda3869ce68902d01d6dfb0fe74964f8c598ea31bc77825772e58a122b`  
		Last Modified: Thu, 31 Oct 2019 22:43:43 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43ce05cccebf9f7a410bbace7582d3f6a8a6eb8f969e738365ff52fa41bef56`  
		Last Modified: Thu, 31 Oct 2019 23:18:26 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232ad1433592ae3e49689f9a399155d8cd4cb66e85d3e9a3371f64c5d3767ef5`  
		Last Modified: Thu, 31 Oct 2019 23:18:27 GMT  
		Size: 2.7 MB (2714202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfb83020b47608042582b07eac59bfe53f87d076f429e2030150fce7671fcfc`  
		Last Modified: Thu, 31 Oct 2019 23:18:28 GMT  
		Size: 5.7 MB (5684577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e67294f8ac41b2fbbb98389025f6a2934cd3e85f08b50641d96ce6fd42c5d4`  
		Last Modified: Thu, 31 Oct 2019 23:18:25 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10477e3f19872878bbd97b9b1d529a9cda966b6dab49c609ca17a815f56eaf03`  
		Last Modified: Thu, 31 Oct 2019 23:18:24 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd80e3c144d231663b9fc4f19de43fe431596d85adb3fd80db6e1965f649b99`  
		Last Modified: Thu, 31 Oct 2019 23:18:23 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390cef7a4233b0430f858343c7ffa603238382f6b3d57400fba4bc37dc1fc338`  
		Last Modified: Thu, 31 Oct 2019 23:18:49 GMT  
		Size: 109.7 MB (109722811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ab2a7a00460c93578481306a6e5212441ae6f399678d3a0938105339ff3659`  
		Last Modified: Thu, 31 Oct 2019 23:18:24 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729e6c5603fe8d82346fcc9450f163fdd06d4f77ad73e59fca74447aa971f9ba`  
		Last Modified: Thu, 31 Oct 2019 23:18:23 GMT  
		Size: 4.0 KB (4005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:0b4c7287582725aa20fa2587f2c4e82bb4a351a36f2a396c4d3e1b43ee68bd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:windowsservercore` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:0b4c7287582725aa20fa2587f2c4e82bb4a351a36f2a396c4d3e1b43ee68bd06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3384; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.3384; amd64

```console
$ docker pull mongo@sha256:7f7b11bc20a76bc2bbdd24f0fb633bc6e4c3d69c748634e24e07bf350afa34c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5815101921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa68d46d103fed8d23f7fcb23bd8726ec78bfd3c4036e73c9e7eed44da87ce8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Fri, 13 Dec 2019 00:15:57 GMT
ENV MONGO_VERSION=4.2.2
# Fri, 13 Dec 2019 00:15:58 GMT
ENV MONGO_DOWNLOAD_URL=https://downloads.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.2-signed.msi
# Fri, 13 Dec 2019 00:16:00 GMT
ENV MONGO_DOWNLOAD_SHA256=c4574977ea850798329bfdb6e912145f683afd3b28fe363abdf51ead33446a94
# Fri, 13 Dec 2019 00:20:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 	if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Fri, 13 Dec 2019 00:20:54 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 13 Dec 2019 00:20:56 GMT
EXPOSE 27017
# Fri, 13 Dec 2019 00:20:58 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b28bcd63a68b203440f2356482f70ca1865e942cbe525a18b317f6c535f6f83`  
		Last Modified: Fri, 13 Dec 2019 00:21:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e79356dbb03db52b24591c93390b35d1e4a1511102b86931184e1961e7520f`  
		Last Modified: Fri, 13 Dec 2019 00:21:53 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352689d28df863f78580da5553f8d2ddee7fa63063d480125205b31523e1da5e`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d30d05b6c30768a884f8628886aa0cb6b52291a615c55090fd616a66084b204`  
		Last Modified: Fri, 13 Dec 2019 00:22:12 GMT  
		Size: 92.4 MB (92389706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d2166520848a56369a75c263ebcd7f2d2f0bbf64ee1618f003155f308e900b`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec027281e628e8bcc2274807a4953fdb5ee239d94b885a25503c02be7d6befb`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51bab8f1b3148b487dbe01317e58486df5884f3b3c8af99676e3ee60d4fb5c4`  
		Last Modified: Fri, 13 Dec 2019 00:21:51 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
