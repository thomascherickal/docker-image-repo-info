<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo`

-	[`mongo:3`](#mongo3)
-	[`mongo:3.6`](#mongo36)
-	[`mongo:3.6.19`](#mongo3619)
-	[`mongo:3.6.19-windowsservercore`](#mongo3619-windowsservercore)
-	[`mongo:3.6.19-windowsservercore-1809`](#mongo3619-windowsservercore-1809)
-	[`mongo:3.6.19-windowsservercore-ltsc2016`](#mongo3619-windowsservercore-ltsc2016)
-	[`mongo:3.6.19-xenial`](#mongo3619-xenial)
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
-	[`mongo:4.0.20`](#mongo4020)
-	[`mongo:4.0.20-windowsservercore`](#mongo4020-windowsservercore)
-	[`mongo:4.0.20-windowsservercore-1809`](#mongo4020-windowsservercore-1809)
-	[`mongo:4.0.20-windowsservercore-ltsc2016`](#mongo4020-windowsservercore-ltsc2016)
-	[`mongo:4.0.20-xenial`](#mongo4020-xenial)
-	[`mongo:4.0-windowsservercore`](#mongo40-windowsservercore)
-	[`mongo:4.0-windowsservercore-1809`](#mongo40-windowsservercore-1809)
-	[`mongo:4.0-windowsservercore-ltsc2016`](#mongo40-windowsservercore-ltsc2016)
-	[`mongo:4.0-xenial`](#mongo40-xenial)
-	[`mongo:4.2`](#mongo42)
-	[`mongo:4.2.9`](#mongo429)
-	[`mongo:4.2.9-bionic`](#mongo429-bionic)
-	[`mongo:4.2.9-windowsservercore`](#mongo429-windowsservercore)
-	[`mongo:4.2.9-windowsservercore-1809`](#mongo429-windowsservercore-1809)
-	[`mongo:4.2.9-windowsservercore-ltsc2016`](#mongo429-windowsservercore-ltsc2016)
-	[`mongo:4.2-bionic`](#mongo42-bionic)
-	[`mongo:4.2-windowsservercore`](#mongo42-windowsservercore)
-	[`mongo:4.2-windowsservercore-1809`](#mongo42-windowsservercore-1809)
-	[`mongo:4.2-windowsservercore-ltsc2016`](#mongo42-windowsservercore-ltsc2016)
-	[`mongo:4.4`](#mongo44)
-	[`mongo:4.4.0`](#mongo440)
-	[`mongo:4.4.0-bionic`](#mongo440-bionic)
-	[`mongo:4.4.0-windowsservercore`](#mongo440-windowsservercore)
-	[`mongo:4.4.0-windowsservercore-1809`](#mongo440-windowsservercore-1809)
-	[`mongo:4.4.0-windowsservercore-ltsc2016`](#mongo440-windowsservercore-ltsc2016)
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
$ docker pull mongo@sha256:0b04b6d6ef3a140c66b2129cd1e3cbdf56fe92815b35b426ef7661918acca0ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:3` - linux; amd64

