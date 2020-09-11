## `mongo:bionic`

```console
$ docker pull mongo@sha256:aa8e828204ff04bccf0c1b14b088909a45cee540491fb87c2e73e3dcc04b8a93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:bionic` - linux; amd64

```console
$ docker pull mongo@sha256:ebd31eaac273a9544a33387aa859b0a8676565340a40fc824fa7bda686f462f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.0 MB (177977605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3f937574b61a7cf3b2d5c2fb5ced77d942dee48d9f896fc92b74c7f599a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:13:50 GMT
ADD file:5c125b7f411566e9daa738d8cb851098f36197810f06488c2609074296f294b2 in / 
# Wed, 19 Aug 2020 21:13:52 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:13:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:13:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:13:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:28:01 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 23:28:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:28:10 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:28:10 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 23:28:20 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:28:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:28:55 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 19 Aug 2020 23:28:56 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:28:56 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:28:56 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:28:56 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:28:57 GMT
ENV MONGO_MAJOR=4.4
# Wed, 19 Aug 2020 23:28:57 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 23:28:58 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:29:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:29:19 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:29:19 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:29:19 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:29:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:29:20 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:29:20 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:f08d8e2a3ba11bea23cf5c17e8e1c620057412ed05c32d1114640e18d6dd0a43`  
		Last Modified: Sat, 08 Aug 2020 12:21:16 GMT  
		Size: 26.7 MB (26700095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3baa9cb2483bd9c5329a44d9c2fe72535625bbd4308bca95785dd58e72c06365`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5ff4c0b1526abf77c236655f21c8f67a23313291c8b970fe6b469549d8153`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1860925334f940c3145808527480b4f0cba7f01279087fdb27679e4354fba967`  
		Last Modified: Wed, 19 Aug 2020 21:16:44 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d42806c06e6ea9b8e57e1a85104f4abe7794655779b30ab0922d6e260b6ecbe`  
		Last Modified: Wed, 19 Aug 2020 23:30:19 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a9fd2182572ee51138d2326285ebb805398a36a7128efb5bb4c185a41b7c93`  
		Last Modified: Wed, 19 Aug 2020 23:30:20 GMT  
		Size: 3.0 MB (2974250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd6e3f73ab9c7bdbfffb9864ce3a59f3e12a05ce0fc29e72bbf7a75644c0a66`  
		Last Modified: Wed, 19 Aug 2020 23:30:33 GMT  
		Size: 5.8 MB (5824740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ae7a64936b90dbb6f31df757d857f9b7f061dfb2c41ecd26bc421121020055`  
		Last Modified: Wed, 19 Aug 2020 23:30:19 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fde2cb25c5f185b356e76e464b1cf488020dbc36b08e3f8772b9ba578d17e0`  
		Last Modified: Wed, 19 Aug 2020 23:30:40 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bec62fe62fcac9def40a4d4e7923ec50a8f257de75aae1aab367e9ee318f7c7`  
		Last Modified: Wed, 19 Aug 2020 23:30:41 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf4970a1653dff8b5206cd5968b88826aa763365dfb2863b57d3f5150a07265`  
		Last Modified: Wed, 19 Aug 2020 23:31:03 GMT  
		Size: 142.4 MB (142434407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fac3226e166720c443014632380f8c2f0235a478595b3830ea37b1dea66b3e`  
		Last Modified: Wed, 19 Aug 2020 23:30:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bca9c64faf3c11b4b9ec9bee87921bd766d092789c5f7db581d577bde9ab71`  
		Last Modified: Wed, 19 Aug 2020 23:30:40 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:e9b9532697674431014dc4ec9036402cce91b1ef98c88574aadcbf35de59d572
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (167956019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64af8516e3ba4631845a3da1ce49b2feb744ad5bf24167c57809b7896f881b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:29:47 GMT
ADD file:b8316fc82a2cf230ce4af7dcf02ec1d7e56b156cf610af8ed23b64509c77c799 in / 
# Wed, 19 Aug 2020 21:29:51 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:29:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:29:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:29:55 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:34:41 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:34:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:34:58 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:34:59 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:35:21 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:35:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:36:28 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 19 Aug 2020 22:36:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:36:32 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:36:33 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:36:34 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:36:35 GMT
ENV MONGO_MAJOR=4.4
# Fri, 11 Sep 2020 20:41:37 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 11 Sep 2020 20:41:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 11 Sep 2020 20:42:12 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 11 Sep 2020 20:42:15 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 11 Sep 2020 20:42:16 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Sep 2020 20:42:16 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 11 Sep 2020 20:42:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 20:42:18 GMT
EXPOSE 27017
# Fri, 11 Sep 2020 20:42:18 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:237528ba509b2abcdba1ff1344bab27ad56235cdb3c1c131d3587f6fba4d92c9`  
		Last Modified: Sat, 08 Aug 2020 00:25:26 GMT  
		Size: 23.7 MB (23721798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393b96f31d8b2bf3ce9eb4ac49e6c7411defa4057c1791f02f54c14f2de298ec`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 35.2 KB (35203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d82b0e39008d2fa246a0dca4cfa5feb15db58591582a839bd69d5000aa2e96d`  
		Last Modified: Wed, 19 Aug 2020 21:32:13 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ca375b8d34c9bc764ae24791184cba22510f0c002815b4f9766dd0463f5f5e`  
		Last Modified: Wed, 19 Aug 2020 21:32:14 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cd10ab1e6e17027cb82b959a8eb6420dbd7c3c0bd88a2ce2665a0ad699a8e9`  
		Last Modified: Wed, 19 Aug 2020 22:39:06 GMT  
		Size: 1.9 KB (1882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ef9cc938b0965f01421130bc42270e9f9f5e7110f0fbc14a022ddbfce0201f`  
		Last Modified: Wed, 19 Aug 2020 22:39:08 GMT  
		Size: 2.7 MB (2666307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe8e25801e2226753bb65fabe153dc286ea7b8e5e95b2c95a9a4f540e849ace`  
		Last Modified: Wed, 19 Aug 2020 22:39:08 GMT  
		Size: 5.3 MB (5345849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badc5b79591898bf8ae8bc76b9ae071189061c282c67d9dbee1b6ec4d7eb908b`  
		Last Modified: Wed, 19 Aug 2020 22:39:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f9505d215b0619bd0839c604875cd1847658b0362465f50f008991a103d0f4`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850dcca5e8459d40be1920a19ef0b8218c69c62f8d44dd075a2f3fc25a5bf989`  
		Last Modified: Fri, 11 Sep 2020 20:42:42 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeab2d15b2a86b3b672d44e3cf7d4acb6047bcb1d2b6bae512aa72e1c223133e`  
		Last Modified: Fri, 11 Sep 2020 20:43:16 GMT  
		Size: 136.2 MB (136178005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbcd362421b3087e38679d515560d8e873d0613a19eda6c66fd32c2c3a8b956`  
		Last Modified: Fri, 11 Sep 2020 20:42:42 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256c7b9f339b6278fd8f8e49dacb05a1604a4c65e4338434457857ea5fa53d17`  
		Last Modified: Fri, 11 Sep 2020 20:42:42 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:ce9345001055111a15613f4950dae66da5b4a74ca49f3609f4161d9318736651
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172916198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:096d4b5b51fc3c6c7ae4af3f42395e0acc37ed81b180d6a3b2e53da30ae20f60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:10:03 GMT
ADD file:1343b5ae7d875bd32e4eac552ae10c9631788fd97b99bcdeb9f6a9b85c230ba2 in / 
# Wed, 19 Aug 2020 21:10:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:10:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:10:06 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:10:06 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:12:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:12:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:12:22 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:12:22 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:12:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:12:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:13:21 GMT
ENV GPG_KEYS=20691EEC35216C63CAF66CE1656408E390CFB1F5
# Wed, 19 Aug 2020 22:13:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:13:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:13:23 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_MAJOR=4.4
# Fri, 11 Sep 2020 20:41:58 GMT
ENV MONGO_VERSION=4.4.1
# Fri, 11 Sep 2020 20:41:58 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 11 Sep 2020 20:42:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 11 Sep 2020 20:42:23 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Fri, 11 Sep 2020 20:42:23 GMT
VOLUME [/data/db /data/configdb]
# Fri, 11 Sep 2020 20:42:23 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Fri, 11 Sep 2020 20:42:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 20:42:24 GMT
EXPOSE 27017
# Fri, 11 Sep 2020 20:42:24 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:25294e13856fd30261115dbfc6dd49e2d854414d32c9ead824b8183a83620e5c`  
		Last Modified: Mon, 10 Aug 2020 15:49:57 GMT  
		Size: 25.4 MB (25371147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e4b14541a6306ab7ffae9ed980e3ebac039f590869efecf63c6d745e1cde3c`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a02312fb3bccad51789030500218898a262ff17a962d62bb9849c9103d59`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68677136804619b55f0437044d91d7bfe75e0b8013ca953c0d4db40c4d91d6b`  
		Last Modified: Wed, 19 Aug 2020 21:11:08 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81e7a34e26647fba14555c14a023b52889c7b5e17e8639153c9efafe8c3fdf2`  
		Last Modified: Wed, 19 Aug 2020 22:14:18 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963769966bddc69bae82c54cdf6f5cfcd96b71ec904badf61b8d595aa4e4b3b7`  
		Last Modified: Wed, 19 Aug 2020 22:14:19 GMT  
		Size: 2.7 MB (2704616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fdf02b71a4fbcd8357f8f2e9cf031d6686b7ef8df7873938a4fde0ee571f085`  
		Last Modified: Wed, 19 Aug 2020 22:14:19 GMT  
		Size: 5.7 MB (5745356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9afe4dab7ce96f6e957a345a78bcc735582545b3a1e56dfc975cc431a69536`  
		Last Modified: Wed, 19 Aug 2020 22:14:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebde910332d01365f7283d2949bf55cd5e683bd0e824fc3527d2a58aa22d81df`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581151cd353acc8b8b0f4575b0fd6d00f8a3be8f72d41da30ce0c3685db5dbb0`  
		Last Modified: Fri, 11 Sep 2020 20:42:38 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6de7b389942a909dacca78f384d9659987638fd6efbf854975f431defc2548a`  
		Last Modified: Fri, 11 Sep 2020 20:42:56 GMT  
		Size: 139.1 MB (139050054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c846c39e92be04ea132e8f7bdd20bdc27a856c1b3bb770a875ece2c78fa7c4`  
		Last Modified: Fri, 11 Sep 2020 20:42:38 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b41dd45cad0188e7602f74814fd0c161d5ab419fb804988a47b05c8b5fdd52`  
		Last Modified: Fri, 11 Sep 2020 20:42:38 GMT  
		Size: 4.0 KB (3955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
