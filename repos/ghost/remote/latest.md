## `ghost:latest`

```console
$ docker pull ghost@sha256:29e1e4e89fb0c1144b2933c8c8368be173bbcb1d54ffb8146fe4512d57c8ae58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:latest` - linux; amd64

```console
$ docker pull ghost@sha256:c5ae135c5a7fec520cd284223b5291772ed265b4713aba5135bf5a2530a66953
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138551711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:feccb1ef917363c6338c5345f65b7ccb97bdeb88fd30e5b689df582f03a013d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 12:38:47 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 15:23:56 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 15:24:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 15:24:11 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:24:22 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 15:24:23 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:24:23 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:29:05 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 18:29:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 18:29:23 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:29:24 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:29:56 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:29:57 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:29:58 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:29:58 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 18:31:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:31:48 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:31:48 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:31:49 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 18:31:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:31:49 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:31:49 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:d121f8d1c4128ebc1e95e5bfad90a0189b84eadbbb2fbaad20cbb26d20b2c8a2`  
		Last Modified: Thu, 10 Sep 2020 00:34:02 GMT  
		Size: 27.1 MB (27092161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a54a24e4e595e4a1aa398f248be0a837871007bf4b08a0eb2ecdaf7c3bbb238`  
		Last Modified: Thu, 10 Sep 2020 12:46:47 GMT  
		Size: 4.2 KB (4154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa65a634fc0ad2035be77125367f1423ed616213499206613b4b444397a1cf5`  
		Last Modified: Wed, 16 Sep 2020 15:31:23 GMT  
		Size: 24.2 MB (24197754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7634d710af87c04ae36c60a7c8bd1cef4be5601ae8469aa705156da862b175ba`  
		Last Modified: Wed, 16 Sep 2020 15:31:17 GMT  
		Size: 2.8 MB (2751789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec150ee2ad17509cd3dc3692f57d958369316a679b0baa16ed482033b4231796`  
		Last Modified: Wed, 16 Sep 2020 15:31:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d63bf0b1e87d599d9c0af240b6f498fbc1253a40e29c7e952bf2185cc6b1d60`  
		Last Modified: Wed, 16 Sep 2020 18:41:01 GMT  
		Size: 1.4 MB (1417644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2b08fee21d98aeeebb23ca9217451b8b8f97a21d7140723d21484b87c85e67`  
		Last Modified: Wed, 16 Sep 2020 18:41:06 GMT  
		Size: 7.3 MB (7300498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c40dde458723fa50129c5a8fafd9cc5b871a47e8e4a158f8004c98766f61836`  
		Last Modified: Wed, 16 Sep 2020 18:41:31 GMT  
		Size: 75.8 MB (75786881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41eca2adb4a9a2048d4a0c03c5cba1ff921036578f125a709db9d36358d2f351`  
		Last Modified: Wed, 16 Sep 2020 18:41:00 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; arm variant v7

```console
$ docker pull ghost@sha256:3722e28c6a05195657700d666b0e4a81489d8af611c41f238ecc782cec55deeb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (133957854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34fdcadad91b1297ae42464df963172e5e801f1e5ed72a5cc4764a3743bf87d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 00:08:04 GMT
ADD file:5ec0d2c3043ae64cb72698b0f6fe7387884f4195df962466215ce534d2208327 in / 
# Thu, 10 Sep 2020 00:08:06 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 07:58:25 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 08:06:01 GMT
ENV NODE_VERSION=12.18.3
# Thu, 10 Sep 2020 08:06:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Thu, 10 Sep 2020 08:06:59 GMT
ENV YARN_VERSION=1.22.4
# Thu, 10 Sep 2020 08:07:36 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Thu, 10 Sep 2020 08:07:38 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 08:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 08:07:42 GMT
CMD ["node"]
# Fri, 11 Sep 2020 00:43:52 GMT
ENV GOSU_VERSION=1.12
# Fri, 11 Sep 2020 00:44:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Sep 2020 00:44:20 GMT
ENV NODE_ENV=production
# Fri, 11 Sep 2020 00:44:21 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Fri, 11 Sep 2020 00:44:56 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 11 Sep 2020 00:44:59 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 11 Sep 2020 00:45:00 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 21:04:44 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 21:09:25 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 21:09:32 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 21:09:33 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 21:09:35 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Mon, 14 Sep 2020 21:09:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 21:09:37 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 21:09:38 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:a7c65856610cb24c46ede2ffe313cbf933c44fa20ba213835af953646f3eb1ed`  
		Last Modified: Thu, 10 Sep 2020 00:17:52 GMT  
		Size: 22.7 MB (22699896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5259d7aaf92c2d6d9a495d1d64d791213938370dcb93651e4456a2a3b7fac28`  
		Last Modified: Thu, 10 Sep 2020 08:20:14 GMT  
		Size: 4.2 KB (4169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b02cdcfcdf40dd016191c5f2d8bc958a7e44bc48d13db0003a5b06ba1169a4`  
		Last Modified: Thu, 10 Sep 2020 08:22:09 GMT  
		Size: 22.2 MB (22226922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b364da23dbccfec00783ce771a318be3ec6a8bc6fbb31d76c3c600c1b216fdec`  
		Last Modified: Thu, 10 Sep 2020 08:22:01 GMT  
		Size: 2.7 MB (2739190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7117c6042c39336b85d901e0b60e1c438abe8c6a4b45af9f9805d2b05b971a55`  
		Last Modified: Thu, 10 Sep 2020 08:22:00 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000b59e6deffe46df01fbcf824c887ee8c76bfc9ebfe73092584a4c24f9ffc4f`  
		Last Modified: Fri, 11 Sep 2020 01:02:37 GMT  
		Size: 1.4 MB (1369844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50728b47a7c6ba5512e22b2eccf4e25bde138ea6b12321adb1e31182890cc32e`  
		Last Modified: Fri, 11 Sep 2020 01:02:41 GMT  
		Size: 7.3 MB (7300095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85645fd51b12fb69f7a1c624c26ac1fddefd7c5c1e011e47763aa04b612b454e`  
		Last Modified: Mon, 14 Sep 2020 21:16:36 GMT  
		Size: 77.6 MB (77616906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3641c04f5ad020fdc17061d914f1290f4e5c4300e4fc47a888ded1902e1049f`  
		Last Modified: Mon, 14 Sep 2020 21:16:01 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:479cefdadbb07cfc9dfc3d51d1d6de90d5e4f8b6fd623c2164f2369824f045a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122369171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d97d89de22ca7c785d038a08e5958a771e021400672fbae0abe244e4c566035`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 10:17:51 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 17:34:01 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 17:34:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 17:35:00 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 17:35:51 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 17:35:53 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 17:35:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 17:35:55 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:30:22 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 19:30:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 19:30:56 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:30:56 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:31:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:31:23 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:31:24 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:31:25 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:35:33 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:35:42 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:35:43 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:35:44 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 19:35:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:35:46 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:35:47 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:a6d76de28f58f3470aff71c934c0fec4e5d0fad788f8b8bcc50601266fc1b34d`  
		Last Modified: Wed, 09 Sep 2020 23:59:09 GMT  
		Size: 25.8 MB (25849325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38e30e54dcc912cf2d85f0ac209130fb4110a6b0bbcd34d975ec5404f7e8853`  
		Last Modified: Thu, 10 Sep 2020 10:33:34 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee76dd593b47001c0362d50c04445d4e310549763310092720c7facef41c3217`  
		Last Modified: Wed, 16 Sep 2020 18:38:00 GMT  
		Size: 24.2 MB (24153836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777f77f360eaa8d3244e3f788992b50868e26ae4afc42c7e4ecb98cf5ab3baf8`  
		Last Modified: Wed, 16 Sep 2020 18:37:53 GMT  
		Size: 2.8 MB (2752100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f8acd447513e9e1fd4374ab3d557c5bc4edb7c59ecb06ff935e09b67a7dad1`  
		Last Modified: Wed, 16 Sep 2020 18:37:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72cb27badab1c61a16167d77e502bb0cd4130a632ce6b86ffef31572cae6f25a`  
		Last Modified: Wed, 16 Sep 2020 19:54:05 GMT  
		Size: 1.4 MB (1353215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1fd0aaf7fbfb97b3fcce93e27c83826333e3ee69d5b4ab9927621cd8b892ac`  
		Last Modified: Wed, 16 Sep 2020 19:54:09 GMT  
		Size: 7.3 MB (7300436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95c31ccf16bf777e4e2e1f43a53c20ddca5d067467dbc485352e20d1a2fe50b`  
		Last Modified: Wed, 16 Sep 2020 19:54:33 GMT  
		Size: 61.0 MB (60955234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128d632b0ef9992a3a43c21caa8a0d1e35125f0a81a7bb8397043de2812d4e8d`  
		Last Modified: Wed, 16 Sep 2020 19:54:05 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; ppc64le

```console
$ docker pull ghost@sha256:ec2cce6de2bea20cd876db3b6940da59ae7fad73e5672efc4c5bb1f087fab386
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127848657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e510e292f3e2209261b5a9d19a425c0b76bae10c511ec5b1c6aada825539780d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 18:13:32 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 18:28:47 GMT
ENV NODE_VERSION=12.18.3
# Thu, 10 Sep 2020 18:32:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Thu, 10 Sep 2020 18:32:51 GMT
ENV YARN_VERSION=1.22.4
# Thu, 10 Sep 2020 18:36:56 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Thu, 10 Sep 2020 18:37:01 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 18:37:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 18:37:09 GMT
CMD ["node"]
# Fri, 11 Sep 2020 21:05:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 11 Sep 2020 21:08:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Sep 2020 21:08:40 GMT
ENV NODE_ENV=production
# Fri, 11 Sep 2020 21:08:44 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Fri, 11 Sep 2020 21:10:14 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 11 Sep 2020 21:10:22 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 11 Sep 2020 21:10:25 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 18:21:16 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 18:44:09 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 18:44:26 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 18:44:48 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 18:44:57 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Mon, 14 Sep 2020 18:45:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 18:45:13 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 18:45:20 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:f8aef3d2247e5f990bc767bc99f575b9bcec34aaa37183414eebe28fcd09519d`  
		Last Modified: Thu, 10 Sep 2020 01:28:12 GMT  
		Size: 30.5 MB (30517880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739d58d52a258810b79f929b5715e4b05d3de4e888bd3cf278206c98fda26d0a`  
		Last Modified: Thu, 10 Sep 2020 18:49:40 GMT  
		Size: 4.2 KB (4207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b3367233f393765c4e4b1b3e427bab10cde7211209b80fe337c80795093c94`  
		Last Modified: Thu, 10 Sep 2020 18:50:57 GMT  
		Size: 24.0 MB (24012735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7390f9e0e9396c41e86866a3e9463bb4fb97422ee6efedc41fbfd6e65d59fcaf`  
		Last Modified: Thu, 10 Sep 2020 18:50:51 GMT  
		Size: 2.8 MB (2750286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f44d6fe0381940066824aed1e4e47a83dfdc62e63c3b22b3f91e51b0c0796b`  
		Last Modified: Thu, 10 Sep 2020 18:50:49 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a265000f3233593b1aed4599583a5d084f349c6e234ffa1f51c52d3343c9fede`  
		Last Modified: Fri, 11 Sep 2020 21:38:48 GMT  
		Size: 1.3 MB (1338657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de08b388e6cd629dfcfe759e80da2acaef27e5b88ab1fa89aceeb5fc9c17bb7`  
		Last Modified: Fri, 11 Sep 2020 21:39:10 GMT  
		Size: 7.3 MB (7300236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef1c719b0bb4b86600e6cf2975573848ed0590b8dd9308087c33f37e04c86f9`  
		Last Modified: Mon, 14 Sep 2020 19:11:37 GMT  
		Size: 61.9 MB (61923823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd1ce88bdc432038d79dd84d69431425262cc943d0e4cda611b692419932f00`  
		Last Modified: Mon, 14 Sep 2020 19:05:24 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; s390x

```console
$ docker pull ghost@sha256:03a09517228c74619fed24046428e7c3ecb404f12bc87eb6068ce01510e2e8f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122384496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a797ee589ad67d66362078e54bfd7c002c55e6583426382648a72e1a9c17d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:10:43 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 17:50:56 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 17:51:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 17:51:13 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 17:51:25 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 17:51:26 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 17:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 17:51:26 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:36:37 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 19:36:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 19:36:51 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:36:51 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:37:04 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:37:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:37:06 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:37:06 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:38:32 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:38:39 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:38:39 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:38:39 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 19:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:38:40 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:38:40 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:07e4a6dbced6eed74bdb331987f95c00aa5b46543570b7adc1575121e66102dd`  
		Last Modified: Wed, 09 Sep 2020 23:46:28 GMT  
		Size: 25.7 MB (25707597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec3495602424cadce69a424a315984a2e6603ded6694750f985049e7c6ab8b`  
		Last Modified: Thu, 10 Sep 2020 04:15:31 GMT  
		Size: 4.2 KB (4188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee3ec1fd24f74db16ae74a8a3189b86561a6500aaea99e25468b6d748e7c7ab`  
		Last Modified: Wed, 16 Sep 2020 19:17:31 GMT  
		Size: 24.3 MB (24271779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5d1a6a5266fa2ef8e3763a64b68a59ff1e4a6b4921b8521da5ad07ebf6d61c`  
		Last Modified: Wed, 16 Sep 2020 19:17:28 GMT  
		Size: 2.8 MB (2755254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2905d72e8d92f0114522962e97a219b0d41082a7eae3a2dacef776d2b48f2dd0`  
		Last Modified: Wed, 16 Sep 2020 19:17:28 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d094b09c7cb53b45ff04a89d0168ed318bb884944223e795c0670fb352b76a`  
		Last Modified: Wed, 16 Sep 2020 19:45:59 GMT  
		Size: 1.4 MB (1404406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d59fb06dd84473030c140a8c18f31aaef2d9d0d4c442df3e0dea6f9e7a016e`  
		Last Modified: Wed, 16 Sep 2020 19:46:00 GMT  
		Size: 7.3 MB (7299815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f7cc2030cb0a6f224679b784f129c661905818de9bcbd017663d96b3728cd6`  
		Last Modified: Wed, 16 Sep 2020 19:46:10 GMT  
		Size: 60.9 MB (60940627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705c480e33032e8ba81e07d90b91d0f229d9eddcfee4977e2fb11e574ea09513`  
		Last Modified: Wed, 16 Sep 2020 19:45:58 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
