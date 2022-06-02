## `mongo:focal`

```console
$ docker pull mongo@sha256:981c6dfc81bd306575ff6c25172891e429c1b29abb400829a1384c38c298a9b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:focal` - linux; amd64

```console
$ docker pull mongo@sha256:9130b650eba8e4baa73e1f2996b5f3933d08ded15b96b8a5a79cd44bdb9b66a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.3 MB (245298884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f9bc7425eef00c066378bc1f7d1d0f2a073f809f4091c255347798b163e5d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Mon, 23 May 2022 23:31:01 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 May 2022 23:31:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 23:31:11 GMT
ENV GOSU_VERSION=1.12
# Mon, 23 May 2022 23:31:11 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 23 May 2022 23:31:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 23:31:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 23:31:31 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Mon, 23 May 2022 23:31:31 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 23 May 2022 23:31:31 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 23 May 2022 23:31:31 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 23 May 2022 23:31:31 GMT
ENV MONGO_MAJOR=5.0
# Mon, 23 May 2022 23:31:32 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 02 Jun 2022 18:38:42 GMT
ENV MONGO_VERSION=5.0.9
# Thu, 02 Jun 2022 18:39:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 02 Jun 2022 18:39:10 GMT
VOLUME [/data/db /data/configdb]
# Thu, 02 Jun 2022 18:39:10 GMT
ENV HOME=/data/db
# Thu, 02 Jun 2022 18:39:10 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Thu, 02 Jun 2022 18:39:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Jun 2022 18:39:10 GMT
EXPOSE 27017
# Thu, 02 Jun 2022 18:39:10 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d1e6b0e1ffe42821814ccdbc8ef5a82b419b7a1dcc6c6aa02a0fa3de1ab7bf`  
		Last Modified: Mon, 23 May 2022 23:35:14 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015ccc3eeca855fb936e2159d1daaa6f67b426d845f51cf5f0b4096c3429f523`  
		Last Modified: Mon, 23 May 2022 23:35:14 GMT  
		Size: 3.1 MB (3063970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0129deec1aaf785650249a55f1d7bac4a95e7b18f8ed660a457f6de21f9d4ca5`  
		Last Modified: Mon, 23 May 2022 23:35:15 GMT  
		Size: 6.5 MB (6505826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9522656704457d67a8a3fbd7d890bd495e5bafbfda575955c2eaa93d7ca141`  
		Last Modified: Mon, 23 May 2022 23:35:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42557cfd554b8b44667112e765e385a6bd38e0a2caa0a0f794513db3967bcb87`  
		Last Modified: Mon, 23 May 2022 23:35:11 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e708669a4172efaa52845c967e705784f89fb52c32031b2c3ee646c8bd04b9`  
		Last Modified: Mon, 23 May 2022 23:35:11 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e35f86444432c21d6832869531d42bc3725598188128af095f48347f3c13a79`  
		Last Modified: Thu, 02 Jun 2022 18:40:12 GMT  
		Size: 207.2 MB (207154224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25527cd13ccd66ffb2b8f34ffe9400698bea506640ae80ac49b8d2429a55311`  
		Last Modified: Thu, 02 Jun 2022 18:39:44 GMT  
		Size: 4.9 KB (4947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:focal` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:0ee764d498848174efae8b85289e71adaae5185463b9b8a7a65ebeb51d5cdb2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.8 MB (237800304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:139e6a541a7923c8df93a81f527101c4dfe414cc8d6b22f9361218112d15d2a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Mon, 23 May 2022 23:58:34 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Mon, 23 May 2022 23:58:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 May 2022 23:58:47 GMT
ENV GOSU_VERSION=1.12
# Mon, 23 May 2022 23:58:48 GMT
ENV JSYAML_VERSION=3.13.1
# Mon, 23 May 2022 23:59:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 23 May 2022 23:59:06 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 23 May 2022 23:59:08 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- 'F5679A222C647C87527C2F8CB00A0BD1E2C63C11'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"
# Mon, 23 May 2022 23:59:09 GMT
ARG MONGO_PACKAGE=mongodb-org
# Mon, 23 May 2022 23:59:10 GMT
ARG MONGO_REPO=repo.mongodb.org
# Mon, 23 May 2022 23:59:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Mon, 23 May 2022 23:59:12 GMT
ENV MONGO_MAJOR=5.0
# Mon, 23 May 2022 23:59:13 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu focal/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 02 Jun 2022 18:00:35 GMT
ENV MONGO_VERSION=5.0.9
# Thu, 02 Jun 2022 18:00:59 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 02 Jun 2022 18:01:00 GMT
VOLUME [/data/db /data/configdb]
# Thu, 02 Jun 2022 18:01:00 GMT
ENV HOME=/data/db
# Thu, 02 Jun 2022 18:01:02 GMT
COPY file:ff519c7454e20e6f14c42932b8d6eaee066ed739bfbbd2a6e884d0a7ffeead38 in /usr/local/bin/ 
# Thu, 02 Jun 2022 18:01:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Jun 2022 18:01:03 GMT
EXPOSE 27017
# Thu, 02 Jun 2022 18:01:04 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0512bdaae73cf7907a5372e174d29934ef3d58b8c419189a40baf81b04f43a`  
		Last Modified: Tue, 24 May 2022 00:03:41 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51571d358e429281c0e3ed2ed7f53f21567aef6fe7532e2ec0b188209e61c8ca`  
		Last Modified: Tue, 24 May 2022 00:03:42 GMT  
		Size: 2.9 MB (2911511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa226bdd983047c6f94630a29b97dfac6379c6aab11572a84d338b40ae3635f6`  
		Last Modified: Tue, 24 May 2022 00:03:43 GMT  
		Size: 6.2 MB (6248132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0e3e44d3aceb5be4f15cafd160b7d54476229cb3d006f27cda634aef64be5e`  
		Last Modified: Tue, 24 May 2022 00:03:39 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e106719865e3d888303573607c0a3e28219aa7b352067276bfb931eec1c45686`  
		Last Modified: Tue, 24 May 2022 00:03:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600ad43e7428f314f08b962d6543e2f4facea799bd703f6b6a383a19669bfef6`  
		Last Modified: Tue, 24 May 2022 00:03:39 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943041bc9b737c9be25a9769179bb1a62422adda25ff26541fd90416dc7c20f2`  
		Last Modified: Thu, 02 Jun 2022 18:02:34 GMT  
		Size: 201.5 MB (201462770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c0dd8839074bb1a604367fe8df3d162750e7f8814457531230766bcf15891b`  
		Last Modified: Thu, 02 Jun 2022 18:02:08 GMT  
		Size: 4.9 KB (4947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
