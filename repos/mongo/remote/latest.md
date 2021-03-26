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
