## `mongo:latest`

```console
$ docker pull mongo@sha256:aea63042abdf9a81319d6e9ffc6a381a6af53ae81a849c59d6269c3f233028a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.17763.1999; amd64
	-	windows version 10.0.14393.4467; amd64

### `mongo:latest` - linux; amd64

```console
$ docker pull mongo@sha256:07af8995615b87ab3cc406e5a2a12e6785626a393f8b71ade02708224a4941c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175678431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e120e3fce9ae7e798cdf515db8124b20691ab8805487ddbb2c6bff217a9a109`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:22 GMT
ADD file:900f735ff138e5137cf25ddd85a32a01921ebec26d86704d24b5f12e73a832c2 in / 
# Thu, 17 Jun 2021 23:31:22 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:12:02 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 18 Jun 2021 01:12:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:12:16 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 01:12:16 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 18 Jun 2021 01:12:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 01:12:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 24 Jun 2021 08:51:52 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 08:51:52 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 24 Jun 2021 08:51:52 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 24 Jun 2021 08:51:52 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 24 Jun 2021 08:51:52 GMT
ENV MONGO_MAJOR=4.4
# Thu, 24 Jun 2021 08:51:54 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 24 Jun 2021 08:51:54 GMT
ENV MONGO_VERSION=4.4.6
# Thu, 24 Jun 2021 08:52:17 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 24 Jun 2021 08:52:18 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 24 Jun 2021 08:52:18 GMT
VOLUME [/data/db /data/configdb]
# Thu, 24 Jun 2021 08:52:19 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 24 Jun 2021 08:52:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 08:52:19 GMT
EXPOSE 27017
# Thu, 24 Jun 2021 08:52:19 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:25fa05cd42bd8fabb25d2a6f3f8c9f7ab34637903d00fd2ed1c1d0fa980427dd`  
		Last Modified: Thu, 17 Jun 2021 23:32:41 GMT  
		Size: 26.7 MB (26700706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3380d70bde1cab6b4455704dcce83e027172549216daea62c6190b09bc05c4be`  
		Last Modified: Fri, 18 Jun 2021 01:15:13 GMT  
		Size: 1.9 KB (1876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5e30e9886d48467be1dfb167593ca15886072e71381d7325c81cc55b028cc2`  
		Last Modified: Fri, 18 Jun 2021 01:15:14 GMT  
		Size: 3.0 MB (2978550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6583381983d84a9b981816a22a57d822fe9a7a1dddfd41349d0adbba81437e6`  
		Last Modified: Fri, 18 Jun 2021 01:15:14 GMT  
		Size: 5.8 MB (5829386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7873a283454075db613d13bef6cfbccba2b35e199aac1f0e31675f0c0acf4ace`  
		Last Modified: Fri, 18 Jun 2021 01:15:13 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5550b05263abbb136151b659852e0ca39932121d1242c6bf99f7f1be3c727b7e`  
		Last Modified: Thu, 24 Jun 2021 08:55:44 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c53eb02c3e7424194175bc0c577ab22de262ff571b57c1022dee4b75e861c0`  
		Last Modified: Thu, 24 Jun 2021 08:55:44 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d83d0aa25866b57a2362ae66c305795ec330de08ea624f73ca4e66ead4d070`  
		Last Modified: Thu, 24 Jun 2021 08:56:03 GMT  
		Size: 140.2 MB (140161459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6790a091c8aebeb55197b8f78b14fcfd86832dc2bc796b5183784530daf99d7`  
		Last Modified: Thu, 24 Jun 2021 08:55:44 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc2814c495664143aefc9cadb354a0c5b566d59069cf476a4ea919aa3307be7`  
		Last Modified: Thu, 24 Jun 2021 08:55:44 GMT  
		Size: 4.5 KB (4472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:b29ac5c0d7e5c159d93aa7a3e26769f9485469dbe15c53f824d4458bade992ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.1 MB (168094206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37820292ee475c564d374c6a3f91547f54b28be967049ce1d645250961424cd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 17 Jun 2021 23:53:50 GMT
ADD file:1c098d4ee63884766899c72e542e107525f0b7ade5528de87642587389864bcc in / 
# Thu, 17 Jun 2021 23:53:51 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:40:26 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 18 Jun 2021 00:40:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:40:35 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:40:35 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 18 Jun 2021 00:40:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:40:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 24 Jun 2021 01:42:11 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Thu, 24 Jun 2021 01:42:11 GMT
ARG MONGO_PACKAGE=mongodb-org
# Thu, 24 Jun 2021 01:42:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Thu, 24 Jun 2021 01:42:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Thu, 24 Jun 2021 01:42:12 GMT
ENV MONGO_MAJOR=4.4
# Thu, 24 Jun 2021 01:42:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Thu, 24 Jun 2021 01:42:13 GMT
ENV MONGO_VERSION=4.4.6
# Thu, 24 Jun 2021 01:42:34 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Thu, 24 Jun 2021 01:42:35 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Thu, 24 Jun 2021 01:42:35 GMT
VOLUME [/data/db /data/configdb]
# Thu, 24 Jun 2021 01:42:35 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Thu, 24 Jun 2021 01:42:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 01:42:36 GMT
EXPOSE 27017
# Thu, 24 Jun 2021 01:42:36 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:55c604a74c4b0b41ef666f811f5e160693236be8ea130c6df723480f59cbb9b8`  
		Last Modified: Thu, 17 Jun 2021 23:55:41 GMT  
		Size: 23.7 MB (23728175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ae63d6c1546e327e93b9a70308b895e4f8c0c488d4132554aa456011c2891b`  
		Last Modified: Fri, 18 Jun 2021 00:44:01 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ff824326e40aca12c8e9780428861a9675b5b55366f354c853a4145d2a9006`  
		Last Modified: Fri, 18 Jun 2021 00:44:01 GMT  
		Size: 2.7 MB (2669141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b6fdecd48a8062f5b47dded0087a71f8e3536e6b22f47e96365fb91285431a`  
		Last Modified: Fri, 18 Jun 2021 00:44:01 GMT  
		Size: 5.3 MB (5347199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c801f51a799a12dee09ac710bf7054307a9366c21b1f2bfe7fcd3c57674bba01`  
		Last Modified: Fri, 18 Jun 2021 00:44:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0d5d13b5a67ba70c05caa0f44bc6bafeb18c631a528c9995e1dda56a93841b`  
		Last Modified: Thu, 24 Jun 2021 01:45:37 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3db09273dfd7d2028b4a2743b7e4ca978174f3be30b0d70f4ab80b50b5b88f`  
		Last Modified: Thu, 24 Jun 2021 01:45:36 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b37759c80348ef0aaf989f8178a2d26901ba7bbd900e5de5528203ff1bfde3`  
		Last Modified: Thu, 24 Jun 2021 01:45:56 GMT  
		Size: 136.3 MB (136341350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028795b7afdcd1bf072d3f058a2cb6766aa129b918416151d2289979f6bf4cb`  
		Last Modified: Thu, 24 Jun 2021 01:45:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a279eb2810d6b2e3c56c5587a1cecf2cfd590d2ee93d53da00bc320b08273`  
		Last Modified: Thu, 24 Jun 2021 01:45:36 GMT  
		Size: 4.5 KB (4472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:2f8e2095ed987037b469d2d253b886aa6b428d2693ccfb134c4738b9a762e3b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.5 MB (169487375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6abd099eea9636cf1fb1447b9dbba55a60dc6aab446573cbba1b2212eb8ca734`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Thu, 17 Jun 2021 23:43:50 GMT
ADD file:cc2ee4aea9fbc14df65175678f3768999a62222c448822b8114b0adc46b28e9d in / 
# Thu, 17 Jun 2021 23:43:52 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:44:15 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Fri, 18 Jun 2021 00:44:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:44:28 GMT
ENV GOSU_VERSION=1.12
# Fri, 18 Jun 2021 00:44:28 GMT
ENV JSYAML_VERSION=3.13.1
# Fri, 18 Jun 2021 00:44:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 18 Jun 2021 00:44:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 23:41:48 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '20691EEC35216C63CAF66CE1656408E390CFB1F5'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --export "$@" > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 23 Jun 2021 23:41:48 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 23 Jun 2021 23:41:49 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 23 Jun 2021 23:41:49 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 23 Jun 2021 23:41:49 GMT
ENV MONGO_MAJOR=4.4
# Wed, 23 Jun 2021 23:41:50 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 23 Jun 2021 23:41:50 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 23 Jun 2021 23:42:16 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 23 Jun 2021 23:42:22 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 23 Jun 2021 23:42:22 GMT
VOLUME [/data/db /data/configdb]
# Wed, 23 Jun 2021 23:42:22 GMT
COPY file:1dd28550b0c6cd4baae08342a3beff8f6014f7551c63d060630b98bd44e1f706 in /usr/local/bin/ 
# Wed, 23 Jun 2021 23:42:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 23:42:23 GMT
EXPOSE 27017
# Wed, 23 Jun 2021 23:42:23 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:dc8b9e6580673058ca03527c82f177ec46b88568b02a42351a756002bdb90d3d`  
		Last Modified: Thu, 17 Jun 2021 23:45:21 GMT  
		Size: 25.4 MB (25366169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7460b77c0089aa1451f58f3d1cd77c5f7d68310192c9f7d686038b0721bab63c`  
		Last Modified: Fri, 18 Jun 2021 00:46:15 GMT  
		Size: 1.9 KB (1881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f541d49e19e2ec42fa54a0cac108206c97af0ecd07e423a9e2cecf87c01a8bae`  
		Last Modified: Fri, 18 Jun 2021 00:46:15 GMT  
		Size: 2.7 MB (2708497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61822a88f708bb3dee2da3d16368f16d25c1cfd75b410a04a7061ed0b1ed404`  
		Last Modified: Fri, 18 Jun 2021 00:46:15 GMT  
		Size: 5.7 MB (5747572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0e9e457b7fab51b14df829de92c0451508732cc0904ffdeb129293baa2b0e3`  
		Last Modified: Fri, 18 Jun 2021 00:46:14 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6468ab4b837a2b4e1bd6268a6489bdb350ae893eaf2b349debdcf1cded32a3a0`  
		Last Modified: Wed, 23 Jun 2021 23:42:38 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c9b6369dfa513356b264b41cf0036d70f1265d20f411236ec8ef2c4eeb00b8`  
		Last Modified: Wed, 23 Jun 2021 23:42:38 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77f479ef89484409307d661777ec4b211b5f9cc48fdf6682e0613d361142f58`  
		Last Modified: Wed, 23 Jun 2021 23:42:55 GMT  
		Size: 135.7 MB (135656800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee02b53bdefa7bcd9407a887d703ee020a9dd6bc0562f4137ffbf5cb3c6f793`  
		Last Modified: Wed, 23 Jun 2021 23:42:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6c774acb681023169bbd494113cf0b940fcd4c21a26e26f7eed9c024ead6ff`  
		Last Modified: Wed, 23 Jun 2021 23:42:38 GMT  
		Size: 4.5 KB (4471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1999; amd64

```console
$ docker pull mongo@sha256:f29cf811ea027d47b3f5340a1d5d63d782769c796c1c420995bfc841d1803c43
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2873302372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec15f7149ae28b361ad54f2e2873c4e52589c9055d3a6c69ebae2ecf1fccc62`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sun, 06 Jun 2021 04:28:43 GMT
RUN Install update 1809-amd64
# Wed, 09 Jun 2021 13:15:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 20:38:08 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 09 Jun 2021 20:38:11 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 09 Jun 2021 20:38:14 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 09 Jun 2021 20:40:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 20:40:12 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Jun 2021 20:40:14 GMT
EXPOSE 27017
# Wed, 09 Jun 2021 20:40:17 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:639bb6bb2beb4cfdcacb9f0844344448fe26494665d5fe78a494419f86fbb18f`  
		Size: 923.3 MB (923252167 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae7d2dc4b590128efeafd375d02122e65a2525623ac2be100c1a390caf8a4b49`  
		Last Modified: Wed, 09 Jun 2021 15:28:02 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad0d495f3c090c8857d01c8c5c1d8808a0bd1ebe3acfc68cddc0518c316610`  
		Last Modified: Wed, 09 Jun 2021 21:05:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9348cb301dc54c9ee2b3f8272d11780555f985ea355cee0ce937d0cddaf45720`  
		Last Modified: Wed, 09 Jun 2021 21:05:11 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6903e6d82f07267bb25a20ef882109bed3163557a58cd437a2af16689aa9e5b1`  
		Last Modified: Wed, 09 Jun 2021 21:05:09 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecaf79bf9107c588c097d630b343f685f276e07697d8bb199cd470153d94239e`  
		Last Modified: Wed, 09 Jun 2021 21:06:01 GMT  
		Size: 231.7 MB (231707523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ff79e7a1c0d2cc43105f021997558851fa1b429b657840b2cb3fb7c94f9924`  
		Last Modified: Wed, 09 Jun 2021 21:05:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570c487450715e390654352a901925f1db5f5892e3953b8ace13a9355a429e6f`  
		Last Modified: Wed, 09 Jun 2021 21:05:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5ec238c82175f83e27fc909d6ce4034997893f49209d2100d4225cb9acc2a1`  
		Last Modified: Wed, 09 Jun 2021 21:05:09 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.4467; amd64

```console
$ docker pull mongo@sha256:b01b78e78ff15717c569d71b13f27bad07e0a54b9f22b7d338992aab78a52095
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6501876232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbf1160505acb0d2b0e89f9a079acda8bbcbedd1ce856ce14483d8e4e73a49f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 13:26:15 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Jun 2021 20:40:35 GMT
ENV MONGO_VERSION=4.4.6
# Wed, 09 Jun 2021 20:40:37 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.6-signed.msi
# Wed, 09 Jun 2021 20:40:39 GMT
ENV MONGO_DOWNLOAD_SHA256=ede50e8f8d8c9d23a8ca2cc1c96cdb9bcc1f617930e8bd1d46f21d95d0b555f8
# Wed, 09 Jun 2021 20:43:39 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'/l*v', 'install.log', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=Client,MiscellaneousTools,Router,ServerNoService' 		); 	if (-Not (Test-Path C:\mongodb\bin\mongo.exe -PathType Leaf)) { 		Write-Host 'Installer failed!'; 		Get-Content install.log; 		exit 1; 	}; 	Remove-Item install.log; 		$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 09 Jun 2021 20:43:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Jun 2021 20:43:44 GMT
EXPOSE 27017
# Wed, 09 Jun 2021 20:43:47 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fa4e6085e5538e957ef06561fe1e62dff898da7f4bb577e81da74323aecab2d7`  
		Last Modified: Wed, 09 Jun 2021 15:28:27 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6562d39fa84cb30abdaf8ba85c49633fe3dbbbb574b420d3d6f0b6dcd84612c`  
		Last Modified: Wed, 09 Jun 2021 21:06:20 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632dffa8911cfd4ce0e581711217246f0acb2c9aa23c00d1665325ca9d01474d`  
		Last Modified: Wed, 09 Jun 2021 21:06:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1a10881159fec53a734a20335f669c66ec8fad205ff18837714b08a2e57eb`  
		Last Modified: Wed, 09 Jun 2021 21:06:18 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fea5282878f8bceeabdfa4eee9a3b15fa82046d07b73acc8bede72ed373e6eb`  
		Last Modified: Wed, 09 Jun 2021 21:10:53 GMT  
		Size: 236.1 MB (236139160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b37d1edadef24c3d2d47473839335006c5e263b365ed3421f7da2ac8cf8d87db`  
		Last Modified: Wed, 09 Jun 2021 21:06:18 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11529cee90aaa262ba14cbf27ff16a20766bacb7c7c673522446ebf8ae34b949`  
		Last Modified: Wed, 09 Jun 2021 21:06:18 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c741f47ea5e251f30ac58630bf0c9d48dd7a1cc68e6394f1ad1c5dfe0aed50ed`  
		Last Modified: Wed, 09 Jun 2021 21:06:18 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