```console
$ docker pull mongo@sha256:4eaf89ddb158d79817aa55f72c6bb9389f2aad5175cbf53710fd5394aee65d50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (166043159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a9a525de518f0e4a5243677811d5225aedf618c47deefda5bbb34dd49953ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:26:48 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 23:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:26:57 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:26:57 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 23:27:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:27:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:27:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 23:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:27:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:27:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 23:27:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:27:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:27:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:27:29 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:27:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:27:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:27:29 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:27:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d3f5ac1e7d68e1f6a8df1cc0a15e10257b638cb61a4703cf473ebcea4a3cdc`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ee44fa74647a5ac9e7235f860ca1837d7cbdf33ff6b8572273b6e437d82c8`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.9 MB (2904023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4a221d83b214928e24798076a8fd803a47b4b2c1636685fd20bf1b7695f92d`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 1.3 MB (1305145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66157b0856629ea0067df90c67b46de982f5fbd52a5aa6f6867acfb1142f873e`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1feeebf7c67bc3ce058e8211a04baff8dcf79e5c80d81aad5ae0edeb306bc7d`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b223d5499407dd90b8a47cf3cf7ae1727525951cc2db67d7a020e4408a6c08`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1b694ff7b774f225a9592b8c86d459e4bf4143a804c78e1b2819589d5f58c`  
		Last Modified: Wed, 19 Aug 2020 23:29:53 GMT  
		Size: 117.4 MB (117376469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451337765eaa999d705f9378340cfba3ae052480b8baa4f8e1c105e39cbcad83`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740a7d10ecb64180be64c489560fa2a6f8c468e4197d06749ab974d2a467127a`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c0ae3888736d69a12caa6c43b40170b51425cfdf79fa3681f4540861576fce18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155338889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2909f7bf21269c9924ca0c2fa73fc710372552ed29206981463832ceab617d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:31:59 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:32:16 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:32:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:32:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:32:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 22:32:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:32:51 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:32:52 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 22:32:54 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 22:32:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:33:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:33:22 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:33:23 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:33:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:33:26 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:33:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e57371bd09af15391debc536f6839de7e6ebe7295d50c757dd90f1df6a30da`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b81baa9ce507ec53d3e562d07f480173afa304930494fbd5016ce1c973d8a7`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.4 MB (2432322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0017ea2c2557a608f31f58299936c07c02b7ace3893a5023ca8cad1251034d`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 1.2 MB (1232551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7d1adbe02e2dba2f95d6a9d5b4e8b7282501efd56540440feebb899992e8b1`  
		Last Modified: Wed, 19 Aug 2020 22:37:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec57e97f591b600e564b6e8987f319c18ba7a51c04e3fa1f57cb379b5925dd1`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29758a89cbd002946903ddf1bb164da5e54f6ee672fc1bbd9757aa6e6a9489db`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9aeebb1082432123096ff49b22c17906659291e2932c7ef81825d5f5f2bbc`  
		Last Modified: Wed, 19 Aug 2020 22:38:18 GMT  
		Size: 111.6 MB (111590125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb536ab7200c7b9051ccf226346ab245dcae3ff7680246249aefb822d3a1da84`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa474c7c76ae49118086d377ef5d0fe8a4671a0cf1db2f13a351d64dd17c747`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:80f49b88be25266fbaf54ecb8d56874b90ae26396165bfbf065179c75003fb99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6194025093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5311f8a28994a0a93e2d3cbfcbd40156f7c4d3ee7c4d184efb4bb59584320b38`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 18:49:54 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:06:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:06:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:07:00 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:07:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198cf2d877b69a84769db31aa1a2b93d281750d73e202d5b75ffaa69a8455af`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967478fc83677ac2a896f0bf9d0031038706b09d7278a140c9524d2d01b7b381`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e317452c12763747fcf2c95765e29dff9ffb68ea7270e3a9ccdc7d9dba3ab`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baac56e8429e174b6ed91e6632336cd084f51c3b5b4ad02899c645c550e939`  
		Last Modified: Wed, 12 Aug 2020 21:08:37 GMT  
		Size: 455.9 MB (455869774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa8b3165120c50c00f0696a0e05b120cc611bdea09a292f30f9440d9cc23a5f`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a229abf6a7a32b7150ac1685ac5cdbc71054162e40ebb34ccaa566dfb5409`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82549182e3420298ada296c9c35f42c61a338795f0dfa940932ceb3bdcdbd4`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:9821d40c3bf7615e1194856a8ca506eca454270017ddbe3aa029a6a918c0ad9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2791158383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bcfc35477ed09662dc392aaa72a0f2a7145688541990ba39ae5b5ef0555bec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 19:07:11 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:24:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:24:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:24:46 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:24:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9762656745a831a530ed58667d50ac83fc00cf7944c20452cc16c4536078eb`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec1ef6b7bb662d96c44be88a67b782baa8875d690630da539c73de98c39c37`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65b8eef495cdc8c17f8c78eb5f2aa90f04a2399db9604fb497d96ac24761ee`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc50b0d90c9a5e216aa2a362af3bdf1ea6c7f7e6bf7c8a8056b8b12bf39a8`  
		Last Modified: Wed, 12 Aug 2020 21:10:11 GMT  
		Size: 455.3 MB (455283454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d19d7ef440474edbb6f191aa9deb685b5d583b997641e72f0e067eda776cc`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce619af052ee66b3900c4bf2191e209924541192afb0bcf0d935b74cc7dec4`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9851b297d4aaa13fac0de850eb984db23b7a92b5b9f51459926d22c21dc82f05`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6`

```console
$ docker pull mongo@sha256:0b04b6d6ef3a140c66b2129cd1e3cbdf56fe92815b35b426ef7661918acca0ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:3.6` - linux; amd64

```console
$ docker pull mongo@sha256:4eaf89ddb158d79817aa55f72c6bb9389f2aad5175cbf53710fd5394aee65d50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (166043159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a9a525de518f0e4a5243677811d5225aedf618c47deefda5bbb34dd49953ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:26:48 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 23:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:26:57 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:26:57 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 23:27:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:27:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:27:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 23:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:27:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:27:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 23:27:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:27:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:27:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:27:29 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:27:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:27:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:27:29 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:27:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d3f5ac1e7d68e1f6a8df1cc0a15e10257b638cb61a4703cf473ebcea4a3cdc`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ee44fa74647a5ac9e7235f860ca1837d7cbdf33ff6b8572273b6e437d82c8`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.9 MB (2904023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4a221d83b214928e24798076a8fd803a47b4b2c1636685fd20bf1b7695f92d`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 1.3 MB (1305145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66157b0856629ea0067df90c67b46de982f5fbd52a5aa6f6867acfb1142f873e`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1feeebf7c67bc3ce058e8211a04baff8dcf79e5c80d81aad5ae0edeb306bc7d`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b223d5499407dd90b8a47cf3cf7ae1727525951cc2db67d7a020e4408a6c08`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1b694ff7b774f225a9592b8c86d459e4bf4143a804c78e1b2819589d5f58c`  
		Last Modified: Wed, 19 Aug 2020 23:29:53 GMT  
		Size: 117.4 MB (117376469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451337765eaa999d705f9378340cfba3ae052480b8baa4f8e1c105e39cbcad83`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740a7d10ecb64180be64c489560fa2a6f8c468e4197d06749ab974d2a467127a`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c0ae3888736d69a12caa6c43b40170b51425cfdf79fa3681f4540861576fce18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155338889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2909f7bf21269c9924ca0c2fa73fc710372552ed29206981463832ceab617d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:31:59 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:32:16 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:32:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:32:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:32:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 22:32:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:32:51 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:32:52 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 22:32:54 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 22:32:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:33:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:33:22 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:33:23 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:33:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:33:26 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:33:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e57371bd09af15391debc536f6839de7e6ebe7295d50c757dd90f1df6a30da`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b81baa9ce507ec53d3e562d07f480173afa304930494fbd5016ce1c973d8a7`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.4 MB (2432322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0017ea2c2557a608f31f58299936c07c02b7ace3893a5023ca8cad1251034d`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 1.2 MB (1232551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7d1adbe02e2dba2f95d6a9d5b4e8b7282501efd56540440feebb899992e8b1`  
		Last Modified: Wed, 19 Aug 2020 22:37:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec57e97f591b600e564b6e8987f319c18ba7a51c04e3fa1f57cb379b5925dd1`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29758a89cbd002946903ddf1bb164da5e54f6ee672fc1bbd9757aa6e6a9489db`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9aeebb1082432123096ff49b22c17906659291e2932c7ef81825d5f5f2bbc`  
		Last Modified: Wed, 19 Aug 2020 22:38:18 GMT  
		Size: 111.6 MB (111590125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb536ab7200c7b9051ccf226346ab245dcae3ff7680246249aefb822d3a1da84`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa474c7c76ae49118086d377ef5d0fe8a4671a0cf1db2f13a351d64dd17c747`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:80f49b88be25266fbaf54ecb8d56874b90ae26396165bfbf065179c75003fb99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6194025093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5311f8a28994a0a93e2d3cbfcbd40156f7c4d3ee7c4d184efb4bb59584320b38`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 18:49:54 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:06:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:06:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:07:00 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:07:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198cf2d877b69a84769db31aa1a2b93d281750d73e202d5b75ffaa69a8455af`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967478fc83677ac2a896f0bf9d0031038706b09d7278a140c9524d2d01b7b381`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e317452c12763747fcf2c95765e29dff9ffb68ea7270e3a9ccdc7d9dba3ab`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baac56e8429e174b6ed91e6632336cd084f51c3b5b4ad02899c645c550e939`  
		Last Modified: Wed, 12 Aug 2020 21:08:37 GMT  
		Size: 455.9 MB (455869774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa8b3165120c50c00f0696a0e05b120cc611bdea09a292f30f9440d9cc23a5f`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a229abf6a7a32b7150ac1685ac5cdbc71054162e40ebb34ccaa566dfb5409`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82549182e3420298ada296c9c35f42c61a338795f0dfa940932ceb3bdcdbd4`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:9821d40c3bf7615e1194856a8ca506eca454270017ddbe3aa029a6a918c0ad9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2791158383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bcfc35477ed09662dc392aaa72a0f2a7145688541990ba39ae5b5ef0555bec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 19:07:11 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:24:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:24:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:24:46 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:24:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9762656745a831a530ed58667d50ac83fc00cf7944c20452cc16c4536078eb`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec1ef6b7bb662d96c44be88a67b782baa8875d690630da539c73de98c39c37`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65b8eef495cdc8c17f8c78eb5f2aa90f04a2399db9604fb497d96ac24761ee`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc50b0d90c9a5e216aa2a362af3bdf1ea6c7f7e6bf7c8a8056b8b12bf39a8`  
		Last Modified: Wed, 12 Aug 2020 21:10:11 GMT  
		Size: 455.3 MB (455283454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d19d7ef440474edbb6f191aa9deb685b5d583b997641e72f0e067eda776cc`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce619af052ee66b3900c4bf2191e209924541192afb0bcf0d935b74cc7dec4`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9851b297d4aaa13fac0de850eb984db23b7a92b5b9f51459926d22c21dc82f05`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.19`

```console
$ docker pull mongo@sha256:0b04b6d6ef3a140c66b2129cd1e3cbdf56fe92815b35b426ef7661918acca0ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:3.6.19` - linux; amd64

```console
$ docker pull mongo@sha256:4eaf89ddb158d79817aa55f72c6bb9389f2aad5175cbf53710fd5394aee65d50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (166043159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a9a525de518f0e4a5243677811d5225aedf618c47deefda5bbb34dd49953ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:26:48 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 23:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:26:57 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:26:57 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 23:27:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:27:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:27:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 23:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:27:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:27:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 23:27:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:27:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:27:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:27:29 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:27:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:27:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:27:29 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:27:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d3f5ac1e7d68e1f6a8df1cc0a15e10257b638cb61a4703cf473ebcea4a3cdc`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ee44fa74647a5ac9e7235f860ca1837d7cbdf33ff6b8572273b6e437d82c8`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.9 MB (2904023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4a221d83b214928e24798076a8fd803a47b4b2c1636685fd20bf1b7695f92d`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 1.3 MB (1305145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66157b0856629ea0067df90c67b46de982f5fbd52a5aa6f6867acfb1142f873e`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1feeebf7c67bc3ce058e8211a04baff8dcf79e5c80d81aad5ae0edeb306bc7d`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b223d5499407dd90b8a47cf3cf7ae1727525951cc2db67d7a020e4408a6c08`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1b694ff7b774f225a9592b8c86d459e4bf4143a804c78e1b2819589d5f58c`  
		Last Modified: Wed, 19 Aug 2020 23:29:53 GMT  
		Size: 117.4 MB (117376469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451337765eaa999d705f9378340cfba3ae052480b8baa4f8e1c105e39cbcad83`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740a7d10ecb64180be64c489560fa2a6f8c468e4197d06749ab974d2a467127a`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.19` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c0ae3888736d69a12caa6c43b40170b51425cfdf79fa3681f4540861576fce18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155338889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2909f7bf21269c9924ca0c2fa73fc710372552ed29206981463832ceab617d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:31:59 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:32:16 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:32:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:32:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:32:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 22:32:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:32:51 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:32:52 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 22:32:54 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 22:32:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:33:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:33:22 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:33:23 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:33:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:33:26 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:33:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e57371bd09af15391debc536f6839de7e6ebe7295d50c757dd90f1df6a30da`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b81baa9ce507ec53d3e562d07f480173afa304930494fbd5016ce1c973d8a7`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.4 MB (2432322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0017ea2c2557a608f31f58299936c07c02b7ace3893a5023ca8cad1251034d`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 1.2 MB (1232551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7d1adbe02e2dba2f95d6a9d5b4e8b7282501efd56540440feebb899992e8b1`  
		Last Modified: Wed, 19 Aug 2020 22:37:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec57e97f591b600e564b6e8987f319c18ba7a51c04e3fa1f57cb379b5925dd1`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29758a89cbd002946903ddf1bb164da5e54f6ee672fc1bbd9757aa6e6a9489db`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9aeebb1082432123096ff49b22c17906659291e2932c7ef81825d5f5f2bbc`  
		Last Modified: Wed, 19 Aug 2020 22:38:18 GMT  
		Size: 111.6 MB (111590125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb536ab7200c7b9051ccf226346ab245dcae3ff7680246249aefb822d3a1da84`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa474c7c76ae49118086d377ef5d0fe8a4671a0cf1db2f13a351d64dd17c747`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.19` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:80f49b88be25266fbaf54ecb8d56874b90ae26396165bfbf065179c75003fb99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6194025093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5311f8a28994a0a93e2d3cbfcbd40156f7c4d3ee7c4d184efb4bb59584320b38`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 18:49:54 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:06:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:06:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:07:00 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:07:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198cf2d877b69a84769db31aa1a2b93d281750d73e202d5b75ffaa69a8455af`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967478fc83677ac2a896f0bf9d0031038706b09d7278a140c9524d2d01b7b381`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e317452c12763747fcf2c95765e29dff9ffb68ea7270e3a9ccdc7d9dba3ab`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baac56e8429e174b6ed91e6632336cd084f51c3b5b4ad02899c645c550e939`  
		Last Modified: Wed, 12 Aug 2020 21:08:37 GMT  
		Size: 455.9 MB (455869774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa8b3165120c50c00f0696a0e05b120cc611bdea09a292f30f9440d9cc23a5f`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a229abf6a7a32b7150ac1685ac5cdbc71054162e40ebb34ccaa566dfb5409`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82549182e3420298ada296c9c35f42c61a338795f0dfa940932ceb3bdcdbd4`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.19` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:9821d40c3bf7615e1194856a8ca506eca454270017ddbe3aa029a6a918c0ad9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2791158383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bcfc35477ed09662dc392aaa72a0f2a7145688541990ba39ae5b5ef0555bec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 19:07:11 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:24:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:24:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:24:46 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:24:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9762656745a831a530ed58667d50ac83fc00cf7944c20452cc16c4536078eb`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec1ef6b7bb662d96c44be88a67b782baa8875d690630da539c73de98c39c37`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65b8eef495cdc8c17f8c78eb5f2aa90f04a2399db9604fb497d96ac24761ee`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc50b0d90c9a5e216aa2a362af3bdf1ea6c7f7e6bf7c8a8056b8b12bf39a8`  
		Last Modified: Wed, 12 Aug 2020 21:10:11 GMT  
		Size: 455.3 MB (455283454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d19d7ef440474edbb6f191aa9deb685b5d583b997641e72f0e067eda776cc`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce619af052ee66b3900c4bf2191e209924541192afb0bcf0d935b74cc7dec4`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9851b297d4aaa13fac0de850eb984db23b7a92b5b9f51459926d22c21dc82f05`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.19-windowsservercore`

```console
$ docker pull mongo@sha256:92283737b545079e7143ae61f3194a387f430aa11f1c8683af094cfe476bba58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:3.6.19-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:80f49b88be25266fbaf54ecb8d56874b90ae26396165bfbf065179c75003fb99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6194025093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5311f8a28994a0a93e2d3cbfcbd40156f7c4d3ee7c4d184efb4bb59584320b38`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 18:49:54 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:06:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:06:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:07:00 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:07:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198cf2d877b69a84769db31aa1a2b93d281750d73e202d5b75ffaa69a8455af`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967478fc83677ac2a896f0bf9d0031038706b09d7278a140c9524d2d01b7b381`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e317452c12763747fcf2c95765e29dff9ffb68ea7270e3a9ccdc7d9dba3ab`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baac56e8429e174b6ed91e6632336cd084f51c3b5b4ad02899c645c550e939`  
		Last Modified: Wed, 12 Aug 2020 21:08:37 GMT  
		Size: 455.9 MB (455869774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa8b3165120c50c00f0696a0e05b120cc611bdea09a292f30f9440d9cc23a5f`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a229abf6a7a32b7150ac1685ac5cdbc71054162e40ebb34ccaa566dfb5409`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82549182e3420298ada296c9c35f42c61a338795f0dfa940932ceb3bdcdbd4`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.19-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:9821d40c3bf7615e1194856a8ca506eca454270017ddbe3aa029a6a918c0ad9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2791158383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bcfc35477ed09662dc392aaa72a0f2a7145688541990ba39ae5b5ef0555bec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 19:07:11 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:24:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:24:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:24:46 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:24:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9762656745a831a530ed58667d50ac83fc00cf7944c20452cc16c4536078eb`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec1ef6b7bb662d96c44be88a67b782baa8875d690630da539c73de98c39c37`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65b8eef495cdc8c17f8c78eb5f2aa90f04a2399db9604fb497d96ac24761ee`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc50b0d90c9a5e216aa2a362af3bdf1ea6c7f7e6bf7c8a8056b8b12bf39a8`  
		Last Modified: Wed, 12 Aug 2020 21:10:11 GMT  
		Size: 455.3 MB (455283454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d19d7ef440474edbb6f191aa9deb685b5d583b997641e72f0e067eda776cc`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce619af052ee66b3900c4bf2191e209924541192afb0bcf0d935b74cc7dec4`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9851b297d4aaa13fac0de850eb984db23b7a92b5b9f51459926d22c21dc82f05`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.19-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a605b976fad03e78343568aad5565a1a040726647b3b8a6350b5cab1a9be5957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `mongo:3.6.19-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:9821d40c3bf7615e1194856a8ca506eca454270017ddbe3aa029a6a918c0ad9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2791158383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bcfc35477ed09662dc392aaa72a0f2a7145688541990ba39ae5b5ef0555bec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 19:07:11 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:24:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:24:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:24:46 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:24:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9762656745a831a530ed58667d50ac83fc00cf7944c20452cc16c4536078eb`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec1ef6b7bb662d96c44be88a67b782baa8875d690630da539c73de98c39c37`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65b8eef495cdc8c17f8c78eb5f2aa90f04a2399db9604fb497d96ac24761ee`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc50b0d90c9a5e216aa2a362af3bdf1ea6c7f7e6bf7c8a8056b8b12bf39a8`  
		Last Modified: Wed, 12 Aug 2020 21:10:11 GMT  
		Size: 455.3 MB (455283454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d19d7ef440474edbb6f191aa9deb685b5d583b997641e72f0e067eda776cc`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce619af052ee66b3900c4bf2191e209924541192afb0bcf0d935b74cc7dec4`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9851b297d4aaa13fac0de850eb984db23b7a92b5b9f51459926d22c21dc82f05`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.19-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:ae9c764e05e2a1952c3c8cfc016577cad8dbbc3fc5437491e6aa3a4c98bdf639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `mongo:3.6.19-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:80f49b88be25266fbaf54ecb8d56874b90ae26396165bfbf065179c75003fb99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6194025093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5311f8a28994a0a93e2d3cbfcbd40156f7c4d3ee7c4d184efb4bb59584320b38`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 18:49:54 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:06:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:06:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:07:00 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:07:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198cf2d877b69a84769db31aa1a2b93d281750d73e202d5b75ffaa69a8455af`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967478fc83677ac2a896f0bf9d0031038706b09d7278a140c9524d2d01b7b381`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e317452c12763747fcf2c95765e29dff9ffb68ea7270e3a9ccdc7d9dba3ab`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baac56e8429e174b6ed91e6632336cd084f51c3b5b4ad02899c645c550e939`  
		Last Modified: Wed, 12 Aug 2020 21:08:37 GMT  
		Size: 455.9 MB (455869774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa8b3165120c50c00f0696a0e05b120cc611bdea09a292f30f9440d9cc23a5f`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a229abf6a7a32b7150ac1685ac5cdbc71054162e40ebb34ccaa566dfb5409`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82549182e3420298ada296c9c35f42c61a338795f0dfa940932ceb3bdcdbd4`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6.19-xenial`

```console
$ docker pull mongo@sha256:e3c85e31f1b9ca6b213cf0dc48e00e6d9702adffe7b765e414c85799ab2606b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6.19-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:4eaf89ddb158d79817aa55f72c6bb9389f2aad5175cbf53710fd5394aee65d50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (166043159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a9a525de518f0e4a5243677811d5225aedf618c47deefda5bbb34dd49953ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:26:48 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 23:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:26:57 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:26:57 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 23:27:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:27:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:27:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 23:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:27:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:27:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 23:27:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:27:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:27:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:27:29 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:27:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:27:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:27:29 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:27:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d3f5ac1e7d68e1f6a8df1cc0a15e10257b638cb61a4703cf473ebcea4a3cdc`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ee44fa74647a5ac9e7235f860ca1837d7cbdf33ff6b8572273b6e437d82c8`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.9 MB (2904023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4a221d83b214928e24798076a8fd803a47b4b2c1636685fd20bf1b7695f92d`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 1.3 MB (1305145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66157b0856629ea0067df90c67b46de982f5fbd52a5aa6f6867acfb1142f873e`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1feeebf7c67bc3ce058e8211a04baff8dcf79e5c80d81aad5ae0edeb306bc7d`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b223d5499407dd90b8a47cf3cf7ae1727525951cc2db67d7a020e4408a6c08`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1b694ff7b774f225a9592b8c86d459e4bf4143a804c78e1b2819589d5f58c`  
		Last Modified: Wed, 19 Aug 2020 23:29:53 GMT  
		Size: 117.4 MB (117376469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451337765eaa999d705f9378340cfba3ae052480b8baa4f8e1c105e39cbcad83`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740a7d10ecb64180be64c489560fa2a6f8c468e4197d06749ab974d2a467127a`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6.19-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c0ae3888736d69a12caa6c43b40170b51425cfdf79fa3681f4540861576fce18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155338889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2909f7bf21269c9924ca0c2fa73fc710372552ed29206981463832ceab617d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:31:59 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:32:16 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:32:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:32:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:32:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 22:32:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:32:51 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:32:52 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 22:32:54 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 22:32:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:33:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:33:22 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:33:23 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:33:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:33:26 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:33:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e57371bd09af15391debc536f6839de7e6ebe7295d50c757dd90f1df6a30da`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b81baa9ce507ec53d3e562d07f480173afa304930494fbd5016ce1c973d8a7`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.4 MB (2432322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0017ea2c2557a608f31f58299936c07c02b7ace3893a5023ca8cad1251034d`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 1.2 MB (1232551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7d1adbe02e2dba2f95d6a9d5b4e8b7282501efd56540440feebb899992e8b1`  
		Last Modified: Wed, 19 Aug 2020 22:37:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec57e97f591b600e564b6e8987f319c18ba7a51c04e3fa1f57cb379b5925dd1`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29758a89cbd002946903ddf1bb164da5e54f6ee672fc1bbd9757aa6e6a9489db`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9aeebb1082432123096ff49b22c17906659291e2932c7ef81825d5f5f2bbc`  
		Last Modified: Wed, 19 Aug 2020 22:38:18 GMT  
		Size: 111.6 MB (111590125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb536ab7200c7b9051ccf226346ab245dcae3ff7680246249aefb822d3a1da84`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa474c7c76ae49118086d377ef5d0fe8a4671a0cf1db2f13a351d64dd17c747`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore`

```console
$ docker pull mongo@sha256:92283737b545079e7143ae61f3194a387f430aa11f1c8683af094cfe476bba58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:3.6-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:80f49b88be25266fbaf54ecb8d56874b90ae26396165bfbf065179c75003fb99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6194025093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5311f8a28994a0a93e2d3cbfcbd40156f7c4d3ee7c4d184efb4bb59584320b38`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 18:49:54 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:06:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:06:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:07:00 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:07:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198cf2d877b69a84769db31aa1a2b93d281750d73e202d5b75ffaa69a8455af`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967478fc83677ac2a896f0bf9d0031038706b09d7278a140c9524d2d01b7b381`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e317452c12763747fcf2c95765e29dff9ffb68ea7270e3a9ccdc7d9dba3ab`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baac56e8429e174b6ed91e6632336cd084f51c3b5b4ad02899c645c550e939`  
		Last Modified: Wed, 12 Aug 2020 21:08:37 GMT  
		Size: 455.9 MB (455869774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa8b3165120c50c00f0696a0e05b120cc611bdea09a292f30f9440d9cc23a5f`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a229abf6a7a32b7150ac1685ac5cdbc71054162e40ebb34ccaa566dfb5409`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82549182e3420298ada296c9c35f42c61a338795f0dfa940932ceb3bdcdbd4`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:9821d40c3bf7615e1194856a8ca506eca454270017ddbe3aa029a6a918c0ad9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2791158383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bcfc35477ed09662dc392aaa72a0f2a7145688541990ba39ae5b5ef0555bec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 19:07:11 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:24:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:24:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:24:46 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:24:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9762656745a831a530ed58667d50ac83fc00cf7944c20452cc16c4536078eb`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec1ef6b7bb662d96c44be88a67b782baa8875d690630da539c73de98c39c37`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65b8eef495cdc8c17f8c78eb5f2aa90f04a2399db9604fb497d96ac24761ee`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc50b0d90c9a5e216aa2a362af3bdf1ea6c7f7e6bf7c8a8056b8b12bf39a8`  
		Last Modified: Wed, 12 Aug 2020 21:10:11 GMT  
		Size: 455.3 MB (455283454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d19d7ef440474edbb6f191aa9deb685b5d583b997641e72f0e067eda776cc`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce619af052ee66b3900c4bf2191e209924541192afb0bcf0d935b74cc7dec4`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9851b297d4aaa13fac0de850eb984db23b7a92b5b9f51459926d22c21dc82f05`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a605b976fad03e78343568aad5565a1a040726647b3b8a6350b5cab1a9be5957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `mongo:3.6-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:9821d40c3bf7615e1194856a8ca506eca454270017ddbe3aa029a6a918c0ad9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2791158383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bcfc35477ed09662dc392aaa72a0f2a7145688541990ba39ae5b5ef0555bec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 19:07:11 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:24:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:24:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:24:46 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:24:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9762656745a831a530ed58667d50ac83fc00cf7944c20452cc16c4536078eb`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec1ef6b7bb662d96c44be88a67b782baa8875d690630da539c73de98c39c37`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65b8eef495cdc8c17f8c78eb5f2aa90f04a2399db9604fb497d96ac24761ee`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc50b0d90c9a5e216aa2a362af3bdf1ea6c7f7e6bf7c8a8056b8b12bf39a8`  
		Last Modified: Wed, 12 Aug 2020 21:10:11 GMT  
		Size: 455.3 MB (455283454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d19d7ef440474edbb6f191aa9deb685b5d583b997641e72f0e067eda776cc`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce619af052ee66b3900c4bf2191e209924541192afb0bcf0d935b74cc7dec4`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9851b297d4aaa13fac0de850eb984db23b7a92b5b9f51459926d22c21dc82f05`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:ae9c764e05e2a1952c3c8cfc016577cad8dbbc3fc5437491e6aa3a4c98bdf639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `mongo:3.6-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:80f49b88be25266fbaf54ecb8d56874b90ae26396165bfbf065179c75003fb99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6194025093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5311f8a28994a0a93e2d3cbfcbd40156f7c4d3ee7c4d184efb4bb59584320b38`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 18:49:54 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:06:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:06:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:07:00 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:07:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198cf2d877b69a84769db31aa1a2b93d281750d73e202d5b75ffaa69a8455af`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967478fc83677ac2a896f0bf9d0031038706b09d7278a140c9524d2d01b7b381`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e317452c12763747fcf2c95765e29dff9ffb68ea7270e3a9ccdc7d9dba3ab`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baac56e8429e174b6ed91e6632336cd084f51c3b5b4ad02899c645c550e939`  
		Last Modified: Wed, 12 Aug 2020 21:08:37 GMT  
		Size: 455.9 MB (455869774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa8b3165120c50c00f0696a0e05b120cc611bdea09a292f30f9440d9cc23a5f`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a229abf6a7a32b7150ac1685ac5cdbc71054162e40ebb34ccaa566dfb5409`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82549182e3420298ada296c9c35f42c61a338795f0dfa940932ceb3bdcdbd4`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3.6-xenial`

```console
$ docker pull mongo@sha256:e3c85e31f1b9ca6b213cf0dc48e00e6d9702adffe7b765e414c85799ab2606b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3.6-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:4eaf89ddb158d79817aa55f72c6bb9389f2aad5175cbf53710fd5394aee65d50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (166043159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a9a525de518f0e4a5243677811d5225aedf618c47deefda5bbb34dd49953ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:26:48 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 23:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:26:57 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:26:57 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 23:27:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:27:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:27:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 23:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:27:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:27:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 23:27:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:27:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:27:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:27:29 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:27:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:27:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:27:29 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:27:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d3f5ac1e7d68e1f6a8df1cc0a15e10257b638cb61a4703cf473ebcea4a3cdc`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ee44fa74647a5ac9e7235f860ca1837d7cbdf33ff6b8572273b6e437d82c8`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.9 MB (2904023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4a221d83b214928e24798076a8fd803a47b4b2c1636685fd20bf1b7695f92d`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 1.3 MB (1305145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66157b0856629ea0067df90c67b46de982f5fbd52a5aa6f6867acfb1142f873e`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1feeebf7c67bc3ce058e8211a04baff8dcf79e5c80d81aad5ae0edeb306bc7d`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b223d5499407dd90b8a47cf3cf7ae1727525951cc2db67d7a020e4408a6c08`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1b694ff7b774f225a9592b8c86d459e4bf4143a804c78e1b2819589d5f58c`  
		Last Modified: Wed, 19 Aug 2020 23:29:53 GMT  
		Size: 117.4 MB (117376469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451337765eaa999d705f9378340cfba3ae052480b8baa4f8e1c105e39cbcad83`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740a7d10ecb64180be64c489560fa2a6f8c468e4197d06749ab974d2a467127a`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3.6-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c0ae3888736d69a12caa6c43b40170b51425cfdf79fa3681f4540861576fce18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155338889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2909f7bf21269c9924ca0c2fa73fc710372552ed29206981463832ceab617d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:31:59 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:32:16 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:32:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:32:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:32:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 22:32:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:32:51 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:32:52 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 22:32:54 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 22:32:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:33:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:33:22 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:33:23 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:33:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:33:26 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:33:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e57371bd09af15391debc536f6839de7e6ebe7295d50c757dd90f1df6a30da`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b81baa9ce507ec53d3e562d07f480173afa304930494fbd5016ce1c973d8a7`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.4 MB (2432322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0017ea2c2557a608f31f58299936c07c02b7ace3893a5023ca8cad1251034d`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 1.2 MB (1232551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7d1adbe02e2dba2f95d6a9d5b4e8b7282501efd56540440feebb899992e8b1`  
		Last Modified: Wed, 19 Aug 2020 22:37:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec57e97f591b600e564b6e8987f319c18ba7a51c04e3fa1f57cb379b5925dd1`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29758a89cbd002946903ddf1bb164da5e54f6ee672fc1bbd9757aa6e6a9489db`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9aeebb1082432123096ff49b22c17906659291e2932c7ef81825d5f5f2bbc`  
		Last Modified: Wed, 19 Aug 2020 22:38:18 GMT  
		Size: 111.6 MB (111590125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb536ab7200c7b9051ccf226346ab245dcae3ff7680246249aefb822d3a1da84`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa474c7c76ae49118086d377ef5d0fe8a4671a0cf1db2f13a351d64dd17c747`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore`

```console
$ docker pull mongo@sha256:92283737b545079e7143ae61f3194a387f430aa11f1c8683af094cfe476bba58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:3-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:80f49b88be25266fbaf54ecb8d56874b90ae26396165bfbf065179c75003fb99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6194025093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5311f8a28994a0a93e2d3cbfcbd40156f7c4d3ee7c4d184efb4bb59584320b38`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 18:49:54 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:06:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:06:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:07:00 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:07:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198cf2d877b69a84769db31aa1a2b93d281750d73e202d5b75ffaa69a8455af`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967478fc83677ac2a896f0bf9d0031038706b09d7278a140c9524d2d01b7b381`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e317452c12763747fcf2c95765e29dff9ffb68ea7270e3a9ccdc7d9dba3ab`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baac56e8429e174b6ed91e6632336cd084f51c3b5b4ad02899c645c550e939`  
		Last Modified: Wed, 12 Aug 2020 21:08:37 GMT  
		Size: 455.9 MB (455869774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa8b3165120c50c00f0696a0e05b120cc611bdea09a292f30f9440d9cc23a5f`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a229abf6a7a32b7150ac1685ac5cdbc71054162e40ebb34ccaa566dfb5409`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82549182e3420298ada296c9c35f42c61a338795f0dfa940932ceb3bdcdbd4`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:9821d40c3bf7615e1194856a8ca506eca454270017ddbe3aa029a6a918c0ad9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2791158383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bcfc35477ed09662dc392aaa72a0f2a7145688541990ba39ae5b5ef0555bec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 19:07:11 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:24:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:24:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:24:46 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:24:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9762656745a831a530ed58667d50ac83fc00cf7944c20452cc16c4536078eb`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec1ef6b7bb662d96c44be88a67b782baa8875d690630da539c73de98c39c37`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65b8eef495cdc8c17f8c78eb5f2aa90f04a2399db9604fb497d96ac24761ee`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc50b0d90c9a5e216aa2a362af3bdf1ea6c7f7e6bf7c8a8056b8b12bf39a8`  
		Last Modified: Wed, 12 Aug 2020 21:10:11 GMT  
		Size: 455.3 MB (455283454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d19d7ef440474edbb6f191aa9deb685b5d583b997641e72f0e067eda776cc`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce619af052ee66b3900c4bf2191e209924541192afb0bcf0d935b74cc7dec4`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9851b297d4aaa13fac0de850eb984db23b7a92b5b9f51459926d22c21dc82f05`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a605b976fad03e78343568aad5565a1a040726647b3b8a6350b5cab1a9be5957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `mongo:3-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:9821d40c3bf7615e1194856a8ca506eca454270017ddbe3aa029a6a918c0ad9a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2791158383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bcfc35477ed09662dc392aaa72a0f2a7145688541990ba39ae5b5ef0555bec`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 19:07:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 19:07:11 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:24:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:24:45 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:24:46 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:24:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9762656745a831a530ed58667d50ac83fc00cf7944c20452cc16c4536078eb`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec1ef6b7bb662d96c44be88a67b782baa8875d690630da539c73de98c39c37`  
		Last Modified: Wed, 12 Aug 2020 21:08:54 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a65b8eef495cdc8c17f8c78eb5f2aa90f04a2399db9604fb497d96ac24761ee`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc50b0d90c9a5e216aa2a362af3bdf1ea6c7f7e6bf7c8a8056b8b12bf39a8`  
		Last Modified: Wed, 12 Aug 2020 21:10:11 GMT  
		Size: 455.3 MB (455283454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756d19d7ef440474edbb6f191aa9deb685b5d583b997641e72f0e067eda776cc`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce619af052ee66b3900c4bf2191e209924541192afb0bcf0d935b74cc7dec4`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9851b297d4aaa13fac0de850eb984db23b7a92b5b9f51459926d22c21dc82f05`  
		Last Modified: Wed, 12 Aug 2020 21:08:51 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:ae9c764e05e2a1952c3c8cfc016577cad8dbbc3fc5437491e6aa3a4c98bdf639
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `mongo:3-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:80f49b88be25266fbaf54ecb8d56874b90ae26396165bfbf065179c75003fb99
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6194025093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5311f8a28994a0a93e2d3cbfcbd40156f7c4d3ee7c4d184efb4bb59584320b38`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 12 Aug 2020 18:49:53 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-3.6.19-signed.msi
# Wed, 12 Aug 2020 18:49:54 GMT
ENV MONGO_DOWNLOAD_SHA256=4375a8fa0d87dd0b16ab40a20487ddb5870d6f056d42ef654debf3e7fab6ae40
# Wed, 12 Aug 2020 19:06:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:06:59 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:07:00 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:07:01 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198cf2d877b69a84769db31aa1a2b93d281750d73e202d5b75ffaa69a8455af`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967478fc83677ac2a896f0bf9d0031038706b09d7278a140c9524d2d01b7b381`  
		Last Modified: Wed, 12 Aug 2020 21:07:25 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e317452c12763747fcf2c95765e29dff9ffb68ea7270e3a9ccdc7d9dba3ab`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9baac56e8429e174b6ed91e6632336cd084f51c3b5b4ad02899c645c550e939`  
		Last Modified: Wed, 12 Aug 2020 21:08:37 GMT  
		Size: 455.9 MB (455869774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa8b3165120c50c00f0696a0e05b120cc611bdea09a292f30f9440d9cc23a5f`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3a229abf6a7a32b7150ac1685ac5cdbc71054162e40ebb34ccaa566dfb5409`  
		Last Modified: Wed, 12 Aug 2020 21:07:22 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce82549182e3420298ada296c9c35f42c61a338795f0dfa940932ceb3bdcdbd4`  
		Last Modified: Wed, 12 Aug 2020 21:07:23 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:3-xenial`

```console
$ docker pull mongo@sha256:e3c85e31f1b9ca6b213cf0dc48e00e6d9702adffe7b765e414c85799ab2606b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:3-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:4eaf89ddb158d79817aa55f72c6bb9389f2aad5175cbf53710fd5394aee65d50
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (166043159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a9a525de518f0e4a5243677811d5225aedf618c47deefda5bbb34dd49953ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:26:48 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 23:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:26:57 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:26:57 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 23:27:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:27:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:27:09 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 23:27:10 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:27:10 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:27:11 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 23:27:11 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 23:27:12 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:27:28 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:27:29 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:27:29 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:27:29 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:27:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:27:29 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:27:30 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d3f5ac1e7d68e1f6a8df1cc0a15e10257b638cb61a4703cf473ebcea4a3cdc`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ee44fa74647a5ac9e7235f860ca1837d7cbdf33ff6b8572273b6e437d82c8`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.9 MB (2904023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4a221d83b214928e24798076a8fd803a47b4b2c1636685fd20bf1b7695f92d`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 1.3 MB (1305145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66157b0856629ea0067df90c67b46de982f5fbd52a5aa6f6867acfb1142f873e`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1feeebf7c67bc3ce058e8211a04baff8dcf79e5c80d81aad5ae0edeb306bc7d`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 2.0 KB (1996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b223d5499407dd90b8a47cf3cf7ae1727525951cc2db67d7a020e4408a6c08`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c1b694ff7b774f225a9592b8c86d459e4bf4143a804c78e1b2819589d5f58c`  
		Last Modified: Wed, 19 Aug 2020 23:29:53 GMT  
		Size: 117.4 MB (117376469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451337765eaa999d705f9378340cfba3ae052480b8baa4f8e1c105e39cbcad83`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740a7d10ecb64180be64c489560fa2a6f8c468e4197d06749ab974d2a467127a`  
		Last Modified: Wed, 19 Aug 2020 23:29:34 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:3-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:c0ae3888736d69a12caa6c43b40170b51425cfdf79fa3681f4540861576fce18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155338889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2909f7bf21269c9924ca0c2fa73fc710372552ed29206981463832ceab617d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:31:59 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:32:16 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:32:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:32:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:32:47 GMT
ENV GPG_KEYS=2930ADAE8CAF5059EE73BB4B58712A2291FA4AD5
# Wed, 19 Aug 2020 22:32:50 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:32:51 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:32:52 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:32:53 GMT
ENV MONGO_MAJOR=3.6
# Wed, 19 Aug 2020 22:32:54 GMT
ENV MONGO_VERSION=3.6.19
# Wed, 19 Aug 2020 22:32:55 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:33:18 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:33:22 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:33:23 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:33:24 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:33:26 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:33:26 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e57371bd09af15391debc536f6839de7e6ebe7295d50c757dd90f1df6a30da`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b81baa9ce507ec53d3e562d07f480173afa304930494fbd5016ce1c973d8a7`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.4 MB (2432322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0017ea2c2557a608f31f58299936c07c02b7ace3893a5023ca8cad1251034d`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 1.2 MB (1232551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7d1adbe02e2dba2f95d6a9d5b4e8b7282501efd56540440feebb899992e8b1`  
		Last Modified: Wed, 19 Aug 2020 22:37:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec57e97f591b600e564b6e8987f319c18ba7a51c04e3fa1f57cb379b5925dd1`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 2.0 KB (2005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29758a89cbd002946903ddf1bb164da5e54f6ee672fc1bbd9757aa6e6a9489db`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9aeebb1082432123096ff49b22c17906659291e2932c7ef81825d5f5f2bbc`  
		Last Modified: Wed, 19 Aug 2020 22:38:18 GMT  
		Size: 111.6 MB (111590125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb536ab7200c7b9051ccf226346ab245dcae3ff7680246249aefb822d3a1da84`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa474c7c76ae49118086d377ef5d0fe8a4671a0cf1db2f13a351d64dd17c747`  
		Last Modified: Wed, 19 Aug 2020 22:37:39 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4`

```console
$ docker pull mongo@sha256:df9eca84736a666d5f7e7a09aeb8a6d8d073698d5b7349400f10ee75812e0e95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4` - linux; amd64

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

### `mongo:4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cd9b4445508d088608aff8d49a6de9bfc1d3eea3b0b223827ecaa27fcc51f9f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167923219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2b6b0873dbe42c8f7859603bdf939f17da04f4b468f9f25af6c6169aa6ca1f`
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
# Wed, 19 Aug 2020 22:36:36 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:36:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:37:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:37:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:37:13 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:37:14 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:37:16 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:37:17 GMT
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
	-	`sha256:faf61d67c581443a883e2b613e3832d2b2c991daa9b1c47410ccff5499e08fc6`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e437891cf74a6a9aba16ead456655e997c04f2fce5794ee214e388178d5fa1c`  
		Last Modified: Wed, 19 Aug 2020 22:40:10 GMT  
		Size: 136.1 MB (136145203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6914935be6ab626955ca4669ee6c7e69d6919abbbf5596db6e87967d01f8fd5f`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cba816b02f9834a93a91560660b43bfcddf84ecf7220ed71e3c2e69f02ab`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - linux; s390x

```console
$ docker pull mongo@sha256:f143bbac6c00e2157a08274e3fb3bf81641e8ac6341a67fff503ed8e5cbebd2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172900638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5495d92d4faf769b9cf64e94c235bbd595e7d6a701ce9cf6ecf4be08a7f5aa`
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
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:13:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:13:43 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:14:00 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:14:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:14:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:14:01 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:14:01 GMT
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
	-	`sha256:2e6595175e6368e1261954ecbe6d1b5d361c7389fca7bc5f0a2061773f01ea6c`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2840e6d43940c9bb7c109a8fcd575df74022ebc13d8a34f1d23b8ec4dd1d6517`  
		Last Modified: Wed, 19 Aug 2020 22:14:57 GMT  
		Size: 139.0 MB (139034494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac410b9916e625ac10d52cc3780a917dc6afd2de331872d5b1de148ebf852971`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241abb48b4fe9fa1d0d6c73748732e0afd16262dcb18add879e2a8a47ecb9b2d`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0`

```console
$ docker pull mongo@sha256:cb9c1b49d6947e99df80817fb9b99c5fa4ce91d083498f1d76f5b8e73a33ec8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.0` - linux; amd64

```console
$ docker pull mongo@sha256:3a377c8e6e0e85ba636b4cb335038e83e173635e61b8c4af6621d29e734453a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.9 MB (153920770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f4b16ab93087a20501a5c42ecacf18fe4f230441d32f6fc548e6c252f7fd11d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:26:48 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 23:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:26:57 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:26:57 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 23:27:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:27:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:27:35 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 19 Aug 2020 23:27:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:27:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:27:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:36 GMT
ENV MONGO_MAJOR=4.0
# Wed, 19 Aug 2020 23:27:36 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 19 Aug 2020 23:27:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:27:54 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:27:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:27:55 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:27:55 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:27:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:27:56 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:27:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d3f5ac1e7d68e1f6a8df1cc0a15e10257b638cb61a4703cf473ebcea4a3cdc`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ee44fa74647a5ac9e7235f860ca1837d7cbdf33ff6b8572273b6e437d82c8`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.9 MB (2904023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4a221d83b214928e24798076a8fd803a47b4b2c1636685fd20bf1b7695f92d`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 1.3 MB (1305145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66157b0856629ea0067df90c67b46de982f5fbd52a5aa6f6867acfb1142f873e`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b58faf95c9ad467302755fbcf2f41234e179fa18e5e9b228f71cd9af5b58b4`  
		Last Modified: Wed, 19 Aug 2020 23:29:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c71c458f9cb9569d509e566ae2e73f6f0cd50dbfe4e80d0789e4823c237dc`  
		Last Modified: Wed, 19 Aug 2020 23:29:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ffead3c6693cd3134b40189176c45bd1f38b6626c81b9eaf6f40fa973b10ac`  
		Last Modified: Wed, 19 Aug 2020 23:30:14 GMT  
		Size: 105.3 MB (105254655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0290953ef0e9e9968608958d0968f044a3105eceb37e4990ee531a5a2d387f92`  
		Last Modified: Wed, 19 Aug 2020 23:29:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa32a0985c0a0a73ba9b475b9d32dac49ed1d171a8bc8fc2259446b27d796980`  
		Last Modified: Wed, 19 Aug 2020 23:29:58 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:65fb7fbf844ab0e0424043c6bd2556c1eb7154646c4a2d2f3f25b444aa3a0fff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143434576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3824928afe09867f38c42ecf373342fa04a0b820d94d0442df6995fcfbe548f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:31:59 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:32:16 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:32:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:32:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:33:41 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 19 Aug 2020 22:33:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:33:45 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:33:45 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:33:46 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:33:47 GMT
ENV MONGO_MAJOR=4.0
# Wed, 19 Aug 2020 22:33:48 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 19 Aug 2020 22:33:50 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:34:17 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:34:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:34:22 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:34:23 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:34:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:34:26 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:34:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e57371bd09af15391debc536f6839de7e6ebe7295d50c757dd90f1df6a30da`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b81baa9ce507ec53d3e562d07f480173afa304930494fbd5016ce1c973d8a7`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.4 MB (2432322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0017ea2c2557a608f31f58299936c07c02b7ace3893a5023ca8cad1251034d`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 1.2 MB (1232551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7d1adbe02e2dba2f95d6a9d5b4e8b7282501efd56540440feebb899992e8b1`  
		Last Modified: Wed, 19 Aug 2020 22:37:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432dea58803529d68d3aa9faf68e7229e7a872ddc8941b9ae1e5107017a08cbc`  
		Last Modified: Wed, 19 Aug 2020 22:38:26 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cba9ab71e53438022156a3626572839c99ad8ff6f17b5213997fc388df6a4`  
		Last Modified: Wed, 19 Aug 2020 22:38:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097481bee9a902a83e966eca76f81ecb11d0c49e1859fe0d87e58c0478e4aa2d`  
		Last Modified: Wed, 19 Aug 2020 22:38:51 GMT  
		Size: 99.7 MB (99686391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d292fb9509481500785703763464495c7038821b7a16422062e470107a53d362`  
		Last Modified: Wed, 19 Aug 2020 22:38:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4b4be8e9eab439b27dbfe7675a863f423542f4f2db7b3dd896b239e0889f1`  
		Last Modified: Wed, 19 Aug 2020 22:38:26 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8cc39d2d4c9ecf3ebba69efa9de748ef1223dc655a8159904da77ddd17439eb5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187174132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbc322cf72cc3be765d11eee8b7f4177445258799b4b2c409084d3e0b8eb2c24`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:24:59 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 12 Aug 2020 19:24:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 12 Aug 2020 19:25:00 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 12 Aug 2020 19:42:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:42:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:42:54 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:42:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aba5d3ab869c436059665befb0e63d8415de6f027d529165832c88ad898cb0a`  
		Last Modified: Wed, 12 Aug 2020 21:10:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba609e0c5850eba0d0a0349bbf8ea5b45f6cc87bc68080259b92ea766480af61`  
		Last Modified: Wed, 12 Aug 2020 21:10:28 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed92018c4366eb2f25cac372642ffe11f70cb297d33d49d6107a294cae5d54`  
		Last Modified: Wed, 12 Aug 2020 21:10:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cea409daa6e5e1bd0d72df82a5ccdff4e3dc4d6299a1921abed7ebbb93e1a1`  
		Last Modified: Wed, 12 Aug 2020 21:12:15 GMT  
		Size: 449.0 MB (449018718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceff6a77051e73dfaf087e9ce1a813e1610b37a3d7e23661210c140193f9e51d`  
		Last Modified: Wed, 12 Aug 2020 21:10:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce1c5b301541417258e414f272aaa5847fbee985a7a05505915ab402e2286b5`  
		Last Modified: Wed, 12 Aug 2020 21:10:25 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0de86af974b9636b12600fb7f17dde3e6f589e1f20d81a54f4dfa39d25c2cdb`  
		Last Modified: Wed, 12 Aug 2020 21:10:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:333df409640b8ec87caff04ce9586c426e16c815f34bbf7fe0512a54ecdf4fc3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784118330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0f961538ed6828173cc0be21e4e4e287ac26e0701d6045ea1d79275a698e89`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:43:01 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 12 Aug 2020 19:43:02 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 12 Aug 2020 19:43:02 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 12 Aug 2020 20:01:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:01:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:01:45 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:01:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4b9de491bd7680bcac3094035f32b0c8dbb10d9665bd07a42dd095c0ce047d`  
		Last Modified: Wed, 12 Aug 2020 21:12:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f47d5b74bdec9cfb34657a15e5e8a85d58c1b68a6a58ccf902f1d0a5d702489`  
		Last Modified: Wed, 12 Aug 2020 21:12:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87089ed8623e8d95b7c6b36a612a3d00526482e7ce98d2fc76c09d4d1d2cdd02`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92336dd6cebb1c2e7d42a33dfb963580ae43b1baca9411fb73d00ad1cb056bda`  
		Last Modified: Wed, 12 Aug 2020 21:13:43 GMT  
		Size: 448.2 MB (448243383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0331a1b61361e816d9e8af31729102f779ac75f893666282cd55c7d5e8851fe4`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd82af7273a6536bb67edb0aecafeeaaad349f73520d02e6671e53baf2bf06e`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ff6d1dfd9f309c8154ea34ef0ebc123e1661de5659a909ff4ca0f5b2305255`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0.20`

**does not exist** (yet?)

## `mongo:4.0.20-windowsservercore`

**does not exist** (yet?)

## `mongo:4.0.20-windowsservercore-1809`

**does not exist** (yet?)

## `mongo:4.0.20-windowsservercore-ltsc2016`

**does not exist** (yet?)

## `mongo:4.0.20-xenial`

**does not exist** (yet?)

## `mongo:4.0-windowsservercore`

```console
$ docker pull mongo@sha256:d88b4905f039c4638a727e4fb2d479e72ebbfa51fda487f4f9aac51ba8535fa9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.0-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8cc39d2d4c9ecf3ebba69efa9de748ef1223dc655a8159904da77ddd17439eb5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187174132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbc322cf72cc3be765d11eee8b7f4177445258799b4b2c409084d3e0b8eb2c24`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:24:59 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 12 Aug 2020 19:24:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 12 Aug 2020 19:25:00 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 12 Aug 2020 19:42:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:42:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:42:54 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:42:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aba5d3ab869c436059665befb0e63d8415de6f027d529165832c88ad898cb0a`  
		Last Modified: Wed, 12 Aug 2020 21:10:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba609e0c5850eba0d0a0349bbf8ea5b45f6cc87bc68080259b92ea766480af61`  
		Last Modified: Wed, 12 Aug 2020 21:10:28 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed92018c4366eb2f25cac372642ffe11f70cb297d33d49d6107a294cae5d54`  
		Last Modified: Wed, 12 Aug 2020 21:10:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cea409daa6e5e1bd0d72df82a5ccdff4e3dc4d6299a1921abed7ebbb93e1a1`  
		Last Modified: Wed, 12 Aug 2020 21:12:15 GMT  
		Size: 449.0 MB (449018718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceff6a77051e73dfaf087e9ce1a813e1610b37a3d7e23661210c140193f9e51d`  
		Last Modified: Wed, 12 Aug 2020 21:10:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce1c5b301541417258e414f272aaa5847fbee985a7a05505915ab402e2286b5`  
		Last Modified: Wed, 12 Aug 2020 21:10:25 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0de86af974b9636b12600fb7f17dde3e6f589e1f20d81a54f4dfa39d25c2cdb`  
		Last Modified: Wed, 12 Aug 2020 21:10:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:333df409640b8ec87caff04ce9586c426e16c815f34bbf7fe0512a54ecdf4fc3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784118330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0f961538ed6828173cc0be21e4e4e287ac26e0701d6045ea1d79275a698e89`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:43:01 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 12 Aug 2020 19:43:02 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 12 Aug 2020 19:43:02 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 12 Aug 2020 20:01:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:01:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:01:45 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:01:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4b9de491bd7680bcac3094035f32b0c8dbb10d9665bd07a42dd095c0ce047d`  
		Last Modified: Wed, 12 Aug 2020 21:12:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f47d5b74bdec9cfb34657a15e5e8a85d58c1b68a6a58ccf902f1d0a5d702489`  
		Last Modified: Wed, 12 Aug 2020 21:12:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87089ed8623e8d95b7c6b36a612a3d00526482e7ce98d2fc76c09d4d1d2cdd02`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92336dd6cebb1c2e7d42a33dfb963580ae43b1baca9411fb73d00ad1cb056bda`  
		Last Modified: Wed, 12 Aug 2020 21:13:43 GMT  
		Size: 448.2 MB (448243383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0331a1b61361e816d9e8af31729102f779ac75f893666282cd55c7d5e8851fe4`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd82af7273a6536bb67edb0aecafeeaaad349f73520d02e6671e53baf2bf06e`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ff6d1dfd9f309c8154ea34ef0ebc123e1661de5659a909ff4ca0f5b2305255`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:a6fc8cbb427109a6e5a0af536953b5349be093a15a7a72a84b4e4d9836af797c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.0-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:333df409640b8ec87caff04ce9586c426e16c815f34bbf7fe0512a54ecdf4fc3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2784118330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0f961538ed6828173cc0be21e4e4e287ac26e0701d6045ea1d79275a698e89`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:43:01 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 12 Aug 2020 19:43:02 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 12 Aug 2020 19:43:02 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 12 Aug 2020 20:01:42 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:01:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:01:45 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:01:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4b9de491bd7680bcac3094035f32b0c8dbb10d9665bd07a42dd095c0ce047d`  
		Last Modified: Wed, 12 Aug 2020 21:12:30 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f47d5b74bdec9cfb34657a15e5e8a85d58c1b68a6a58ccf902f1d0a5d702489`  
		Last Modified: Wed, 12 Aug 2020 21:12:30 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87089ed8623e8d95b7c6b36a612a3d00526482e7ce98d2fc76c09d4d1d2cdd02`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92336dd6cebb1c2e7d42a33dfb963580ae43b1baca9411fb73d00ad1cb056bda`  
		Last Modified: Wed, 12 Aug 2020 21:13:43 GMT  
		Size: 448.2 MB (448243383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0331a1b61361e816d9e8af31729102f779ac75f893666282cd55c7d5e8851fe4`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd82af7273a6536bb67edb0aecafeeaaad349f73520d02e6671e53baf2bf06e`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ff6d1dfd9f309c8154ea34ef0ebc123e1661de5659a909ff4ca0f5b2305255`  
		Last Modified: Wed, 12 Aug 2020 21:12:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:b1c8ff40ae9a85ac962fa30013ccd085abecd3e44778cd9575e8552785ad9035
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `mongo:4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8cc39d2d4c9ecf3ebba69efa9de748ef1223dc655a8159904da77ddd17439eb5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6187174132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbc322cf72cc3be765d11eee8b7f4177445258799b4b2c409084d3e0b8eb2c24`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 19:24:59 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 12 Aug 2020 19:24:59 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2008plus-ssl-4.0.19-signed.msi
# Wed, 12 Aug 2020 19:25:00 GMT
ENV MONGO_DOWNLOAD_SHA256=fcdadb2d83e21551da2e8302f6cdab69ac840d4b1cca2cb353853c5d81aebac6
# Wed, 12 Aug 2020 19:42:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 19:42:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 19:42:54 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 19:42:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aba5d3ab869c436059665befb0e63d8415de6f027d529165832c88ad898cb0a`  
		Last Modified: Wed, 12 Aug 2020 21:10:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba609e0c5850eba0d0a0349bbf8ea5b45f6cc87bc68080259b92ea766480af61`  
		Last Modified: Wed, 12 Aug 2020 21:10:28 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed92018c4366eb2f25cac372642ffe11f70cb297d33d49d6107a294cae5d54`  
		Last Modified: Wed, 12 Aug 2020 21:10:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cea409daa6e5e1bd0d72df82a5ccdff4e3dc4d6299a1921abed7ebbb93e1a1`  
		Last Modified: Wed, 12 Aug 2020 21:12:15 GMT  
		Size: 449.0 MB (449018718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceff6a77051e73dfaf087e9ce1a813e1610b37a3d7e23661210c140193f9e51d`  
		Last Modified: Wed, 12 Aug 2020 21:10:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce1c5b301541417258e414f272aaa5847fbee985a7a05505915ab402e2286b5`  
		Last Modified: Wed, 12 Aug 2020 21:10:25 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0de86af974b9636b12600fb7f17dde3e6f589e1f20d81a54f4dfa39d25c2cdb`  
		Last Modified: Wed, 12 Aug 2020 21:10:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.0-xenial`

```console
$ docker pull mongo@sha256:425d81898e5a9d629d2ac783ecaed1940aa454607ae83fcefec95cfa70bbf2b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo:4.0-xenial` - linux; amd64

```console
$ docker pull mongo@sha256:3a377c8e6e0e85ba636b4cb335038e83e173635e61b8c4af6621d29e734453a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.9 MB (153920770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f4b16ab93087a20501a5c42ecacf18fe4f230441d32f6fc548e6c252f7fd11d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:26:48 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 23:26:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 23:26:57 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 23:26:57 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 23:27:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 23:27:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 23:27:35 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 19 Aug 2020 23:27:35 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:27:36 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:27:36 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:36 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:27:36 GMT
ENV MONGO_MAJOR=4.0
# Wed, 19 Aug 2020 23:27:36 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 19 Aug 2020 23:27:37 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:27:54 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:27:55 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:27:55 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:27:55 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:27:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:27:56 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:27:56 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d3f5ac1e7d68e1f6a8df1cc0a15e10257b638cb61a4703cf473ebcea4a3cdc`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.0 KB (1987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0ee44fa74647a5ac9e7235f860ca1837d7cbdf33ff6b8572273b6e437d82c8`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 2.9 MB (2904023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4a221d83b214928e24798076a8fd803a47b4b2c1636685fd20bf1b7695f92d`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 1.3 MB (1305145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66157b0856629ea0067df90c67b46de982f5fbd52a5aa6f6867acfb1142f873e`  
		Last Modified: Wed, 19 Aug 2020 23:29:35 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b58faf95c9ad467302755fbcf2f41234e179fa18e5e9b228f71cd9af5b58b4`  
		Last Modified: Wed, 19 Aug 2020 23:29:57 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c71c458f9cb9569d509e566ae2e73f6f0cd50dbfe4e80d0789e4823c237dc`  
		Last Modified: Wed, 19 Aug 2020 23:29:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ffead3c6693cd3134b40189176c45bd1f38b6626c81b9eaf6f40fa973b10ac`  
		Last Modified: Wed, 19 Aug 2020 23:30:14 GMT  
		Size: 105.3 MB (105254655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0290953ef0e9e9968608958d0968f044a3105eceb37e4990ee531a5a2d387f92`  
		Last Modified: Wed, 19 Aug 2020 23:29:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa32a0985c0a0a73ba9b475b9d32dac49ed1d171a8bc8fc2259446b27d796980`  
		Last Modified: Wed, 19 Aug 2020 23:29:58 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.0-xenial` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:65fb7fbf844ab0e0424043c6bd2556c1eb7154646c4a2d2f3f25b444aa3a0fff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143434576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3824928afe09867f38c42ecf373342fa04a0b820d94d0442df6995fcfbe548f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["mongod"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:31:59 GMT
RUN groupadd -r mongodb && useradd -r -g mongodb mongodb
# Wed, 19 Aug 2020 22:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		jq 		numactl 	; 	if ! command -v ps > /dev/null; then 		apt-get install -y --no-install-recommends procps; 	fi; 	rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 22:32:15 GMT
ENV GOSU_VERSION=1.12
# Wed, 19 Aug 2020 22:32:16 GMT
ENV JSYAML_VERSION=3.13.1
# Wed, 19 Aug 2020 22:32:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		wget 	; 	if ! command -v gpg > /dev/null; then 		apt-get install -y --no-install-recommends gnupg dirmngr; 		savedAptMark="$savedAptMark gnupg dirmngr"; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 		wget -O /js-yaml.js "https://github.com/nodeca/js-yaml/raw/${JSYAML_VERSION}/dist/js-yaml.js"; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 19 Aug 2020 22:32:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 19 Aug 2020 22:33:41 GMT
ENV GPG_KEYS=9DA31620334BD75D9DCB49F368818C72E52529D4
# Wed, 19 Aug 2020 22:33:44 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:33:45 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:33:45 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:33:46 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:33:47 GMT
ENV MONGO_MAJOR=4.0
# Wed, 19 Aug 2020 22:33:48 GMT
ENV MONGO_VERSION=4.0.19
# Wed, 19 Aug 2020 22:33:50 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu xenial/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:34:17 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:34:21 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:34:22 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:34:23 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:34:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:34:26 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:34:27 GMT
CMD ["mongod"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e57371bd09af15391debc536f6839de7e6ebe7295d50c757dd90f1df6a30da`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.0 KB (1994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b81baa9ce507ec53d3e562d07f480173afa304930494fbd5016ce1c973d8a7`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 2.4 MB (2432322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0017ea2c2557a608f31f58299936c07c02b7ace3893a5023ca8cad1251034d`  
		Last Modified: Wed, 19 Aug 2020 22:37:42 GMT  
		Size: 1.2 MB (1232551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7d1adbe02e2dba2f95d6a9d5b4e8b7282501efd56540440feebb899992e8b1`  
		Last Modified: Wed, 19 Aug 2020 22:37:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432dea58803529d68d3aa9faf68e7229e7a872ddc8941b9ae1e5107017a08cbc`  
		Last Modified: Wed, 19 Aug 2020 22:38:26 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19cba9ab71e53438022156a3626572839c99ad8ff6f17b5213997fc388df6a4`  
		Last Modified: Wed, 19 Aug 2020 22:38:26 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097481bee9a902a83e966eca76f81ecb11d0c49e1859fe0d87e58c0478e4aa2d`  
		Last Modified: Wed, 19 Aug 2020 22:38:51 GMT  
		Size: 99.7 MB (99686391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d292fb9509481500785703763464495c7038821b7a16422062e470107a53d362`  
		Last Modified: Wed, 19 Aug 2020 22:38:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4b4be8e9eab439b27dbfe7675a863f423542f4f2db7b3dd896b239e0889f1`  
		Last Modified: Wed, 19 Aug 2020 22:38:26 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2`

```console
$ docker pull mongo@sha256:bb3616e2f78a37bb607f59e451922d63d27e81d272514fb1cbffc7d1eab00eaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.2` - linux; amd64

```console
$ docker pull mongo@sha256:a658234b5e704b9694ddf1d0343baff2999ddeb1401d4bdd16f29798ac8fbd12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164665557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9775815948bc46df5e2a2a6a7676a322b03fd4378d95df888cb498565685c10`
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
# Wed, 19 Aug 2020 23:28:21 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 19 Aug 2020 23:28:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:28:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:28:23 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:28:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:28:23 GMT
ENV MONGO_MAJOR=4.2
# Wed, 19 Aug 2020 23:28:23 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 19 Aug 2020 23:28:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:28:42 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:28:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:28:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:28:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:28:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:28:44 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:28:44 GMT
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
	-	`sha256:a614d629c2848a030f38b31b71a781c61f88d97a18cf381187f286cdb0527ba1`  
		Last Modified: Wed, 19 Aug 2020 23:30:18 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477320af2dcc05dc13295366b1ec14e08bf8d39c58861691b12586cebd70ebdd`  
		Last Modified: Wed, 19 Aug 2020 23:30:18 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aab702fcf56b224102ecf54a4d0af0a1b42b81df1fddee78b15c08cf54c2ad`  
		Last Modified: Wed, 19 Aug 2020 23:30:36 GMT  
		Size: 129.1 MB (129122344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94c6a2dc294267bbab1718f5e4948528dda38dc8312e00f513764125789810a`  
		Last Modified: Wed, 19 Aug 2020 23:30:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf889bdb7c65ff5ae1e72f60f8a22ae4cb324b4756c3321dfc270650efe7ad7`  
		Last Modified: Wed, 19 Aug 2020 23:30:18 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8ae70bed1137fd41febc74bc981f907b38e0264505165474d3adc75f50d53549
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154678350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e194770a8c8f0ac94c5355d49778d13fda23873aaf571ee712fbe9e14af3a58d`
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
# Wed, 19 Aug 2020 22:35:23 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 19 Aug 2020 22:35:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:35:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:35:27 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:35:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:35:30 GMT
ENV MONGO_MAJOR=4.2
# Wed, 19 Aug 2020 22:35:31 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 19 Aug 2020 22:35:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:36:02 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:36:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:36:06 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:36:07 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:36:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:36:09 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:36:11 GMT
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
	-	`sha256:1e3d9c6e96a39031cb9c1dc26cda911d8e36de718489edcb4257c2cbd5735e11`  
		Last Modified: Wed, 19 Aug 2020 22:39:03 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66651b0c33490b229f317298c74d09923988c8f392133e9aec200c2ed2349db4`  
		Last Modified: Wed, 19 Aug 2020 22:39:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053ed69102564ccae4e255643d87f86b3dec330e99f02a280d41566b9fe070fe`  
		Last Modified: Wed, 19 Aug 2020 22:39:31 GMT  
		Size: 122.9 MB (122900327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9bdc108220d80f0f46736b9035de7cb84d596d1ae7a722f46c698e1c2502b2`  
		Last Modified: Wed, 19 Aug 2020 22:39:03 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe70fa264db739aa2161a82692cb4ba68fc48cabfe39da5804288dd00a6cf3d`  
		Last Modified: Wed, 19 Aug 2020 22:39:03 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - linux; s390x

```console
$ docker pull mongo@sha256:0a943b86abdac8a82df902143a2b0cd8d5cc8eec9a3b49ab918cba241f220519
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160603894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d8768d9bd1fffc1bfe2301e67d6d4d5e4f4e506ff2e8de2e6237d066bd9ed84`
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
# Wed, 19 Aug 2020 22:12:36 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 19 Aug 2020 22:12:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:12:38 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:12:38 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:12:38 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:12:38 GMT
ENV MONGO_MAJOR=4.2
# Wed, 19 Aug 2020 22:12:39 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 19 Aug 2020 22:12:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:12:59 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:13:09 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:13:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:13:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:13:10 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:13:11 GMT
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
	-	`sha256:36c1f84903b9d4be36bcfb63bc0673f9d027922a0927bceb59bc4fc20e572432`  
		Last Modified: Wed, 19 Aug 2020 22:14:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74e8de2ffc25051eac0bad58f8dd9e4d7e366f8eb5baa4eeb8fc94e7a6c5781`  
		Last Modified: Wed, 19 Aug 2020 22:14:16 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b8123363956f36be5837bf22a3a4b2e9374286424bada968faa9ec2a45d76e`  
		Last Modified: Wed, 19 Aug 2020 22:14:31 GMT  
		Size: 126.7 MB (126737747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128606e9bea6ea651d3fef77dc073b1f6968d357a3b97d07f0704a13721cc6f6`  
		Last Modified: Wed, 19 Aug 2020 22:14:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944f45fc7024dea46dd82727969fd5588ac374bdc37c6a4661dcfdfe968f6421`  
		Last Modified: Wed, 19 Aug 2020 22:14:16 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:ba94700a194453d8cd720213434e35e92fc2dcaf88cb3d3c0b2b4993f2743cd7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5834871231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0109bc2c3b21d4224c17d35ae5e5b9015e920ccf4c024afc416affd631c1f5d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:02:04 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 12 Aug 2020 20:02:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 12 Aug 2020 20:02:05 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 12 Aug 2020 20:15:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:15:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:15:45 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:15:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22abf30a235006bd84369b4c2f28c7514fb54df61565615cbe7163009282fa`  
		Last Modified: Wed, 12 Aug 2020 21:13:57 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05444b18dcb481c307188a4f4749118846698e11e5de785d7d903f8fc367430c`  
		Last Modified: Wed, 12 Aug 2020 21:13:57 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e84f0a0bd7fca59d06eaff58d16fa670fe03c250ce401f1358a87b40d04c6`  
		Last Modified: Wed, 12 Aug 2020 21:13:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddebb7ba4b31efcec93d29822e85dcd7c867b607f443ddecc061eccce998330c`  
		Last Modified: Wed, 12 Aug 2020 21:14:17 GMT  
		Size: 96.7 MB (96715828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c135c56289c2b4490692cc23491f982fe13746cd24db0a9996818e72bf8b88`  
		Last Modified: Wed, 12 Aug 2020 21:13:54 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d78d4029c5e493b2e93086a109ac0db5f4c1eb3b228845487273751b090a2`  
		Last Modified: Wed, 12 Aug 2020 21:13:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fee93a9d7aca9fff7fdddaf12c1b96bfa4e2e104d7f3b3ba85da1eb9e2757c`  
		Last Modified: Wed, 12 Aug 2020 21:13:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:4d4b270e5fdf1ef4e14c6a64e9ba4e5de2637af467a26a9b812a68e78124918b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794057038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fb200062c1444cf004c8e5573f661768f8411bcc87ce5046b6cf1e0c687634d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:15:51 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 12 Aug 2020 20:15:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 12 Aug 2020 20:15:53 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 12 Aug 2020 20:34:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:34:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:34:51 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:34:51 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8f485c4fcf17152559a89206593fe2a133559ae35b8e5226df18233bb6a29d`  
		Last Modified: Wed, 12 Aug 2020 21:14:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c29d0f444afad58be341423334f449d8c68227100b7812ddc6849a12311023`  
		Last Modified: Wed, 12 Aug 2020 21:14:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8541d508faef1ced258bf2fe60980350cdf2245cd6a5affa7523f4aac9aed0`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0a380939bd96fc14221db1d7f04347148ceb109ddaaf9a877f59e4aef5030c`  
		Last Modified: Wed, 12 Aug 2020 21:15:29 GMT  
		Size: 458.2 MB (458182108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8dbdadace66db5cd38a5d4b83b62f3189dad48632d294f3adea9b05eddef40`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5c66b3b07de4ebee8cac55df14e73a9c6878373f632e390d01479af4dee19`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ac22a1e2aa9b42ffa192f0909b4c32685854553fc1b0bae6366659adce675d`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2.9`

**does not exist** (yet?)

## `mongo:4.2.9-bionic`

**does not exist** (yet?)

## `mongo:4.2.9-windowsservercore`

**does not exist** (yet?)

## `mongo:4.2.9-windowsservercore-1809`

**does not exist** (yet?)

## `mongo:4.2.9-windowsservercore-ltsc2016`

**does not exist** (yet?)

## `mongo:4.2-bionic`

```console
$ docker pull mongo@sha256:ace03acac85f185981731116fa39bf01b3f2aa98620f5e5f04cf40815aa2aaec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.2-bionic` - linux; amd64

```console
$ docker pull mongo@sha256:a658234b5e704b9694ddf1d0343baff2999ddeb1401d4bdd16f29798ac8fbd12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.7 MB (164665557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9775815948bc46df5e2a2a6a7676a322b03fd4378d95df888cb498565685c10`
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
# Wed, 19 Aug 2020 23:28:21 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 19 Aug 2020 23:28:22 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 23:28:22 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 23:28:23 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:28:23 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 23:28:23 GMT
ENV MONGO_MAJOR=4.2
# Wed, 19 Aug 2020 23:28:23 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 19 Aug 2020 23:28:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 23:28:42 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 23:28:43 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 23:28:43 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 23:28:43 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 23:28:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:28:44 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 23:28:44 GMT
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
	-	`sha256:a614d629c2848a030f38b31b71a781c61f88d97a18cf381187f286cdb0527ba1`  
		Last Modified: Wed, 19 Aug 2020 23:30:18 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477320af2dcc05dc13295366b1ec14e08bf8d39c58861691b12586cebd70ebdd`  
		Last Modified: Wed, 19 Aug 2020 23:30:18 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aab702fcf56b224102ecf54a4d0af0a1b42b81df1fddee78b15c08cf54c2ad`  
		Last Modified: Wed, 19 Aug 2020 23:30:36 GMT  
		Size: 129.1 MB (129122344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94c6a2dc294267bbab1718f5e4948528dda38dc8312e00f513764125789810a`  
		Last Modified: Wed, 19 Aug 2020 23:30:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf889bdb7c65ff5ae1e72f60f8a22ae4cb324b4756c3321dfc270650efe7ad7`  
		Last Modified: Wed, 19 Aug 2020 23:30:18 GMT  
		Size: 4.0 KB (3950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:8ae70bed1137fd41febc74bc981f907b38e0264505165474d3adc75f50d53549
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.7 MB (154678350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e194770a8c8f0ac94c5355d49778d13fda23873aaf571ee712fbe9e14af3a58d`
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
# Wed, 19 Aug 2020 22:35:23 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 19 Aug 2020 22:35:26 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:35:26 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:35:27 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:35:28 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:35:30 GMT
ENV MONGO_MAJOR=4.2
# Wed, 19 Aug 2020 22:35:31 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 19 Aug 2020 22:35:33 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:36:02 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:36:05 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:36:06 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:36:07 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:36:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:36:09 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:36:11 GMT
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
	-	`sha256:1e3d9c6e96a39031cb9c1dc26cda911d8e36de718489edcb4257c2cbd5735e11`  
		Last Modified: Wed, 19 Aug 2020 22:39:03 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66651b0c33490b229f317298c74d09923988c8f392133e9aec200c2ed2349db4`  
		Last Modified: Wed, 19 Aug 2020 22:39:03 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053ed69102564ccae4e255643d87f86b3dec330e99f02a280d41566b9fe070fe`  
		Last Modified: Wed, 19 Aug 2020 22:39:31 GMT  
		Size: 122.9 MB (122900327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9bdc108220d80f0f46736b9035de7cb84d596d1ae7a722f46c698e1c2502b2`  
		Last Modified: Wed, 19 Aug 2020 22:39:03 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe70fa264db739aa2161a82692cb4ba68fc48cabfe39da5804288dd00a6cf3d`  
		Last Modified: Wed, 19 Aug 2020 22:39:03 GMT  
		Size: 4.0 KB (3951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:0a943b86abdac8a82df902143a2b0cd8d5cc8eec9a3b49ab918cba241f220519
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160603894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d8768d9bd1fffc1bfe2301e67d6d4d5e4f4e506ff2e8de2e6237d066bd9ed84`
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
# Wed, 19 Aug 2020 22:12:36 GMT
ENV GPG_KEYS=E162F504A20CDF15827F718D4B7C549A058F8B6B
# Wed, 19 Aug 2020 22:12:38 GMT
RUN set -ex; 	export GNUPGHOME="$(mktemp -d)"; 	for key in $GPG_KEYS; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --export $GPG_KEYS > /etc/apt/trusted.gpg.d/mongodb.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -r "$GNUPGHOME"; 	apt-key list
# Wed, 19 Aug 2020 22:12:38 GMT
ARG MONGO_PACKAGE=mongodb-org
# Wed, 19 Aug 2020 22:12:38 GMT
ARG MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:12:38 GMT
ENV MONGO_PACKAGE=mongodb-org MONGO_REPO=repo.mongodb.org
# Wed, 19 Aug 2020 22:12:38 GMT
ENV MONGO_MAJOR=4.2
# Wed, 19 Aug 2020 22:12:39 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 19 Aug 2020 22:12:39 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:12:59 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:09 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:13:09 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:13:10 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:13:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:13:10 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:13:11 GMT
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
	-	`sha256:36c1f84903b9d4be36bcfb63bc0673f9d027922a0927bceb59bc4fc20e572432`  
		Last Modified: Wed, 19 Aug 2020 22:14:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74e8de2ffc25051eac0bad58f8dd9e4d7e366f8eb5baa4eeb8fc94e7a6c5781`  
		Last Modified: Wed, 19 Aug 2020 22:14:16 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b8123363956f36be5837bf22a3a4b2e9374286424bada968faa9ec2a45d76e`  
		Last Modified: Wed, 19 Aug 2020 22:14:31 GMT  
		Size: 126.7 MB (126737747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128606e9bea6ea651d3fef77dc073b1f6968d357a3b97d07f0704a13721cc6f6`  
		Last Modified: Wed, 19 Aug 2020 22:14:16 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944f45fc7024dea46dd82727969fd5588ac374bdc37c6a4661dcfdfe968f6421`  
		Last Modified: Wed, 19 Aug 2020 22:14:16 GMT  
		Size: 4.0 KB (3952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore`

```console
$ docker pull mongo@sha256:437a166802f907c8c0873ef4557356335d311b0f74639eb238e6b05607ec6de5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.2-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:ba94700a194453d8cd720213434e35e92fc2dcaf88cb3d3c0b2b4993f2743cd7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5834871231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0109bc2c3b21d4224c17d35ae5e5b9015e920ccf4c024afc416affd631c1f5d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:02:04 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 12 Aug 2020 20:02:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 12 Aug 2020 20:02:05 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 12 Aug 2020 20:15:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:15:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:15:45 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:15:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22abf30a235006bd84369b4c2f28c7514fb54df61565615cbe7163009282fa`  
		Last Modified: Wed, 12 Aug 2020 21:13:57 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05444b18dcb481c307188a4f4749118846698e11e5de785d7d903f8fc367430c`  
		Last Modified: Wed, 12 Aug 2020 21:13:57 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e84f0a0bd7fca59d06eaff58d16fa670fe03c250ce401f1358a87b40d04c6`  
		Last Modified: Wed, 12 Aug 2020 21:13:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddebb7ba4b31efcec93d29822e85dcd7c867b607f443ddecc061eccce998330c`  
		Last Modified: Wed, 12 Aug 2020 21:14:17 GMT  
		Size: 96.7 MB (96715828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c135c56289c2b4490692cc23491f982fe13746cd24db0a9996818e72bf8b88`  
		Last Modified: Wed, 12 Aug 2020 21:13:54 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d78d4029c5e493b2e93086a109ac0db5f4c1eb3b228845487273751b090a2`  
		Last Modified: Wed, 12 Aug 2020 21:13:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fee93a9d7aca9fff7fdddaf12c1b96bfa4e2e104d7f3b3ba85da1eb9e2757c`  
		Last Modified: Wed, 12 Aug 2020 21:13:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.2-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:4d4b270e5fdf1ef4e14c6a64e9ba4e5de2637af467a26a9b812a68e78124918b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794057038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fb200062c1444cf004c8e5573f661768f8411bcc87ce5046b6cf1e0c687634d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:15:51 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 12 Aug 2020 20:15:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 12 Aug 2020 20:15:53 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 12 Aug 2020 20:34:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:34:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:34:51 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:34:51 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8f485c4fcf17152559a89206593fe2a133559ae35b8e5226df18233bb6a29d`  
		Last Modified: Wed, 12 Aug 2020 21:14:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c29d0f444afad58be341423334f449d8c68227100b7812ddc6849a12311023`  
		Last Modified: Wed, 12 Aug 2020 21:14:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8541d508faef1ced258bf2fe60980350cdf2245cd6a5affa7523f4aac9aed0`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0a380939bd96fc14221db1d7f04347148ceb109ddaaf9a877f59e4aef5030c`  
		Last Modified: Wed, 12 Aug 2020 21:15:29 GMT  
		Size: 458.2 MB (458182108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8dbdadace66db5cd38a5d4b83b62f3189dad48632d294f3adea9b05eddef40`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5c66b3b07de4ebee8cac55df14e73a9c6878373f632e390d01479af4dee19`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ac22a1e2aa9b42ffa192f0909b4c32685854553fc1b0bae6366659adce675d`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-1809`

```console
$ docker pull mongo@sha256:45bcd878e9de8fa009acca63738e6541d42cb56f580c57cb64b859927ceb3637
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.2-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:4d4b270e5fdf1ef4e14c6a64e9ba4e5de2637af467a26a9b812a68e78124918b
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2794057038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fb200062c1444cf004c8e5573f661768f8411bcc87ce5046b6cf1e0c687634d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:15:51 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 12 Aug 2020 20:15:52 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 12 Aug 2020 20:15:53 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 12 Aug 2020 20:34:49 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:34:50 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:34:51 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:34:51 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8f485c4fcf17152559a89206593fe2a133559ae35b8e5226df18233bb6a29d`  
		Last Modified: Wed, 12 Aug 2020 21:14:31 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c29d0f444afad58be341423334f449d8c68227100b7812ddc6849a12311023`  
		Last Modified: Wed, 12 Aug 2020 21:14:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8541d508faef1ced258bf2fe60980350cdf2245cd6a5affa7523f4aac9aed0`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0a380939bd96fc14221db1d7f04347148ceb109ddaaf9a877f59e4aef5030c`  
		Last Modified: Wed, 12 Aug 2020 21:15:29 GMT  
		Size: 458.2 MB (458182108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8dbdadace66db5cd38a5d4b83b62f3189dad48632d294f3adea9b05eddef40`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc5c66b3b07de4ebee8cac55df14e73a9c6878373f632e390d01479af4dee19`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ac22a1e2aa9b42ffa192f0909b4c32685854553fc1b0bae6366659adce675d`  
		Last Modified: Wed, 12 Aug 2020 21:14:28 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.2-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:505e56a5eac4b4b9d217495a8e8d6aaf3063bcec4f133a80ea6f42c4245a8f40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `mongo:4.2-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:ba94700a194453d8cd720213434e35e92fc2dcaf88cb3d3c0b2b4993f2743cd7
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5834871231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0109bc2c3b21d4224c17d35ae5e5b9015e920ccf4c024afc416affd631c1f5d`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:02:04 GMT
ENV MONGO_VERSION=4.2.8
# Wed, 12 Aug 2020 20:02:04 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/win32/mongodb-win32-x86_64-2012plus-4.2.8-signed.msi
# Wed, 12 Aug 2020 20:02:05 GMT
ENV MONGO_DOWNLOAD_SHA256=166c5cd99132d72969a67446e494da6287710a34f3f75ee9fb798a2945c0f502
# Wed, 12 Aug 2020 20:15:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:15:44 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:15:45 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:15:46 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22abf30a235006bd84369b4c2f28c7514fb54df61565615cbe7163009282fa`  
		Last Modified: Wed, 12 Aug 2020 21:13:57 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05444b18dcb481c307188a4f4749118846698e11e5de785d7d903f8fc367430c`  
		Last Modified: Wed, 12 Aug 2020 21:13:57 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3e84f0a0bd7fca59d06eaff58d16fa670fe03c250ce401f1358a87b40d04c6`  
		Last Modified: Wed, 12 Aug 2020 21:13:54 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddebb7ba4b31efcec93d29822e85dcd7c867b607f443ddecc061eccce998330c`  
		Last Modified: Wed, 12 Aug 2020 21:14:17 GMT  
		Size: 96.7 MB (96715828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c135c56289c2b4490692cc23491f982fe13746cd24db0a9996818e72bf8b88`  
		Last Modified: Wed, 12 Aug 2020 21:13:54 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740d78d4029c5e493b2e93086a109ac0db5f4c1eb3b228845487273751b090a2`  
		Last Modified: Wed, 12 Aug 2020 21:13:55 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fee93a9d7aca9fff7fdddaf12c1b96bfa4e2e104d7f3b3ba85da1eb9e2757c`  
		Last Modified: Wed, 12 Aug 2020 21:13:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4`

```console
$ docker pull mongo@sha256:df9eca84736a666d5f7e7a09aeb8a6d8d073698d5b7349400f10ee75812e0e95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.4` - linux; amd64

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

### `mongo:4.4` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cd9b4445508d088608aff8d49a6de9bfc1d3eea3b0b223827ecaa27fcc51f9f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167923219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2b6b0873dbe42c8f7859603bdf939f17da04f4b468f9f25af6c6169aa6ca1f`
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
# Wed, 19 Aug 2020 22:36:36 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:36:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:37:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:37:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:37:13 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:37:14 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:37:16 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:37:17 GMT
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
	-	`sha256:faf61d67c581443a883e2b613e3832d2b2c991daa9b1c47410ccff5499e08fc6`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e437891cf74a6a9aba16ead456655e997c04f2fce5794ee214e388178d5fa1c`  
		Last Modified: Wed, 19 Aug 2020 22:40:10 GMT  
		Size: 136.1 MB (136145203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6914935be6ab626955ca4669ee6c7e69d6919abbbf5596db6e87967d01f8fd5f`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cba816b02f9834a93a91560660b43bfcddf84ecf7220ed71e3c2e69f02ab`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - linux; s390x

```console
$ docker pull mongo@sha256:f143bbac6c00e2157a08274e3fb3bf81641e8ac6341a67fff503ed8e5cbebd2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172900638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5495d92d4faf769b9cf64e94c235bbd595e7d6a701ce9cf6ecf4be08a7f5aa`
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
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:13:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:13:43 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:14:00 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:14:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:14:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:14:01 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:14:01 GMT
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
	-	`sha256:2e6595175e6368e1261954ecbe6d1b5d361c7389fca7bc5f0a2061773f01ea6c`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2840e6d43940c9bb7c109a8fcd575df74022ebc13d8a34f1d23b8ec4dd1d6517`  
		Last Modified: Wed, 19 Aug 2020 22:14:57 GMT  
		Size: 139.0 MB (139034494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac410b9916e625ac10d52cc3780a917dc6afd2de331872d5b1de148ebf852971`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241abb48b4fe9fa1d0d6c73748732e0afd16262dcb18add879e2a8a47ecb9b2d`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0`

```console
$ docker pull mongo@sha256:df9eca84736a666d5f7e7a09aeb8a6d8d073698d5b7349400f10ee75812e0e95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.4.0` - linux; amd64

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

### `mongo:4.4.0` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cd9b4445508d088608aff8d49a6de9bfc1d3eea3b0b223827ecaa27fcc51f9f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167923219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2b6b0873dbe42c8f7859603bdf939f17da04f4b468f9f25af6c6169aa6ca1f`
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
# Wed, 19 Aug 2020 22:36:36 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:36:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:37:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:37:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:37:13 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:37:14 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:37:16 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:37:17 GMT
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
	-	`sha256:faf61d67c581443a883e2b613e3832d2b2c991daa9b1c47410ccff5499e08fc6`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e437891cf74a6a9aba16ead456655e997c04f2fce5794ee214e388178d5fa1c`  
		Last Modified: Wed, 19 Aug 2020 22:40:10 GMT  
		Size: 136.1 MB (136145203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6914935be6ab626955ca4669ee6c7e69d6919abbbf5596db6e87967d01f8fd5f`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cba816b02f9834a93a91560660b43bfcddf84ecf7220ed71e3c2e69f02ab`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0` - linux; s390x

```console
$ docker pull mongo@sha256:f143bbac6c00e2157a08274e3fb3bf81641e8ac6341a67fff503ed8e5cbebd2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172900638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5495d92d4faf769b9cf64e94c235bbd595e7d6a701ce9cf6ecf4be08a7f5aa`
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
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:13:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:13:43 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:14:00 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:14:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:14:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:14:01 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:14:01 GMT
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
	-	`sha256:2e6595175e6368e1261954ecbe6d1b5d361c7389fca7bc5f0a2061773f01ea6c`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2840e6d43940c9bb7c109a8fcd575df74022ebc13d8a34f1d23b8ec4dd1d6517`  
		Last Modified: Wed, 19 Aug 2020 22:14:57 GMT  
		Size: 139.0 MB (139034494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac410b9916e625ac10d52cc3780a917dc6afd2de331872d5b1de148ebf852971`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241abb48b4fe9fa1d0d6c73748732e0afd16262dcb18add879e2a8a47ecb9b2d`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-bionic`

```console
$ docker pull mongo@sha256:b7de11e3dc4a8fd787e4e1cb7a7fc49e5015fe649ba82090a2d74280425b9c3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4.0-bionic` - linux; amd64

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

### `mongo:4.4.0-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cd9b4445508d088608aff8d49a6de9bfc1d3eea3b0b223827ecaa27fcc51f9f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167923219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2b6b0873dbe42c8f7859603bdf939f17da04f4b468f9f25af6c6169aa6ca1f`
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
# Wed, 19 Aug 2020 22:36:36 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:36:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:37:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:37:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:37:13 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:37:14 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:37:16 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:37:17 GMT
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
	-	`sha256:faf61d67c581443a883e2b613e3832d2b2c991daa9b1c47410ccff5499e08fc6`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e437891cf74a6a9aba16ead456655e997c04f2fce5794ee214e388178d5fa1c`  
		Last Modified: Wed, 19 Aug 2020 22:40:10 GMT  
		Size: 136.1 MB (136145203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6914935be6ab626955ca4669ee6c7e69d6919abbbf5596db6e87967d01f8fd5f`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cba816b02f9834a93a91560660b43bfcddf84ecf7220ed71e3c2e69f02ab`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:f143bbac6c00e2157a08274e3fb3bf81641e8ac6341a67fff503ed8e5cbebd2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172900638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5495d92d4faf769b9cf64e94c235bbd595e7d6a701ce9cf6ecf4be08a7f5aa`
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
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:13:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:13:43 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:14:00 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:14:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:14:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:14:01 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:14:01 GMT
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
	-	`sha256:2e6595175e6368e1261954ecbe6d1b5d361c7389fca7bc5f0a2061773f01ea6c`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2840e6d43940c9bb7c109a8fcd575df74022ebc13d8a34f1d23b8ec4dd1d6517`  
		Last Modified: Wed, 19 Aug 2020 22:14:57 GMT  
		Size: 139.0 MB (139034494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac410b9916e625ac10d52cc3780a917dc6afd2de331872d5b1de148ebf852971`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241abb48b4fe9fa1d0d6c73748732e0afd16262dcb18add879e2a8a47ecb9b2d`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-windowsservercore`

```console
$ docker pull mongo@sha256:aece32dee1891f275d9e103ec8c905d8f35d050ba07bb3bc0d9439ad6a7830e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.4.0-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4.0-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-windowsservercore-1809`

```console
$ docker pull mongo@sha256:7fa3a689c42da7c9d0b4da47a52638d8006d166dbe15fb3b66d47bece05a3402
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.4.0-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4.0-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:08e24b657f1adcec61252f30bd55a9bf761467750aa4199ee7013ea4980d039a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `mongo:4.4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-bionic`

```console
$ docker pull mongo@sha256:b7de11e3dc4a8fd787e4e1cb7a7fc49e5015fe649ba82090a2d74280425b9c3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4.4-bionic` - linux; amd64

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

### `mongo:4.4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cd9b4445508d088608aff8d49a6de9bfc1d3eea3b0b223827ecaa27fcc51f9f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167923219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2b6b0873dbe42c8f7859603bdf939f17da04f4b468f9f25af6c6169aa6ca1f`
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
# Wed, 19 Aug 2020 22:36:36 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:36:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:37:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:37:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:37:13 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:37:14 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:37:16 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:37:17 GMT
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
	-	`sha256:faf61d67c581443a883e2b613e3832d2b2c991daa9b1c47410ccff5499e08fc6`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e437891cf74a6a9aba16ead456655e997c04f2fce5794ee214e388178d5fa1c`  
		Last Modified: Wed, 19 Aug 2020 22:40:10 GMT  
		Size: 136.1 MB (136145203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6914935be6ab626955ca4669ee6c7e69d6919abbbf5596db6e87967d01f8fd5f`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cba816b02f9834a93a91560660b43bfcddf84ecf7220ed71e3c2e69f02ab`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:f143bbac6c00e2157a08274e3fb3bf81641e8ac6341a67fff503ed8e5cbebd2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172900638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5495d92d4faf769b9cf64e94c235bbd595e7d6a701ce9cf6ecf4be08a7f5aa`
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
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:13:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:13:43 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:14:00 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:14:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:14:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:14:01 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:14:01 GMT
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
	-	`sha256:2e6595175e6368e1261954ecbe6d1b5d361c7389fca7bc5f0a2061773f01ea6c`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2840e6d43940c9bb7c109a8fcd575df74022ebc13d8a34f1d23b8ec4dd1d6517`  
		Last Modified: Wed, 19 Aug 2020 22:14:57 GMT  
		Size: 139.0 MB (139034494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac410b9916e625ac10d52cc3780a917dc6afd2de331872d5b1de148ebf852971`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241abb48b4fe9fa1d0d6c73748732e0afd16262dcb18add879e2a8a47ecb9b2d`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore`

```console
$ docker pull mongo@sha256:aece32dee1891f275d9e103ec8c905d8f35d050ba07bb3bc0d9439ad6a7830e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.4-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4.4-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:7fa3a689c42da7c9d0b4da47a52638d8006d166dbe15fb3b66d47bece05a3402
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `mongo:4.4-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4.4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:08e24b657f1adcec61252f30bd55a9bf761467750aa4199ee7013ea4980d039a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `mongo:4.4-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-bionic`

```console
$ docker pull mongo@sha256:b7de11e3dc4a8fd787e4e1cb7a7fc49e5015fe649ba82090a2d74280425b9c3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `mongo:4-bionic` - linux; amd64

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

### `mongo:4-bionic` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cd9b4445508d088608aff8d49a6de9bfc1d3eea3b0b223827ecaa27fcc51f9f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167923219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2b6b0873dbe42c8f7859603bdf939f17da04f4b468f9f25af6c6169aa6ca1f`
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
# Wed, 19 Aug 2020 22:36:36 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:36:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:37:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:37:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:37:13 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:37:14 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:37:16 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:37:17 GMT
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
	-	`sha256:faf61d67c581443a883e2b613e3832d2b2c991daa9b1c47410ccff5499e08fc6`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e437891cf74a6a9aba16ead456655e997c04f2fce5794ee214e388178d5fa1c`  
		Last Modified: Wed, 19 Aug 2020 22:40:10 GMT  
		Size: 136.1 MB (136145203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6914935be6ab626955ca4669ee6c7e69d6919abbbf5596db6e87967d01f8fd5f`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cba816b02f9834a93a91560660b43bfcddf84ecf7220ed71e3c2e69f02ab`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-bionic` - linux; s390x

```console
$ docker pull mongo@sha256:f143bbac6c00e2157a08274e3fb3bf81641e8ac6341a67fff503ed8e5cbebd2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172900638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5495d92d4faf769b9cf64e94c235bbd595e7d6a701ce9cf6ecf4be08a7f5aa`
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
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:13:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:13:43 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:14:00 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:14:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:14:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:14:01 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:14:01 GMT
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
	-	`sha256:2e6595175e6368e1261954ecbe6d1b5d361c7389fca7bc5f0a2061773f01ea6c`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2840e6d43940c9bb7c109a8fcd575df74022ebc13d8a34f1d23b8ec4dd1d6517`  
		Last Modified: Wed, 19 Aug 2020 22:14:57 GMT  
		Size: 139.0 MB (139034494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac410b9916e625ac10d52cc3780a917dc6afd2de331872d5b1de148ebf852971`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241abb48b4fe9fa1d0d6c73748732e0afd16262dcb18add879e2a8a47ecb9b2d`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore`

```console
$ docker pull mongo@sha256:aece32dee1891f275d9e103ec8c905d8f35d050ba07bb3bc0d9439ad6a7830e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:4-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-1809`

```console
$ docker pull mongo@sha256:7fa3a689c42da7c9d0b4da47a52638d8006d166dbe15fb3b66d47bece05a3402
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `mongo:4-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:4-windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:08e24b657f1adcec61252f30bd55a9bf761467750aa4199ee7013ea4980d039a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `mongo:4-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:bionic`

```console
$ docker pull mongo@sha256:b7de11e3dc4a8fd787e4e1cb7a7fc49e5015fe649ba82090a2d74280425b9c3e
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
$ docker pull mongo@sha256:cd9b4445508d088608aff8d49a6de9bfc1d3eea3b0b223827ecaa27fcc51f9f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167923219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2b6b0873dbe42c8f7859603bdf939f17da04f4b468f9f25af6c6169aa6ca1f`
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
# Wed, 19 Aug 2020 22:36:36 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:36:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:37:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:37:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:37:13 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:37:14 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:37:16 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:37:17 GMT
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
	-	`sha256:faf61d67c581443a883e2b613e3832d2b2c991daa9b1c47410ccff5499e08fc6`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e437891cf74a6a9aba16ead456655e997c04f2fce5794ee214e388178d5fa1c`  
		Last Modified: Wed, 19 Aug 2020 22:40:10 GMT  
		Size: 136.1 MB (136145203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6914935be6ab626955ca4669ee6c7e69d6919abbbf5596db6e87967d01f8fd5f`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cba816b02f9834a93a91560660b43bfcddf84ecf7220ed71e3c2e69f02ab`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:bionic` - linux; s390x

```console
$ docker pull mongo@sha256:f143bbac6c00e2157a08274e3fb3bf81641e8ac6341a67fff503ed8e5cbebd2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172900638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5495d92d4faf769b9cf64e94c235bbd595e7d6a701ce9cf6ecf4be08a7f5aa`
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
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:13:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:13:43 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:14:00 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:14:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:14:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:14:01 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:14:01 GMT
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
	-	`sha256:2e6595175e6368e1261954ecbe6d1b5d361c7389fca7bc5f0a2061773f01ea6c`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2840e6d43940c9bb7c109a8fcd575df74022ebc13d8a34f1d23b8ec4dd1d6517`  
		Last Modified: Wed, 19 Aug 2020 22:14:57 GMT  
		Size: 139.0 MB (139034494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac410b9916e625ac10d52cc3780a917dc6afd2de331872d5b1de148ebf852971`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241abb48b4fe9fa1d0d6c73748732e0afd16262dcb18add879e2a8a47ecb9b2d`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:latest`

```console
$ docker pull mongo@sha256:df9eca84736a666d5f7e7a09aeb8a6d8d073698d5b7349400f10ee75812e0e95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:latest` - linux; amd64

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

### `mongo:latest` - linux; arm64 variant v8

```console
$ docker pull mongo@sha256:cd9b4445508d088608aff8d49a6de9bfc1d3eea3b0b223827ecaa27fcc51f9f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.9 MB (167923219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2b6b0873dbe42c8f7859603bdf939f17da04f4b468f9f25af6c6169aa6ca1f`
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
# Wed, 19 Aug 2020 22:36:36 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:36:38 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:37:08 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:37:13 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:37:13 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:37:14 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:37:16 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:37:17 GMT
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
	-	`sha256:faf61d67c581443a883e2b613e3832d2b2c991daa9b1c47410ccff5499e08fc6`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e437891cf74a6a9aba16ead456655e997c04f2fce5794ee214e388178d5fa1c`  
		Last Modified: Wed, 19 Aug 2020 22:40:10 GMT  
		Size: 136.1 MB (136145203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6914935be6ab626955ca4669ee6c7e69d6919abbbf5596db6e87967d01f8fd5f`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cba816b02f9834a93a91560660b43bfcddf84ecf7220ed71e3c2e69f02ab`  
		Last Modified: Wed, 19 Aug 2020 22:39:38 GMT  
		Size: 4.0 KB (3954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - linux; s390x

```console
$ docker pull mongo@sha256:f143bbac6c00e2157a08274e3fb3bf81641e8ac6341a67fff503ed8e5cbebd2e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172900638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5495d92d4faf769b9cf64e94c235bbd595e7d6a701ce9cf6ecf4be08a7f5aa`
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
# Wed, 19 Aug 2020 22:13:23 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 19 Aug 2020 22:13:24 GMT
RUN echo "deb http://$MONGO_REPO/apt/ubuntu bionic/${MONGO_PACKAGE%-unstable}/$MONGO_MAJOR multiverse" | tee "/etc/apt/sources.list.d/${MONGO_PACKAGE%-unstable}.list"
# Wed, 19 Aug 2020 22:13:43 GMT
RUN set -x 	&& export DEBIAN_FRONTEND=noninteractive 	&& apt-get update 	&& ln -s /bin/true /usr/local/bin/systemctl 	&& apt-get install -y 		${MONGO_PACKAGE}=$MONGO_VERSION 		${MONGO_PACKAGE}-server=$MONGO_VERSION 		${MONGO_PACKAGE}-shell=$MONGO_VERSION 		${MONGO_PACKAGE}-mongos=$MONGO_VERSION 		${MONGO_PACKAGE}-tools=$MONGO_VERSION 	&& rm -f /usr/local/bin/systemctl 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /var/lib/mongodb 	&& mv /etc/mongod.conf /etc/mongod.conf.orig
# Wed, 19 Aug 2020 22:13:59 GMT
RUN mkdir -p /data/db /data/configdb 	&& chown -R mongodb:mongodb /data/db /data/configdb
# Wed, 19 Aug 2020 22:14:00 GMT
VOLUME [/data/db /data/configdb]
# Wed, 19 Aug 2020 22:14:00 GMT
COPY file:c3beae20a29d6d69ecab76830068690f9c4f9d77d82eb60160db72670df64615 in /usr/local/bin/ 
# Wed, 19 Aug 2020 22:14:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:14:01 GMT
EXPOSE 27017
# Wed, 19 Aug 2020 22:14:01 GMT
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
	-	`sha256:2e6595175e6368e1261954ecbe6d1b5d361c7389fca7bc5f0a2061773f01ea6c`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2840e6d43940c9bb7c109a8fcd575df74022ebc13d8a34f1d23b8ec4dd1d6517`  
		Last Modified: Wed, 19 Aug 2020 22:14:57 GMT  
		Size: 139.0 MB (139034494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac410b9916e625ac10d52cc3780a917dc6afd2de331872d5b1de148ebf852971`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241abb48b4fe9fa1d0d6c73748732e0afd16262dcb18add879e2a8a47ecb9b2d`  
		Last Modified: Wed, 19 Aug 2020 22:14:38 GMT  
		Size: 4.0 KB (3953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:latest` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore`

```console
$ docker pull mongo@sha256:aece32dee1891f275d9e103ec8c905d8f35d050ba07bb3bc0d9439ad6a7830e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64
	-	windows version 10.0.17763.1397; amd64

### `mongo:windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-1809`

```console
$ docker pull mongo@sha256:7fa3a689c42da7c9d0b4da47a52638d8006d166dbe15fb3b66d47bece05a3402
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `mongo:windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull mongo@sha256:006709f7c65cc8a7a4080c2fac200769d26a0ec0954febcf8b24320dc88ccd35
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2386027760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a02677d3a3ef0268b4f0b138851334a0ca6459ffa62c40b4e470cf149554b1c1`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Wed, 12 Aug 2020 12:15:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:52:56 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:52:57 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:52:58 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 21:06:33 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 21:06:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 21:06:35 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 21:06:36 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0465a83fdc9bb4320b7a8d4235d585e19f98779b5153f47841875a388f1e8a9`  
		Last Modified: Wed, 12 Aug 2020 14:51:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9d605dcdd4b80b38cea76f9f599561521b16693ac743c98707e6b567aee7fd`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1d3432ed1184c6db8559144e6eafc7fab6243192e463fa5a9a7471e6e4a72c`  
		Last Modified: Wed, 12 Aug 2020 21:16:54 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69803ed822af960657f0d3ad4394c537815ec4a5657d190bbea2b271736ca70`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee52fb13c760508a6ae90124f97ff30e866032c7e212f362e95f4aed8f86dc76`  
		Last Modified: Wed, 12 Aug 2020 21:17:00 GMT  
		Size: 50.2 MB (50152785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abada71d32589db1b8c4a8b1c31be4fb799301239f7fe2e3b476afa3550b465`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0e5f7e3e54f3df3343dc09e69752526f3492ea00e15024dad325a0ac78c80`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e611f01b622fd60c1d57cb36401a7bfba8933e67ab8553c0f83bf5a859bb76`  
		Last Modified: Wed, 12 Aug 2020 21:16:51 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo:windowsservercore-ltsc2016`

```console
$ docker pull mongo@sha256:08e24b657f1adcec61252f30bd55a9bf761467750aa4199ee7013ea4980d039a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `mongo:windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull mongo@sha256:8a19fe2347eec188238c3a59935408eaeecdd8dd5d499b7e773e2aa1aaffca1e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6151345048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78589d859f3262bf006499e263e1388e2bfbab1523a449d89c58138d6454fa43`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 Aug 2020 12:23:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 12 Aug 2020 20:35:09 GMT
ENV MONGO_VERSION=4.4.0
# Wed, 12 Aug 2020 20:35:10 GMT
ENV MONGO_DOWNLOAD_URL=https://fastdl.mongodb.org/windows/mongodb-windows-x86_64-4.4.0-signed.msi
# Wed, 12 Aug 2020 20:35:11 GMT
ENV MONGO_DOWNLOAD_SHA256=ab326721c480dfafe0d0c3c1489c25e3a411b86e830dd91151b5ae24b8c9d508
# Wed, 12 Aug 2020 20:52:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:MONGO_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	(New-Object System.Net.WebClient).DownloadFile($env:MONGO_DOWNLOAD_URL, 'mongo.msi'); 		if ($env:MONGO_DOWNLOAD_SHA256) { 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:MONGO_DOWNLOAD_SHA256); 		if ((Get-FileHash mongo.msi -Algorithm sha256).Hash -ne $env:MONGO_DOWNLOAD_SHA256) { 			Write-Host 'FAILED!'; 			exit 1; 		}; 	}; 		Write-Host 'Installing ...'; 	Start-Process msiexec -Wait 		-ArgumentList @( 			'/i', 			'mongo.msi', 			'/quiet', 			'/qn', 			'INSTALLLOCATION=C:\mongodb', 			'ADDLOCAL=all' 		); 	$env:PATH = 'C:\mongodb\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  mongo --version'; mongo --version; 	Write-Host '  mongod --version'; mongod --version; 		Write-Host 'Removing ...'; 	Remove-Item C:\mongodb\bin\*.pdb -Force; 	Remove-Item C:\windows\installer\*.msi -Force; 	Remove-Item mongo.msi -Force; 		Write-Host 'Complete.';
# Wed, 12 Aug 2020 20:52:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 12 Aug 2020 20:52:48 GMT
EXPOSE 27017
# Wed, 12 Aug 2020 20:52:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:44c31749d2d4be3aede3e54780d9e54b5a7eeaa617e1adf027e92fce2ebf0f2a`  
		Last Modified: Wed, 12 Aug 2020 14:52:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5adf59baf68d421c2650eef5874e7cd44c70737df9b55916d70b0441523012`  
		Last Modified: Wed, 12 Aug 2020 21:15:43 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2769d7eebe7f70de63f4579ee995f328999f90695f70b6d9c66df1e6eac32e`  
		Last Modified: Wed, 12 Aug 2020 21:15:42 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fdd9af48a05583ba1a22006747873bdc1ae301b3d4896b4469bbbc64860aaa`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc5473614bd23b7d08bdaaf2f34280efa79ac8c226e4e9b8dd0e066fd203287`  
		Last Modified: Wed, 12 Aug 2020 21:16:35 GMT  
		Size: 413.2 MB (413189665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed73ecbfb716c6ca18f7ad75fef5112b5a9451cca56cf69938bea7fea278715a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa88170eb87d3731c73f727505b065e80de74560bc451358b61b2e5c5e58716`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74114785ea95bcbe74d5b44660d5bdcf72710df0ff8fe30fa1b5e1b12c12656a`  
		Last Modified: Wed, 12 Aug 2020 21:15:40 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
