## `mongo:6-jammy`

```console
$ docker pull mongo@sha256:9f46b495f4c2b27e2ee2358ed08ea3db6b8aea32e8e332adb1b11f96dd65ccc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:6-jammy` - linux; amd64

```console
$ docker pull mongo@sha256:aa24c133e22f38c76f1da1dcf61eeef9591ac1dca8ade4d91179ccc95f5136ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.2 MB (246164752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba6518b3f09682dd2c25d9cc18aa80497341e29347684ba5dca8b587c338023`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:54:06 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 03 Oct 2023 06:54:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:54:21 GMT
ENV GOSU_VERSION=1.16
# Tue, 03 Oct 2023 06:54:21 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 03 Oct 2023 06:54:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 03 Oct 2023 06:54:29 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 03 Oct 2023 06:55:05 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '39BD841E4BE5FB195A65400E6A26B1AE64C3C388'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 03 Oct 2023 06:55:05 GMT
ARG MONGO_PACKAGE=mongodb-org
# Tue, 03 Oct 2023 06:55:05 GMT
ARG MONGO_REPO=repo.mongodb.org
# Tue, 03 Oct 2023 06:55:05 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Tue, 03 Oct 2023 06:55:05 GMT
ENV MONGO_MAJOR=6.0
# Tue, 03 Oct 2023 06:55:06 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu jammy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Fri, 13 Oct 2023 02:00:19 GMT
ENV MONGO_VERSION=6.0.11
# Fri, 13 Oct 2023 02:00:41 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 		${MONGO_PACKAGE}-database=$MONGO_VERSION 		${MONGO_PACKAGE}-database-tools-extra=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Fri, 13 Oct 2023 02:00:43 GMT
VOLUME [/data/db /data/configdb]
# Fri, 13 Oct 2023 02:00:43 GMT
ENV HOME=/data/db
# Fri, 13 Oct 2023 02:00:43 GMT
COPY file:8fc8efb4e3db886ece2de8764459b4ab3e639e636ed08b2e828441229b4f8571 in /usr/local/bin/ 
# Fri, 13 Oct 2023 02:00:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 02:00:43 GMT
EXPOSE 27017
# Fri, 13 Oct 2023 02:00:43 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:707e32e9fc569fee476af9e92ae3d1df8b8e6dca47f9cb31db9d2c922a6de952`  
		Last Modified: Mon, 25 Sep 2023 12:54:05 GMT  
		Size: 30.4 MB (30440869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ac84d07e956a21a84edd5656ca5f8c6a4d46b774a69a9c6bb1307ea3c07a59`  
		Last Modified: Tue, 03 Oct 2023 06:55:58 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce678af55db40aca17e12e2491540b0db04997abe68d23bee7ee26bc679cab62`  
		Last Modified: Tue, 03 Oct 2023 06:55:59 GMT  
		Size: 5.1 MB (5050667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6212b74a0e2a0bf5776404a542f864df8ecd3e8e346afe06b090b8ad91162ff`  
		Last Modified: Tue, 03 Oct 2023 06:55:59 GMT  
		Size: 1.3 MB (1253059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08077ff6df719127adcc0ba3894d9da76284b6f80691d74d4834c4b3f6749aef`  
		Last Modified: Tue, 03 Oct 2023 06:55:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd57de34668892dbc10655c39eb70fb4f53b28b11d6b8497a5279d5611ab01ac`  
		Last Modified: Tue, 03 Oct 2023 06:56:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe042c164d9de20fe1e48789f8120973e7fc29d7d5dc57ce2e2257be52b73147`  
		Last Modified: Tue, 03 Oct 2023 06:56:37 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5cd85b1d0442c256d27312a517ddcf8134baae9602ca8adc6e06193b1cd74d`  
		Last Modified: Fri, 13 Oct 2023 02:01:38 GMT  
		Size: 209.4 MB (209411482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9209cc71c56a75bbded789a9b083509de9adf960720153811be48f2d8d4ca9a5`  
		Last Modified: Fri, 13 Oct 2023 02:01:12 GMT  
		Size: 5.0 KB (4999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:6-jammy` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:ddb0f7acacd34613c5eeb1310c75a53b943dd0bae72630da9a1d791c680aefba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.0 MB (239002082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:685eccb3c04d4f280d4d8bdab552011a45110e25e3d93699de8c79c4486234cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:05:20 GMT
RUN set -eux; 	groupadd --gid 999 --system mongodb; 	useradd --uid 999 --system --gid mongodb --home-dir /data/db mongodb; 	mkdir -p /data/db /data/configdb; 	chown -R mongodb:mongodb /data/db /data/configdb
# Tue, 03 Oct 2023 05:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		gnupg 		jq 		numactl 		procps 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:05:30 GMT
ENV GOSU_VERSION=1.16
# Tue, 03 Oct 2023 05:05:30 GMT
ENV JSYAML_VERSION=3.13.1
# Tue, 03 Oct 2023 05:05:36 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 03 Oct 2023 05:05:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 03 Oct 2023 05:06:09 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	set -- '39BD841E4BE5FB195A65400E6A26B1AE64C3C388'; 	for key; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	mkdir -p /etc/apt/keyrings; 	gpg --batch --export "$@" > /etc/apt/keyrings/mongodb.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 03 Oct 2023 05:06:09 GMT
ARG MONGO_PACKAGE=mongodb-org
# Tue, 03 Oct 2023 05:06:09 GMT
ARG MONGO_REPO=repo.mongodb.org
# Tue, 03 Oct 2023 05:06:09 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Tue, 03 Oct 2023 05:06:10 GMT
ENV MONGO_MAJOR=6.0
# Tue, 03 Oct 2023 05:06:10 GMT
RUN echo "deb [ signed-by=/etc/apt/keyrings/mongodb.gpg ] http://$MONGO_REPO/apt/ubuntu jammy/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Tue, 03 Oct 2023 05:06:10 GMT
ENV MONGO_VERSION=6.0.10
# Tue, 03 Oct 2023 05:06:27 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 		${MONGO_PACKAGE}-database=$MONGO_VERSION 		${MONGO_PACKAGE}-database-tools-extra=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Tue, 03 Oct 2023 05:06:31 GMT
VOLUME [/data/db /data/configdb]
# Tue, 03 Oct 2023 05:06:31 GMT
ENV HOME=/data/db
# Tue, 03 Oct 2023 05:06:31 GMT
COPY file:8fc8efb4e3db886ece2de8764459b4ab3e639e636ed08b2e828441229b4f8571 in /usr/local/bin/ 
# Tue, 03 Oct 2023 05:06:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 05:06:31 GMT
EXPOSE 27017
# Tue, 03 Oct 2023 05:06:31 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:6ea603f1df5e3d23206761eca19fba4cdf4e22d773256cb65b71b730aa5acced`  
		Last Modified: Mon, 25 Sep 2023 17:30:11 GMT  
		Size: 28.4 MB (28392073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e7f50dd3203f7b84dc0002961680b684151760bcb368411e9860375243ebaa`  
		Last Modified: Tue, 03 Oct 2023 05:06:59 GMT  
		Size: 1.8 KB (1842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515a5b396a1e4dad243802f8309d901c2b854defc42ef3b02f01ff8f3a9b44ac`  
		Last Modified: Tue, 03 Oct 2023 05:07:00 GMT  
		Size: 5.0 MB (4994019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6981979503451cde4f8f32f20ad796e9ec88004b24b0fa20a433941dde3cb9`  
		Last Modified: Tue, 03 Oct 2023 05:07:00 GMT  
		Size: 1.2 MB (1186478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ca81d067655ac8527498c273c9654d825c4dafef6ee63680891bca645c3f06`  
		Last Modified: Tue, 03 Oct 2023 05:06:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5665c1d0cf92fcb36e041307cf1b9173c02c7adf2bea25a065112bfa24dc1e`  
		Last Modified: Tue, 03 Oct 2023 05:07:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1bf9e7ee2a74c81c6b4ecb16e208ef3ef77be2782a5f13c5f1b8a850abd255`  
		Last Modified: Tue, 03 Oct 2023 05:07:30 GMT  
		Size: 263.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b1af009197388022e3c4bb2f6f3c95edee76b3aaccbe78757a792196602f07`  
		Last Modified: Tue, 03 Oct 2023 05:07:47 GMT  
		Size: 204.4 MB (204420838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af6db37806333f5d5dbd983ba5e4d78fb56e72b3a0dc0c21678a484ebea8e61`  
		Last Modified: Tue, 03 Oct 2023 05:07:29 GMT  
		Size: 5.0 KB (4997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
