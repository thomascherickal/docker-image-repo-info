<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ghost`

-	[`ghost:2`](#ghost2)
-	[`ghost:2.38`](#ghost238)
-	[`ghost:2.38.2`](#ghost2382)
-	[`ghost:2.38.2-alpine`](#ghost2382-alpine)
-	[`ghost:2.38-alpine`](#ghost238-alpine)
-	[`ghost:2-alpine`](#ghost2-alpine)
-	[`ghost:3`](#ghost3)
-	[`ghost:3.33`](#ghost333)
-	[`ghost:3.33.0`](#ghost3330)
-	[`ghost:3.33.0-alpine`](#ghost3330-alpine)
-	[`ghost:3.33-alpine`](#ghost333-alpine)
-	[`ghost:3-alpine`](#ghost3-alpine)
-	[`ghost:alpine`](#ghostalpine)
-	[`ghost:latest`](#ghostlatest)

## `ghost:2`

```console
$ docker pull ghost@sha256:5510ca8f51dfb031e558a634d8ab875d5bb9ec1e5758e3f353e3118da9b52876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:2` - linux; amd64

```console
$ docker pull ghost@sha256:e21c94361d1906de03a2fc84b964a970f08d3828acc683d0c4624cc031f6e961
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131810323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b84dded01dbf6c5aafeba8ec817a08ac93e849cda3fb6cb64d2c7d1e50cb54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 12:38:47 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 15:26:28 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 15:26:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 15:26:43 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:26:54 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 15:26:55 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:26:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:26:55 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:35:25 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 18:35:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 18:35:43 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:35:44 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:36:15 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:36:15 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:36:16 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:36:16 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 18:38:03 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:38:05 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:38:05 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:38:06 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 18:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:38:07 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:38:07 GMT
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
	-	`sha256:d529751e49be97e599d849a351043398bf1d257c3625b0e3b895f321d0371166`  
		Last Modified: Wed, 16 Sep 2020 15:33:18 GMT  
		Size: 22.0 MB (22037978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4e747e0ab9e71dca2a7d5c1dbbce2f1d28dd2818cfbf7392ee88b0d51f2f0f`  
		Last Modified: Wed, 16 Sep 2020 15:33:12 GMT  
		Size: 2.9 MB (2857346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc64762bc9464da84b7a073e993e62943cdbc61679f37e185c8f6c12e09f696`  
		Last Modified: Wed, 16 Sep 2020 15:33:11 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4ab005747f1432ccad6b27ffa30a4e43953d531c46e0cacf10e24e73dbbe12`  
		Last Modified: Wed, 16 Sep 2020 18:42:18 GMT  
		Size: 1.4 MB (1417660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7479016d2e9f0df246eeff28a04c366a717737e895b5bb272c193c30abb6c81c`  
		Last Modified: Wed, 16 Sep 2020 18:42:23 GMT  
		Size: 7.3 MB (7300343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb4279712d5884494db75d51f9513e2345f7b3be5f80027cd8d607d2c85738f`  
		Last Modified: Wed, 16 Sep 2020 18:42:39 GMT  
		Size: 71.1 MB (71099850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a22bdb171fd112fa97701258601b09808adc7465ba9a9213e469b777882ac8`  
		Last Modified: Wed, 16 Sep 2020 18:42:17 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2` - linux; arm variant v7

```console
$ docker pull ghost@sha256:c046d71236d2b1b51fa92f4857c4d4c15e74e5280a2f0b7ea2e3685f20445583
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127931402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb85adffe94aab1a93d24ab34ac97d1d6843789bf325737b057cbcc40ea710e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 00:08:04 GMT
ADD file:5ec0d2c3043ae64cb72698b0f6fe7387884f4195df962466215ce534d2208327 in / 
# Thu, 10 Sep 2020 00:08:06 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 07:58:25 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 08:15:03 GMT
ENV NODE_VERSION=10.22.0
# Thu, 10 Sep 2020 08:15:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Thu, 10 Sep 2020 08:16:02 GMT
ENV YARN_VERSION=1.22.4
# Thu, 10 Sep 2020 08:16:49 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Thu, 10 Sep 2020 08:16:53 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 08:16:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 08:16:57 GMT
CMD ["node"]
# Fri, 11 Sep 2020 00:56:26 GMT
ENV GOSU_VERSION=1.12
# Fri, 11 Sep 2020 00:56:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Sep 2020 00:56:56 GMT
ENV NODE_ENV=production
# Fri, 11 Sep 2020 00:56:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Fri, 11 Sep 2020 00:57:36 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 11 Sep 2020 00:57:39 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 11 Sep 2020 00:57:40 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 11 Sep 2020 00:57:41 GMT
ENV GHOST_VERSION=2.38.2
# Fri, 11 Sep 2020 01:01:54 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 11 Sep 2020 01:02:01 GMT
WORKDIR /var/lib/ghost
# Fri, 11 Sep 2020 01:02:02 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 11 Sep 2020 01:02:03 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 11 Sep 2020 01:02:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 01:02:06 GMT
EXPOSE 2368
# Fri, 11 Sep 2020 01:02:06 GMT
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
	-	`sha256:f77b07675dea24e6beefdc125c53dafcfe8182ad621c670364224400e98ad71c`  
		Last Modified: Thu, 10 Sep 2020 08:23:39 GMT  
		Size: 20.9 MB (20863015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61df949ba315b0279c334f0ac70057661f92de60045641a2fb57e75f7522e208`  
		Last Modified: Thu, 10 Sep 2020 08:23:31 GMT  
		Size: 2.8 MB (2834349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdbe9c19d9b7af191a2b2cae4886b22311994b1e628beec0de7f395b673a901`  
		Last Modified: Thu, 10 Sep 2020 08:23:30 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2d74c723985e4baf0ab7154e385348bdfdc1dbcfbdfcabfe8d011ffe5a4905`  
		Last Modified: Fri, 11 Sep 2020 01:04:10 GMT  
		Size: 1.4 MB (1369618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca17c15e65690e59c28d258bc77fd85a6456881d09d92d689e37b0b9170b8766`  
		Last Modified: Fri, 11 Sep 2020 01:04:21 GMT  
		Size: 7.3 MB (7300316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee381db822865a5758ffdcd2172326d089095a3a9a293bc9f6c3c1a3848e831`  
		Last Modified: Fri, 11 Sep 2020 01:04:35 GMT  
		Size: 72.9 MB (72859207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9614a757dc009ea977292a55c8c50e56825c42d5be2fe88e1a2164efe734078`  
		Last Modified: Fri, 11 Sep 2020 01:04:09 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:88fcb9ccfd8d2aa24d89ebbf76d036c8c8c0b9ef0291d6f31eeab804dd71c950
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132681459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08fd85529a473e53ebfc623729fc97ec22a578d0056d3e6b080d59eecd5822a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 10:17:51 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 18:11:48 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:12:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 18:12:31 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:13:04 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 18:13:05 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:13:08 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:42:54 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 19:43:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 19:43:16 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:43:17 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:43:55 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:43:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:43:59 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:44:01 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:48:02 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:48:07 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:48:08 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:48:09 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 19:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:48:11 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:48:13 GMT
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
	-	`sha256:e3d6f611df6d3a0506d444fe1ab2a7ef170062674b011db84f79e4927ead05b8`  
		Last Modified: Wed, 16 Sep 2020 18:40:35 GMT  
		Size: 22.1 MB (22131453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22cc8e391d8fda709bb120c0592dbc8cfd0e7f7d0668f65293ab9eb4d29e0f`  
		Last Modified: Wed, 16 Sep 2020 18:40:23 GMT  
		Size: 2.9 MB (2857556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8606dda7c01de19747340e32ffb667e390c9a35aa6794b8f70e4ead27e16ee`  
		Last Modified: Wed, 16 Sep 2020 18:40:21 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc63643be52fb5b4655138ec0b3f1c50d6728ede057732bde22cb961285c9f5`  
		Last Modified: Wed, 16 Sep 2020 19:55:23 GMT  
		Size: 1.4 MB (1353164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089b22f2ff1c695f750756d90ca2d099b9e9d70d88338ac0ee9cb0a2083be05`  
		Last Modified: Wed, 16 Sep 2020 19:55:26 GMT  
		Size: 7.3 MB (7300482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d841ff99c4caea4b1f75c87a6d7ff54ec9990ba5f4770a347f820304d85bd2`  
		Last Modified: Wed, 16 Sep 2020 19:55:44 GMT  
		Size: 73.2 MB (73184458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d9d212bb0aa3e80c643ce542d99cadc5cc6830d65e6eb05b5b524a8b996da0`  
		Last Modified: Wed, 16 Sep 2020 19:55:23 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2` - linux; ppc64le

```console
$ docker pull ghost@sha256:f83efac7baad8a83dbaeeae0090e2c332744d391363d19bb67a9d4c5571a4284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121775371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75e53a57dcee9c3b6221b62f98cb8790f237880a043008e5505300f6d687191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 18:13:32 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 18:39:35 GMT
ENV NODE_VERSION=10.22.0
# Thu, 10 Sep 2020 18:43:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Thu, 10 Sep 2020 18:43:39 GMT
ENV YARN_VERSION=1.22.4
# Thu, 10 Sep 2020 18:46:34 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Thu, 10 Sep 2020 18:46:36 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 18:46:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 18:46:46 GMT
CMD ["node"]
# Fri, 11 Sep 2020 21:27:46 GMT
ENV GOSU_VERSION=1.12
# Fri, 11 Sep 2020 21:30:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Sep 2020 21:30:19 GMT
ENV NODE_ENV=production
# Fri, 11 Sep 2020 21:30:23 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Fri, 11 Sep 2020 21:31:27 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 11 Sep 2020 21:31:33 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 11 Sep 2020 21:31:36 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 11 Sep 2020 21:31:40 GMT
ENV GHOST_VERSION=2.38.2
# Fri, 11 Sep 2020 21:37:43 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 11 Sep 2020 21:37:56 GMT
WORKDIR /var/lib/ghost
# Fri, 11 Sep 2020 21:38:02 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 11 Sep 2020 21:38:05 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 11 Sep 2020 21:38:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:38:13 GMT
EXPOSE 2368
# Fri, 11 Sep 2020 21:38:17 GMT
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
	-	`sha256:b6ddddc4493ee92c9a9adbbfddbe79bcd304a9b77ff70b6560b1721c7e63009b`  
		Last Modified: Thu, 10 Sep 2020 18:51:54 GMT  
		Size: 21.9 MB (21856794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7334c905eda04b73c0927e34f13af44009f188fe6838279d16ed5a903f3719`  
		Last Modified: Thu, 10 Sep 2020 18:51:48 GMT  
		Size: 2.9 MB (2874839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70efb9aa105513fde1b24abb5b67444b0f52c96488f6d5a88a0abc03ee96f7`  
		Last Modified: Thu, 10 Sep 2020 18:51:47 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa3ee059065cce8a4f33ec30c4a62d046556b0a876bbd8ae16fe6eba75b635a`  
		Last Modified: Fri, 11 Sep 2020 21:40:36 GMT  
		Size: 1.3 MB (1338622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30bb69526c6ea7d982b48f8510bca0a9205d411684d8eda5c70893695e5703b`  
		Last Modified: Fri, 11 Sep 2020 21:40:39 GMT  
		Size: 7.3 MB (7300241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11732869dfcaa0b6ddeb169feb79a2d1f87851c5b3ffc387341f98d5a8f01f5e`  
		Last Modified: Fri, 11 Sep 2020 21:40:49 GMT  
		Size: 57.9 MB (57881956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1947302d2458000b585717170dde3bbb712a8886a9db2bc8fa7b2a63b545225c`  
		Last Modified: Fri, 11 Sep 2020 21:40:34 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2` - linux; s390x

```console
$ docker pull ghost@sha256:533130775007f7a0d81c6d77ff623dc9de8584071b9cac84cff51b1caa525fdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116345296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13886f35064a3ae2b1e5bb38e9bae16b5d46e6b99e5e5142b2863d4805e12a51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:10:43 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 18:41:03 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:41:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 18:41:16 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:41:30 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 18:41:31 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:41:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:41:31 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:41:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 19:41:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 19:41:44 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:41:44 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:41:57 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:41:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:41:58 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:41:59 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:43:14 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:43:18 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:43:18 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:43:18 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 19:43:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:43:19 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:43:19 GMT
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
	-	`sha256:f9d2688f7bfe05ca0166f21f892895752ffb418501fb4282fce7d58d586db235`  
		Last Modified: Wed, 16 Sep 2020 19:18:34 GMT  
		Size: 22.1 MB (22143387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9922d94f1fd891d09b4bad06acddfb642ce0eff2a4d55b4d5959c27d9304a849`  
		Last Modified: Wed, 16 Sep 2020 19:18:31 GMT  
		Size: 2.9 MB (2853285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67077e806a4ba7edf833b5a660dbce37e12afabdd221330b1b3b3d1227867642`  
		Last Modified: Wed, 16 Sep 2020 19:18:31 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512184dff9c1dca76fbe614ced0a65e12b28d98110be65fe2572e2a8acb958f3`  
		Last Modified: Wed, 16 Sep 2020 19:46:37 GMT  
		Size: 1.4 MB (1404414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95a5904ad9af77ca64143fa2e8cd1913904930ea75d5d7439247863de2f915a`  
		Last Modified: Wed, 16 Sep 2020 19:46:38 GMT  
		Size: 7.3 MB (7299991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36d6921e27ff10f1739cb06065c2455a7c5e653d1c6a233a821f8efecde48a2`  
		Last Modified: Wed, 16 Sep 2020 19:46:44 GMT  
		Size: 56.9 MB (56931603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fcd04b3a4a41cc7df97c0a4cbb03e0116402aaf0c84b602b0d6b36e95d39f7`  
		Last Modified: Wed, 16 Sep 2020 19:46:36 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:2.38`

```console
$ docker pull ghost@sha256:5510ca8f51dfb031e558a634d8ab875d5bb9ec1e5758e3f353e3118da9b52876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:2.38` - linux; amd64

```console
$ docker pull ghost@sha256:e21c94361d1906de03a2fc84b964a970f08d3828acc683d0c4624cc031f6e961
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131810323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b84dded01dbf6c5aafeba8ec817a08ac93e849cda3fb6cb64d2c7d1e50cb54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 12:38:47 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 15:26:28 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 15:26:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 15:26:43 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:26:54 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 15:26:55 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:26:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:26:55 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:35:25 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 18:35:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 18:35:43 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:35:44 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:36:15 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:36:15 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:36:16 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:36:16 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 18:38:03 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:38:05 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:38:05 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:38:06 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 18:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:38:07 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:38:07 GMT
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
	-	`sha256:d529751e49be97e599d849a351043398bf1d257c3625b0e3b895f321d0371166`  
		Last Modified: Wed, 16 Sep 2020 15:33:18 GMT  
		Size: 22.0 MB (22037978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4e747e0ab9e71dca2a7d5c1dbbce2f1d28dd2818cfbf7392ee88b0d51f2f0f`  
		Last Modified: Wed, 16 Sep 2020 15:33:12 GMT  
		Size: 2.9 MB (2857346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc64762bc9464da84b7a073e993e62943cdbc61679f37e185c8f6c12e09f696`  
		Last Modified: Wed, 16 Sep 2020 15:33:11 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4ab005747f1432ccad6b27ffa30a4e43953d531c46e0cacf10e24e73dbbe12`  
		Last Modified: Wed, 16 Sep 2020 18:42:18 GMT  
		Size: 1.4 MB (1417660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7479016d2e9f0df246eeff28a04c366a717737e895b5bb272c193c30abb6c81c`  
		Last Modified: Wed, 16 Sep 2020 18:42:23 GMT  
		Size: 7.3 MB (7300343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb4279712d5884494db75d51f9513e2345f7b3be5f80027cd8d607d2c85738f`  
		Last Modified: Wed, 16 Sep 2020 18:42:39 GMT  
		Size: 71.1 MB (71099850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a22bdb171fd112fa97701258601b09808adc7465ba9a9213e469b777882ac8`  
		Last Modified: Wed, 16 Sep 2020 18:42:17 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38` - linux; arm variant v7

```console
$ docker pull ghost@sha256:c046d71236d2b1b51fa92f4857c4d4c15e74e5280a2f0b7ea2e3685f20445583
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127931402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb85adffe94aab1a93d24ab34ac97d1d6843789bf325737b057cbcc40ea710e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 00:08:04 GMT
ADD file:5ec0d2c3043ae64cb72698b0f6fe7387884f4195df962466215ce534d2208327 in / 
# Thu, 10 Sep 2020 00:08:06 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 07:58:25 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 08:15:03 GMT
ENV NODE_VERSION=10.22.0
# Thu, 10 Sep 2020 08:15:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Thu, 10 Sep 2020 08:16:02 GMT
ENV YARN_VERSION=1.22.4
# Thu, 10 Sep 2020 08:16:49 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Thu, 10 Sep 2020 08:16:53 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 08:16:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 08:16:57 GMT
CMD ["node"]
# Fri, 11 Sep 2020 00:56:26 GMT
ENV GOSU_VERSION=1.12
# Fri, 11 Sep 2020 00:56:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Sep 2020 00:56:56 GMT
ENV NODE_ENV=production
# Fri, 11 Sep 2020 00:56:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Fri, 11 Sep 2020 00:57:36 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 11 Sep 2020 00:57:39 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 11 Sep 2020 00:57:40 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 11 Sep 2020 00:57:41 GMT
ENV GHOST_VERSION=2.38.2
# Fri, 11 Sep 2020 01:01:54 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 11 Sep 2020 01:02:01 GMT
WORKDIR /var/lib/ghost
# Fri, 11 Sep 2020 01:02:02 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 11 Sep 2020 01:02:03 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 11 Sep 2020 01:02:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 01:02:06 GMT
EXPOSE 2368
# Fri, 11 Sep 2020 01:02:06 GMT
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
	-	`sha256:f77b07675dea24e6beefdc125c53dafcfe8182ad621c670364224400e98ad71c`  
		Last Modified: Thu, 10 Sep 2020 08:23:39 GMT  
		Size: 20.9 MB (20863015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61df949ba315b0279c334f0ac70057661f92de60045641a2fb57e75f7522e208`  
		Last Modified: Thu, 10 Sep 2020 08:23:31 GMT  
		Size: 2.8 MB (2834349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdbe9c19d9b7af191a2b2cae4886b22311994b1e628beec0de7f395b673a901`  
		Last Modified: Thu, 10 Sep 2020 08:23:30 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2d74c723985e4baf0ab7154e385348bdfdc1dbcfbdfcabfe8d011ffe5a4905`  
		Last Modified: Fri, 11 Sep 2020 01:04:10 GMT  
		Size: 1.4 MB (1369618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca17c15e65690e59c28d258bc77fd85a6456881d09d92d689e37b0b9170b8766`  
		Last Modified: Fri, 11 Sep 2020 01:04:21 GMT  
		Size: 7.3 MB (7300316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee381db822865a5758ffdcd2172326d089095a3a9a293bc9f6c3c1a3848e831`  
		Last Modified: Fri, 11 Sep 2020 01:04:35 GMT  
		Size: 72.9 MB (72859207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9614a757dc009ea977292a55c8c50e56825c42d5be2fe88e1a2164efe734078`  
		Last Modified: Fri, 11 Sep 2020 01:04:09 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:88fcb9ccfd8d2aa24d89ebbf76d036c8c8c0b9ef0291d6f31eeab804dd71c950
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132681459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08fd85529a473e53ebfc623729fc97ec22a578d0056d3e6b080d59eecd5822a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 10:17:51 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 18:11:48 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:12:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 18:12:31 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:13:04 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 18:13:05 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:13:08 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:42:54 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 19:43:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 19:43:16 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:43:17 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:43:55 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:43:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:43:59 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:44:01 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:48:02 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:48:07 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:48:08 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:48:09 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 19:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:48:11 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:48:13 GMT
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
	-	`sha256:e3d6f611df6d3a0506d444fe1ab2a7ef170062674b011db84f79e4927ead05b8`  
		Last Modified: Wed, 16 Sep 2020 18:40:35 GMT  
		Size: 22.1 MB (22131453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22cc8e391d8fda709bb120c0592dbc8cfd0e7f7d0668f65293ab9eb4d29e0f`  
		Last Modified: Wed, 16 Sep 2020 18:40:23 GMT  
		Size: 2.9 MB (2857556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8606dda7c01de19747340e32ffb667e390c9a35aa6794b8f70e4ead27e16ee`  
		Last Modified: Wed, 16 Sep 2020 18:40:21 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc63643be52fb5b4655138ec0b3f1c50d6728ede057732bde22cb961285c9f5`  
		Last Modified: Wed, 16 Sep 2020 19:55:23 GMT  
		Size: 1.4 MB (1353164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089b22f2ff1c695f750756d90ca2d099b9e9d70d88338ac0ee9cb0a2083be05`  
		Last Modified: Wed, 16 Sep 2020 19:55:26 GMT  
		Size: 7.3 MB (7300482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d841ff99c4caea4b1f75c87a6d7ff54ec9990ba5f4770a347f820304d85bd2`  
		Last Modified: Wed, 16 Sep 2020 19:55:44 GMT  
		Size: 73.2 MB (73184458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d9d212bb0aa3e80c643ce542d99cadc5cc6830d65e6eb05b5b524a8b996da0`  
		Last Modified: Wed, 16 Sep 2020 19:55:23 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38` - linux; ppc64le

```console
$ docker pull ghost@sha256:f83efac7baad8a83dbaeeae0090e2c332744d391363d19bb67a9d4c5571a4284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121775371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75e53a57dcee9c3b6221b62f98cb8790f237880a043008e5505300f6d687191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 18:13:32 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 18:39:35 GMT
ENV NODE_VERSION=10.22.0
# Thu, 10 Sep 2020 18:43:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Thu, 10 Sep 2020 18:43:39 GMT
ENV YARN_VERSION=1.22.4
# Thu, 10 Sep 2020 18:46:34 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Thu, 10 Sep 2020 18:46:36 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 18:46:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 18:46:46 GMT
CMD ["node"]
# Fri, 11 Sep 2020 21:27:46 GMT
ENV GOSU_VERSION=1.12
# Fri, 11 Sep 2020 21:30:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Sep 2020 21:30:19 GMT
ENV NODE_ENV=production
# Fri, 11 Sep 2020 21:30:23 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Fri, 11 Sep 2020 21:31:27 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 11 Sep 2020 21:31:33 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 11 Sep 2020 21:31:36 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 11 Sep 2020 21:31:40 GMT
ENV GHOST_VERSION=2.38.2
# Fri, 11 Sep 2020 21:37:43 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 11 Sep 2020 21:37:56 GMT
WORKDIR /var/lib/ghost
# Fri, 11 Sep 2020 21:38:02 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 11 Sep 2020 21:38:05 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 11 Sep 2020 21:38:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:38:13 GMT
EXPOSE 2368
# Fri, 11 Sep 2020 21:38:17 GMT
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
	-	`sha256:b6ddddc4493ee92c9a9adbbfddbe79bcd304a9b77ff70b6560b1721c7e63009b`  
		Last Modified: Thu, 10 Sep 2020 18:51:54 GMT  
		Size: 21.9 MB (21856794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7334c905eda04b73c0927e34f13af44009f188fe6838279d16ed5a903f3719`  
		Last Modified: Thu, 10 Sep 2020 18:51:48 GMT  
		Size: 2.9 MB (2874839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70efb9aa105513fde1b24abb5b67444b0f52c96488f6d5a88a0abc03ee96f7`  
		Last Modified: Thu, 10 Sep 2020 18:51:47 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa3ee059065cce8a4f33ec30c4a62d046556b0a876bbd8ae16fe6eba75b635a`  
		Last Modified: Fri, 11 Sep 2020 21:40:36 GMT  
		Size: 1.3 MB (1338622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30bb69526c6ea7d982b48f8510bca0a9205d411684d8eda5c70893695e5703b`  
		Last Modified: Fri, 11 Sep 2020 21:40:39 GMT  
		Size: 7.3 MB (7300241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11732869dfcaa0b6ddeb169feb79a2d1f87851c5b3ffc387341f98d5a8f01f5e`  
		Last Modified: Fri, 11 Sep 2020 21:40:49 GMT  
		Size: 57.9 MB (57881956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1947302d2458000b585717170dde3bbb712a8886a9db2bc8fa7b2a63b545225c`  
		Last Modified: Fri, 11 Sep 2020 21:40:34 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38` - linux; s390x

```console
$ docker pull ghost@sha256:533130775007f7a0d81c6d77ff623dc9de8584071b9cac84cff51b1caa525fdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116345296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13886f35064a3ae2b1e5bb38e9bae16b5d46e6b99e5e5142b2863d4805e12a51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:10:43 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 18:41:03 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:41:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 18:41:16 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:41:30 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 18:41:31 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:41:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:41:31 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:41:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 19:41:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 19:41:44 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:41:44 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:41:57 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:41:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:41:58 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:41:59 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:43:14 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:43:18 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:43:18 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:43:18 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 19:43:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:43:19 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:43:19 GMT
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
	-	`sha256:f9d2688f7bfe05ca0166f21f892895752ffb418501fb4282fce7d58d586db235`  
		Last Modified: Wed, 16 Sep 2020 19:18:34 GMT  
		Size: 22.1 MB (22143387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9922d94f1fd891d09b4bad06acddfb642ce0eff2a4d55b4d5959c27d9304a849`  
		Last Modified: Wed, 16 Sep 2020 19:18:31 GMT  
		Size: 2.9 MB (2853285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67077e806a4ba7edf833b5a660dbce37e12afabdd221330b1b3b3d1227867642`  
		Last Modified: Wed, 16 Sep 2020 19:18:31 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512184dff9c1dca76fbe614ced0a65e12b28d98110be65fe2572e2a8acb958f3`  
		Last Modified: Wed, 16 Sep 2020 19:46:37 GMT  
		Size: 1.4 MB (1404414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95a5904ad9af77ca64143fa2e8cd1913904930ea75d5d7439247863de2f915a`  
		Last Modified: Wed, 16 Sep 2020 19:46:38 GMT  
		Size: 7.3 MB (7299991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36d6921e27ff10f1739cb06065c2455a7c5e653d1c6a233a821f8efecde48a2`  
		Last Modified: Wed, 16 Sep 2020 19:46:44 GMT  
		Size: 56.9 MB (56931603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fcd04b3a4a41cc7df97c0a4cbb03e0116402aaf0c84b602b0d6b36e95d39f7`  
		Last Modified: Wed, 16 Sep 2020 19:46:36 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:2.38.2`

```console
$ docker pull ghost@sha256:5510ca8f51dfb031e558a634d8ab875d5bb9ec1e5758e3f353e3118da9b52876
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:2.38.2` - linux; amd64

```console
$ docker pull ghost@sha256:e21c94361d1906de03a2fc84b964a970f08d3828acc683d0c4624cc031f6e961
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131810323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b84dded01dbf6c5aafeba8ec817a08ac93e849cda3fb6cb64d2c7d1e50cb54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 00:23:29 GMT
ADD file:e7407f2294ad23634565820b9669b18ff2a2ca0212a7ec84b9c89d8550859954 in / 
# Thu, 10 Sep 2020 00:23:30 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 12:38:47 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 15:26:28 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 15:26:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 15:26:43 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:26:54 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 15:26:55 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:26:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:26:55 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:35:25 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 18:35:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 18:35:43 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:35:44 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:36:15 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:36:15 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:36:16 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:36:16 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 18:38:03 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:38:05 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:38:05 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:38:06 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 18:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:38:07 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:38:07 GMT
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
	-	`sha256:d529751e49be97e599d849a351043398bf1d257c3625b0e3b895f321d0371166`  
		Last Modified: Wed, 16 Sep 2020 15:33:18 GMT  
		Size: 22.0 MB (22037978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4e747e0ab9e71dca2a7d5c1dbbce2f1d28dd2818cfbf7392ee88b0d51f2f0f`  
		Last Modified: Wed, 16 Sep 2020 15:33:12 GMT  
		Size: 2.9 MB (2857346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc64762bc9464da84b7a073e993e62943cdbc61679f37e185c8f6c12e09f696`  
		Last Modified: Wed, 16 Sep 2020 15:33:11 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4ab005747f1432ccad6b27ffa30a4e43953d531c46e0cacf10e24e73dbbe12`  
		Last Modified: Wed, 16 Sep 2020 18:42:18 GMT  
		Size: 1.4 MB (1417660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7479016d2e9f0df246eeff28a04c366a717737e895b5bb272c193c30abb6c81c`  
		Last Modified: Wed, 16 Sep 2020 18:42:23 GMT  
		Size: 7.3 MB (7300343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb4279712d5884494db75d51f9513e2345f7b3be5f80027cd8d607d2c85738f`  
		Last Modified: Wed, 16 Sep 2020 18:42:39 GMT  
		Size: 71.1 MB (71099850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a22bdb171fd112fa97701258601b09808adc7465ba9a9213e469b777882ac8`  
		Last Modified: Wed, 16 Sep 2020 18:42:17 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2` - linux; arm variant v7

```console
$ docker pull ghost@sha256:c046d71236d2b1b51fa92f4857c4d4c15e74e5280a2f0b7ea2e3685f20445583
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.9 MB (127931402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb85adffe94aab1a93d24ab34ac97d1d6843789bf325737b057cbcc40ea710e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 00:08:04 GMT
ADD file:5ec0d2c3043ae64cb72698b0f6fe7387884f4195df962466215ce534d2208327 in / 
# Thu, 10 Sep 2020 00:08:06 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 07:58:25 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 08:15:03 GMT
ENV NODE_VERSION=10.22.0
# Thu, 10 Sep 2020 08:15:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Thu, 10 Sep 2020 08:16:02 GMT
ENV YARN_VERSION=1.22.4
# Thu, 10 Sep 2020 08:16:49 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Thu, 10 Sep 2020 08:16:53 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 08:16:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 08:16:57 GMT
CMD ["node"]
# Fri, 11 Sep 2020 00:56:26 GMT
ENV GOSU_VERSION=1.12
# Fri, 11 Sep 2020 00:56:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Sep 2020 00:56:56 GMT
ENV NODE_ENV=production
# Fri, 11 Sep 2020 00:56:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Fri, 11 Sep 2020 00:57:36 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 11 Sep 2020 00:57:39 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 11 Sep 2020 00:57:40 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 11 Sep 2020 00:57:41 GMT
ENV GHOST_VERSION=2.38.2
# Fri, 11 Sep 2020 01:01:54 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 11 Sep 2020 01:02:01 GMT
WORKDIR /var/lib/ghost
# Fri, 11 Sep 2020 01:02:02 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 11 Sep 2020 01:02:03 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 11 Sep 2020 01:02:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 01:02:06 GMT
EXPOSE 2368
# Fri, 11 Sep 2020 01:02:06 GMT
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
	-	`sha256:f77b07675dea24e6beefdc125c53dafcfe8182ad621c670364224400e98ad71c`  
		Last Modified: Thu, 10 Sep 2020 08:23:39 GMT  
		Size: 20.9 MB (20863015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61df949ba315b0279c334f0ac70057661f92de60045641a2fb57e75f7522e208`  
		Last Modified: Thu, 10 Sep 2020 08:23:31 GMT  
		Size: 2.8 MB (2834349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdbe9c19d9b7af191a2b2cae4886b22311994b1e628beec0de7f395b673a901`  
		Last Modified: Thu, 10 Sep 2020 08:23:30 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2d74c723985e4baf0ab7154e385348bdfdc1dbcfbdfcabfe8d011ffe5a4905`  
		Last Modified: Fri, 11 Sep 2020 01:04:10 GMT  
		Size: 1.4 MB (1369618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca17c15e65690e59c28d258bc77fd85a6456881d09d92d689e37b0b9170b8766`  
		Last Modified: Fri, 11 Sep 2020 01:04:21 GMT  
		Size: 7.3 MB (7300316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee381db822865a5758ffdcd2172326d089095a3a9a293bc9f6c3c1a3848e831`  
		Last Modified: Fri, 11 Sep 2020 01:04:35 GMT  
		Size: 72.9 MB (72859207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9614a757dc009ea977292a55c8c50e56825c42d5be2fe88e1a2164efe734078`  
		Last Modified: Fri, 11 Sep 2020 01:04:09 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:88fcb9ccfd8d2aa24d89ebbf76d036c8c8c0b9ef0291d6f31eeab804dd71c950
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132681459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08fd85529a473e53ebfc623729fc97ec22a578d0056d3e6b080d59eecd5822a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:54 GMT
ADD file:d870fb0484ea283840d9cc923c9c3fe36d1bb6b3b5ecfefcce06aa26a22c9414 in / 
# Wed, 09 Sep 2020 23:50:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 10:17:51 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 18:11:48 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:12:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 18:12:31 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:13:04 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 18:13:05 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:13:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:13:08 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:42:54 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 19:43:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 19:43:16 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:43:17 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:43:55 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:43:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:43:59 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:44:01 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:48:02 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:48:07 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:48:08 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:48:09 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 19:48:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:48:11 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:48:13 GMT
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
	-	`sha256:e3d6f611df6d3a0506d444fe1ab2a7ef170062674b011db84f79e4927ead05b8`  
		Last Modified: Wed, 16 Sep 2020 18:40:35 GMT  
		Size: 22.1 MB (22131453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee22cc8e391d8fda709bb120c0592dbc8cfd0e7f7d0668f65293ab9eb4d29e0f`  
		Last Modified: Wed, 16 Sep 2020 18:40:23 GMT  
		Size: 2.9 MB (2857556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8606dda7c01de19747340e32ffb667e390c9a35aa6794b8f70e4ead27e16ee`  
		Last Modified: Wed, 16 Sep 2020 18:40:21 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc63643be52fb5b4655138ec0b3f1c50d6728ede057732bde22cb961285c9f5`  
		Last Modified: Wed, 16 Sep 2020 19:55:23 GMT  
		Size: 1.4 MB (1353164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089b22f2ff1c695f750756d90ca2d099b9e9d70d88338ac0ee9cb0a2083be05`  
		Last Modified: Wed, 16 Sep 2020 19:55:26 GMT  
		Size: 7.3 MB (7300482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d841ff99c4caea4b1f75c87a6d7ff54ec9990ba5f4770a347f820304d85bd2`  
		Last Modified: Wed, 16 Sep 2020 19:55:44 GMT  
		Size: 73.2 MB (73184458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d9d212bb0aa3e80c643ce542d99cadc5cc6830d65e6eb05b5b524a8b996da0`  
		Last Modified: Wed, 16 Sep 2020 19:55:23 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2` - linux; ppc64le

```console
$ docker pull ghost@sha256:f83efac7baad8a83dbaeeae0090e2c332744d391363d19bb67a9d4c5571a4284
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121775371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c75e53a57dcee9c3b6221b62f98cb8790f237880a043008e5505300f6d687191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:11 GMT
ADD file:4dede556abae88027bd22f3166fdbc38778a6fcd686c5ce768c3ca024ab3f9cf in / 
# Thu, 10 Sep 2020 01:06:20 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 18:13:32 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 18:39:35 GMT
ENV NODE_VERSION=10.22.0
# Thu, 10 Sep 2020 18:43:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Thu, 10 Sep 2020 18:43:39 GMT
ENV YARN_VERSION=1.22.4
# Thu, 10 Sep 2020 18:46:34 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Thu, 10 Sep 2020 18:46:36 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 18:46:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 18:46:46 GMT
CMD ["node"]
# Fri, 11 Sep 2020 21:27:46 GMT
ENV GOSU_VERSION=1.12
# Fri, 11 Sep 2020 21:30:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 11 Sep 2020 21:30:19 GMT
ENV NODE_ENV=production
# Fri, 11 Sep 2020 21:30:23 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Fri, 11 Sep 2020 21:31:27 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 11 Sep 2020 21:31:33 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 11 Sep 2020 21:31:36 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 11 Sep 2020 21:31:40 GMT
ENV GHOST_VERSION=2.38.2
# Fri, 11 Sep 2020 21:37:43 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 11 Sep 2020 21:37:56 GMT
WORKDIR /var/lib/ghost
# Fri, 11 Sep 2020 21:38:02 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 11 Sep 2020 21:38:05 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 11 Sep 2020 21:38:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:38:13 GMT
EXPOSE 2368
# Fri, 11 Sep 2020 21:38:17 GMT
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
	-	`sha256:b6ddddc4493ee92c9a9adbbfddbe79bcd304a9b77ff70b6560b1721c7e63009b`  
		Last Modified: Thu, 10 Sep 2020 18:51:54 GMT  
		Size: 21.9 MB (21856794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7334c905eda04b73c0927e34f13af44009f188fe6838279d16ed5a903f3719`  
		Last Modified: Thu, 10 Sep 2020 18:51:48 GMT  
		Size: 2.9 MB (2874839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70efb9aa105513fde1b24abb5b67444b0f52c96488f6d5a88a0abc03ee96f7`  
		Last Modified: Thu, 10 Sep 2020 18:51:47 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa3ee059065cce8a4f33ec30c4a62d046556b0a876bbd8ae16fe6eba75b635a`  
		Last Modified: Fri, 11 Sep 2020 21:40:36 GMT  
		Size: 1.3 MB (1338622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30bb69526c6ea7d982b48f8510bca0a9205d411684d8eda5c70893695e5703b`  
		Last Modified: Fri, 11 Sep 2020 21:40:39 GMT  
		Size: 7.3 MB (7300241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11732869dfcaa0b6ddeb169feb79a2d1f87851c5b3ffc387341f98d5a8f01f5e`  
		Last Modified: Fri, 11 Sep 2020 21:40:49 GMT  
		Size: 57.9 MB (57881956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1947302d2458000b585717170dde3bbb712a8886a9db2bc8fa7b2a63b545225c`  
		Last Modified: Fri, 11 Sep 2020 21:40:34 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2` - linux; s390x

```console
$ docker pull ghost@sha256:533130775007f7a0d81c6d77ff623dc9de8584071b9cac84cff51b1caa525fdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116345296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13886f35064a3ae2b1e5bb38e9bae16b5d46e6b99e5e5142b2863d4805e12a51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:35 GMT
ADD file:65e860d387f18169ea1783465571eaf0946b51c52e560a06759bbc680752f810 in / 
# Wed, 09 Sep 2020 23:42:37 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 04:10:43 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 16 Sep 2020 18:41:03 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:41:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Wed, 16 Sep 2020 18:41:16 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:41:30 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Wed, 16 Sep 2020 18:41:31 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:41:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:41:31 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:41:30 GMT
ENV GOSU_VERSION=1.12
# Wed, 16 Sep 2020 19:41:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 16 Sep 2020 19:41:44 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:41:44 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:41:57 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:41:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:41:58 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:41:59 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:43:14 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends python make gcc g++ libc-dev; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:43:18 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:43:18 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:43:18 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 16 Sep 2020 19:43:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:43:19 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:43:19 GMT
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
	-	`sha256:f9d2688f7bfe05ca0166f21f892895752ffb418501fb4282fce7d58d586db235`  
		Last Modified: Wed, 16 Sep 2020 19:18:34 GMT  
		Size: 22.1 MB (22143387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9922d94f1fd891d09b4bad06acddfb642ce0eff2a4d55b4d5959c27d9304a849`  
		Last Modified: Wed, 16 Sep 2020 19:18:31 GMT  
		Size: 2.9 MB (2853285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67077e806a4ba7edf833b5a660dbce37e12afabdd221330b1b3b3d1227867642`  
		Last Modified: Wed, 16 Sep 2020 19:18:31 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512184dff9c1dca76fbe614ced0a65e12b28d98110be65fe2572e2a8acb958f3`  
		Last Modified: Wed, 16 Sep 2020 19:46:37 GMT  
		Size: 1.4 MB (1404414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95a5904ad9af77ca64143fa2e8cd1913904930ea75d5d7439247863de2f915a`  
		Last Modified: Wed, 16 Sep 2020 19:46:38 GMT  
		Size: 7.3 MB (7299991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36d6921e27ff10f1739cb06065c2455a7c5e653d1c6a233a821f8efecde48a2`  
		Last Modified: Wed, 16 Sep 2020 19:46:44 GMT  
		Size: 56.9 MB (56931603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fcd04b3a4a41cc7df97c0a4cbb03e0116402aaf0c84b602b0d6b36e95d39f7`  
		Last Modified: Wed, 16 Sep 2020 19:46:36 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:2.38.2-alpine`

```console
$ docker pull ghost@sha256:ebd8ad1c773325d9036911b0b0e6f3c35b0eda67a59d118d630d358e0ce5235d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ghost:2.38.2-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:e13a47a9335a89dd60349a2ef254285778bbb13cd24cf27348f3ef4e3a064797
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107770276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98c43285a3975f01f38c5590f68baa44d1664c634db3d1d3dc3617aa20403f44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 15:27:27 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 15:27:32 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 15:27:32 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:27:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 15:27:35 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:27:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:27:35 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:38:14 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:38:16 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:38:16 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:38:17 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:38:47 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:38:48 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:38:48 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:38:48 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 18:40:27 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:40:29 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:40:29 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:40:30 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:40:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:40:30 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:40:31 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338e24a1fcf8d67fef4eabf85cbada0f25fe49d81ccff404312a3c1848d0aed8`  
		Last Modified: Wed, 16 Sep 2020 15:33:54 GMT  
		Size: 22.5 MB (22450934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c2b1f63a506a82234fb7890dece99ace91da6e4b89e3f497b6db7badf85b9a`  
		Last Modified: Wed, 16 Sep 2020 15:33:48 GMT  
		Size: 2.3 MB (2344655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70840f95d8e30211ed5a4ef1005cb515b5436d932f5fe002c5c791536e910b5e`  
		Last Modified: Wed, 16 Sep 2020 15:33:48 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd47901cea0996df6ecd5ecbcde0721c2e7b6b38d42d81943a3670947ffdff3d`  
		Last Modified: Wed, 16 Sep 2020 18:42:45 GMT  
		Size: 9.9 KB (9910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b867e205e06cb774b484ae8bd89acd678b943185936af220bd64d2e5c47ed8f2`  
		Last Modified: Wed, 16 Sep 2020 18:42:46 GMT  
		Size: 780.5 KB (780518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b034d3ae8a9a6323e5a9bebcf981dd495b648d6f3d8d2617c3e1499d2469349f`  
		Last Modified: Wed, 16 Sep 2020 18:42:51 GMT  
		Size: 7.3 MB (7300262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2174fc9807119de24bd4a0d5b8fc7fa0739c4eb7139b594a68693d972686043a`  
		Last Modified: Wed, 16 Sep 2020 18:43:06 GMT  
		Size: 72.1 MB (72069856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c52c98dec1e402b207a3cf15789ddf592d1bee33d3b4873c610f53e7235f7bf`  
		Last Modified: Wed, 16 Sep 2020 18:42:45 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:6c112270308e68d04839ed79b7710473af7bdf11831efc847602d01d00642202
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.8 MB (91790953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394779ac4db1db6d68246244e9c70e501777fdb03dd60e897b6986b3661ccadf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:06:47 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:13:19 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:13:21 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:13:28 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:13:29 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:13:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:13:33 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:41:29 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:41:32 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:41:33 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:41:34 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:42:14 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:42:16 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:42:17 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:42:18 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 18:48:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:48:11 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:48:11 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:48:12 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:48:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:48:13 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:48:14 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e868703658906ef78763cf488359c3dbc326345f292ece29d61e6199614f546`  
		Last Modified: Wed, 16 Sep 2020 18:21:03 GMT  
		Size: 21.9 MB (21857177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d591444f73ec93078045c94f0aeb3a8cafe3e90979493afefda8eb8d776ce2`  
		Last Modified: Wed, 16 Sep 2020 18:20:56 GMT  
		Size: 2.4 MB (2359864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8077bd96ec3dd9e9aeca44357bbb9eff82fbdea00bd78d382572ad9d337c79f5`  
		Last Modified: Wed, 16 Sep 2020 18:20:56 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c04845f10de3aeed40b5566ff2dfb02d0e9dc065b8ca69ceadf9c3e94bcfd5`  
		Last Modified: Wed, 16 Sep 2020 18:49:09 GMT  
		Size: 9.7 KB (9732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1d831020998a971d4fda8b544cd17f8e522bed4d6f00f4de41b6f433220d04`  
		Last Modified: Wed, 16 Sep 2020 18:49:09 GMT  
		Size: 733.5 KB (733455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9bc927203afc8cf7d371b8f67fe13667e98d97a690d15d9f68fe34d391633c`  
		Last Modified: Wed, 16 Sep 2020 18:49:14 GMT  
		Size: 7.3 MB (7300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d752d43c47a1d303db14a8afd0798e489fb4a77b82705e2f75a2099b213d50`  
		Last Modified: Wed, 16 Sep 2020 18:49:32 GMT  
		Size: 56.9 MB (56909572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e020667ff2ddb117285f6c99d4d5ca78c98df04fe0cbf8152040fd9d8fd657f`  
		Last Modified: Wed, 16 Sep 2020 18:49:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:ec90a9d11f0dce9d6f30b1fbbf7b9c878c934f12e4956eaa90daec89cf505f89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90706859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf93ee91cfca63c8e19c06d8999fb9d8af0b9d397740d494188d11827d1ce1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 00:11:46 GMT
ENV NODE_VERSION=10.22.0
# Wed, 22 Jul 2020 00:16:34 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 22 Jul 2020 00:16:38 GMT
ENV YARN_VERSION=1.22.4
# Wed, 22 Jul 2020 00:16:45 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 22 Jul 2020 00:16:46 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 22 Jul 2020 00:16:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:16:47 GMT
CMD ["node"]
# Wed, 22 Jul 2020 00:35:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 22 Jul 2020 00:35:57 GMT
RUN apk add --no-cache 		bash
# Wed, 22 Jul 2020 00:35:58 GMT
ENV NODE_ENV=production
# Wed, 22 Jul 2020 00:35:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 22 Jul 2020 00:36:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 22 Jul 2020 00:36:37 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 22 Jul 2020 00:36:41 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 22 Jul 2020 00:36:42 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 22 Jul 2020 00:41:01 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 22 Jul 2020 00:41:05 GMT
WORKDIR /var/lib/ghost
# Wed, 22 Jul 2020 00:41:06 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 22 Jul 2020 00:41:06 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 22 Jul 2020 00:41:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:41:09 GMT
EXPOSE 2368
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb6df863fb23fac4389fa026bb19f026d46d75a8f0c191f5e5452bc4808b720`  
		Last Modified: Wed, 22 Jul 2020 00:20:52 GMT  
		Size: 21.5 MB (21494222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482c98ca04888db38a14c3607fabb23c108fa5e2806f230a58b41064de4900c4`  
		Last Modified: Wed, 22 Jul 2020 00:20:44 GMT  
		Size: 2.4 MB (2372173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf11bc811e0d45877d108999e88d85c8181d3eab4decadbadb6e25f4f540f33`  
		Last Modified: Wed, 22 Jul 2020 00:20:43 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d35c1f9fff94855dd108a3f6fc11edde744ad2a4330bacc906c5750d3eca5a`  
		Last Modified: Wed, 22 Jul 2020 00:42:07 GMT  
		Size: 9.5 KB (9518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9bcb1dfaf30e6cec261d335e090ef62e3f33ac28ea89a9b93d4f355cc47ef9`  
		Last Modified: Wed, 22 Jul 2020 00:42:07 GMT  
		Size: 669.0 KB (669036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80be43bb09ff3d263092a8391b754d4e28a4a197871912a543c3aade5d179579`  
		Last Modified: Wed, 22 Jul 2020 00:42:12 GMT  
		Size: 7.3 MB (7293566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66cdf72cde4ef8803c0147dea96bfc92f7952caddc787b2a83f4733281e59de`  
		Last Modified: Wed, 22 Jul 2020 00:42:30 GMT  
		Size: 56.4 MB (56445458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bb191e401e98e6b4294e6a34fa15bae14f22a1a98777d45b710167eec8bdf0`  
		Last Modified: Wed, 22 Jul 2020 00:42:07 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:ac75cc01af7115ada345d27915c90ebdf50c149b2ac8349b672c284049c274b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (92964612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4103efca4c7c555094139712d79116c57d65a814be372d5f0544e9b247b3e77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:25:10 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:31:08 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:31:11 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:31:18 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:31:19 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:31:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:31:21 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:48:35 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:48:38 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:48:39 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:48:40 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:49:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:49:07 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:49:08 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:49:09 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:53:31 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:53:34 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:53:35 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:53:36 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:53:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:53:37 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:53:38 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee2c099378c4b936058fb6dfc460a827c36e72931f9e050b7b27325992f4ce7`  
		Last Modified: Wed, 16 Sep 2020 18:41:27 GMT  
		Size: 22.7 MB (22680857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a48b1602124ebb7d2d73fc2c60fb371e19e963fdc351afe70581fbde66b937`  
		Last Modified: Wed, 16 Sep 2020 18:41:21 GMT  
		Size: 2.4 MB (2400009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349061677383cc100f2b2ea95b6410a601ec53ed1f4c8917d4171787a794c8d`  
		Last Modified: Wed, 16 Sep 2020 18:41:20 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c89b0fa9c726d97a0ace1211f3f2a6bf83656c1087dbb1af02c6d9389815cb`  
		Last Modified: Wed, 16 Sep 2020 19:55:53 GMT  
		Size: 9.8 KB (9844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2ace9ee454011ffaa2760c825682a079d27d81799de4cda017d17196f826b5`  
		Last Modified: Wed, 16 Sep 2020 19:55:53 GMT  
		Size: 792.2 KB (792151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092b8de196c753b57b4f84860fa9ca983962271e3bfa62c82087a38047065efa`  
		Last Modified: Wed, 16 Sep 2020 19:55:57 GMT  
		Size: 7.3 MB (7300299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509bb753382efc1dcec10d7c482d6db8b358fc7dc68094f942e640f8dd3ac30b`  
		Last Modified: Wed, 16 Sep 2020 19:56:16 GMT  
		Size: 57.1 MB (57056205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf45b19358d7143d315454444ee5c9ad6672d2189a70c262c8f9793ea85ab42a`  
		Last Modified: Wed, 16 Sep 2020 19:55:54 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2-alpine` - linux; 386

```console
$ docker pull ghost@sha256:3e5603603d2f9895600c2bfe05a94274b1cd05d54e33ea115aefbb63ac72c699
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93105129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd2c212a00fe163815d3d5d46c1b1323133bc2b5b3464afab1563f3098158b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:31:39 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 19:05:38 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 19:05:38 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 19:05:41 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 19:05:41 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 19:05:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:05:42 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:19:22 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:19:23 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:19:23 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:19:23 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:19:43 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:19:43 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:19:44 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:19:44 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:22:49 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:22:50 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:22:51 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:22:51 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:22:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:22:51 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:22:51 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15902211d41f7605a5df8cf5df9217a3d96ccfd25e67151cc2b6d3dae6ec1f85`  
		Last Modified: Wed, 16 Sep 2020 19:06:44 GMT  
		Size: 22.7 MB (22654207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5215b865719ad8eb2b52d09ed13c4ab02ad87d485e42314f4eddad8d939d54e`  
		Last Modified: Wed, 16 Sep 2020 19:06:37 GMT  
		Size: 2.4 MB (2359947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d384d817744c421521d189470848adba8cb7eb590ae0b9c19da433878ecabe`  
		Last Modified: Wed, 16 Sep 2020 19:06:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f207c55bb687dd6d2ef7cf98de5219e3c582ca81244652a13eda8d1d8883e2`  
		Last Modified: Wed, 16 Sep 2020 19:23:14 GMT  
		Size: 10.0 KB (9984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f907e8daacc48275108c08c1f1abdf07da117a29d71c6a39453ca5157dbf257`  
		Last Modified: Wed, 16 Sep 2020 19:23:14 GMT  
		Size: 831.1 KB (831119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a71f29740d845f49d7e0e361255da5e9aa80ae32fe24a31a4e61ffcf8c94e2e`  
		Last Modified: Wed, 16 Sep 2020 19:23:19 GMT  
		Size: 7.3 MB (7300208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7812515c7d8b3ebe1f59101f409e453f0665fa3d55054f3c713105da596445f`  
		Last Modified: Wed, 16 Sep 2020 19:23:32 GMT  
		Size: 57.1 MB (57140421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a218cd79d182ceec18b0c99d33bc2d0f1afb00432725e440d6ac7de0d05236`  
		Last Modified: Wed, 16 Sep 2020 19:23:14 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:40e98ca5934d831ad7c7b96945a2863ff024dc7a6defb0244c8305bee1e56cf5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95784894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a7411aeb32bda5ae6dcb4a5d503d8aaa8739298785cb3382882536f0409042`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 01:20:01 GMT
ENV NODE_VERSION=10.22.0
# Wed, 22 Jul 2020 01:32:51 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 22 Jul 2020 01:32:57 GMT
ENV YARN_VERSION=1.22.4
# Wed, 22 Jul 2020 01:33:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 22 Jul 2020 01:33:16 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 22 Jul 2020 01:33:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 01:33:27 GMT
CMD ["node"]
# Wed, 22 Jul 2020 03:49:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 22 Jul 2020 03:49:27 GMT
RUN apk add --no-cache 		bash
# Wed, 22 Jul 2020 03:49:33 GMT
ENV NODE_ENV=production
# Wed, 22 Jul 2020 03:49:38 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 22 Jul 2020 03:50:53 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 22 Jul 2020 03:51:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 22 Jul 2020 03:51:09 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 22 Jul 2020 03:51:14 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 22 Jul 2020 03:55:38 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 22 Jul 2020 03:55:56 GMT
WORKDIR /var/lib/ghost
# Wed, 22 Jul 2020 03:56:00 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 22 Jul 2020 03:56:02 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 22 Jul 2020 03:56:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 03:56:14 GMT
EXPOSE 2368
# Wed, 22 Jul 2020 03:56:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc954aa2c027c77dea23be4fef3a9b5970847052c9110ca9e17e91ec3715150`  
		Last Modified: Wed, 22 Jul 2020 01:39:44 GMT  
		Size: 24.4 MB (24440216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc839a4ac8595a10c2ab83c33ec98009cad7f69a1cd9e8c7fbafc3c0501e780`  
		Last Modified: Wed, 22 Jul 2020 01:39:37 GMT  
		Size: 2.4 MB (2412465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1a09d80bcc9197e18422aee9e7108a18329435a95f44bd644f22fc65b61da7`  
		Last Modified: Wed, 22 Jul 2020 01:39:37 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ac42d144af8739e59624a406b404f66b0d4fe6c23ea789f2ce4c23b9f30369`  
		Last Modified: Wed, 22 Jul 2020 04:07:21 GMT  
		Size: 10.4 KB (10404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb3f5b63942c6126766138593038dcbbd32f3496846ef8c453214bd2ae14dc3`  
		Last Modified: Wed, 22 Jul 2020 04:07:21 GMT  
		Size: 862.6 KB (862614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba576c51d9dbbab92f484a50fc956e0268ba1ed12a4d4dbfa47830c7e3fc7795`  
		Last Modified: Wed, 22 Jul 2020 04:08:48 GMT  
		Size: 7.3 MB (7293630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea1a385b6425771a72054947acfe8a696f8f01e9bdab585faaa4ffd55f77a4b`  
		Last Modified: Wed, 22 Jul 2020 04:10:57 GMT  
		Size: 57.9 MB (57942894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8697f445baa55f1212d888b91a9cff74ff52ff11ee1b92e266347f9d1a8b74`  
		Last Modified: Wed, 22 Jul 2020 04:07:20 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38.2-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:fd83a23acb8efca12888c3947722edcfe744916600ac9355dcda55ee5aedcf8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92539300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11a94ad4b560ce2d683bc1fcdf3c360a1f926c23a5315ce5098f702dd8d31df5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 19:04:10 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 19:15:31 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 19:15:32 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 19:15:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 19:15:35 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 19:15:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:15:35 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:43:34 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:43:35 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:43:35 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:43:35 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:43:48 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:43:50 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:43:50 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:43:50 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:45:33 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:45:40 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:45:40 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:45:40 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:45:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:45:41 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:45:41 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ec6fe451b18fae47acacdf413b462eef19a808e610b6d0b2da9d6092ca441`  
		Last Modified: Wed, 16 Sep 2020 19:19:17 GMT  
		Size: 22.5 MB (22472216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edacb793d987e7222bd954be02f101ed0e510c7979d4c663bb117a36bcaf37a`  
		Last Modified: Wed, 16 Sep 2020 19:19:14 GMT  
		Size: 2.4 MB (2395691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9176a4389a323c7d021fcc67b3e8405c0e71662733ae2d6dd8dd97953060a1b`  
		Last Modified: Wed, 16 Sep 2020 19:19:22 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095bdea0bea9c528513647a25aa79fe39531ed5b20aa67a2e9fc8f83455feb6`  
		Last Modified: Wed, 16 Sep 2020 19:46:51 GMT  
		Size: 10.0 KB (10003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f08099b7c8eeffe922b4d35523df77ad80a26f382cd379004d534ea3c786b83`  
		Last Modified: Wed, 16 Sep 2020 19:46:51 GMT  
		Size: 813.9 KB (813883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d031decd4330d44952ef4d4079a9058b1799e00a112c5eb7f5638e3c650c7f86`  
		Last Modified: Wed, 16 Sep 2020 19:46:53 GMT  
		Size: 7.3 MB (7299944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a8a1b5fac6d1da1f57e21ae989d1ec1d5dec7414870db8314429dec3ecab03`  
		Last Modified: Wed, 16 Sep 2020 19:46:59 GMT  
		Size: 57.0 MB (56963878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a957831e162967c4598e0e95ed83e9d927ee6d9eadca4fc65fabfacde8d5bbb0`  
		Last Modified: Wed, 16 Sep 2020 19:46:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:2.38-alpine`

```console
$ docker pull ghost@sha256:ebd8ad1c773325d9036911b0b0e6f3c35b0eda67a59d118d630d358e0ce5235d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ghost:2.38-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:e13a47a9335a89dd60349a2ef254285778bbb13cd24cf27348f3ef4e3a064797
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107770276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98c43285a3975f01f38c5590f68baa44d1664c634db3d1d3dc3617aa20403f44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 15:27:27 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 15:27:32 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 15:27:32 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:27:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 15:27:35 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:27:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:27:35 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:38:14 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:38:16 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:38:16 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:38:17 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:38:47 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:38:48 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:38:48 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:38:48 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 18:40:27 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:40:29 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:40:29 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:40:30 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:40:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:40:30 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:40:31 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338e24a1fcf8d67fef4eabf85cbada0f25fe49d81ccff404312a3c1848d0aed8`  
		Last Modified: Wed, 16 Sep 2020 15:33:54 GMT  
		Size: 22.5 MB (22450934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c2b1f63a506a82234fb7890dece99ace91da6e4b89e3f497b6db7badf85b9a`  
		Last Modified: Wed, 16 Sep 2020 15:33:48 GMT  
		Size: 2.3 MB (2344655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70840f95d8e30211ed5a4ef1005cb515b5436d932f5fe002c5c791536e910b5e`  
		Last Modified: Wed, 16 Sep 2020 15:33:48 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd47901cea0996df6ecd5ecbcde0721c2e7b6b38d42d81943a3670947ffdff3d`  
		Last Modified: Wed, 16 Sep 2020 18:42:45 GMT  
		Size: 9.9 KB (9910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b867e205e06cb774b484ae8bd89acd678b943185936af220bd64d2e5c47ed8f2`  
		Last Modified: Wed, 16 Sep 2020 18:42:46 GMT  
		Size: 780.5 KB (780518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b034d3ae8a9a6323e5a9bebcf981dd495b648d6f3d8d2617c3e1499d2469349f`  
		Last Modified: Wed, 16 Sep 2020 18:42:51 GMT  
		Size: 7.3 MB (7300262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2174fc9807119de24bd4a0d5b8fc7fa0739c4eb7139b594a68693d972686043a`  
		Last Modified: Wed, 16 Sep 2020 18:43:06 GMT  
		Size: 72.1 MB (72069856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c52c98dec1e402b207a3cf15789ddf592d1bee33d3b4873c610f53e7235f7bf`  
		Last Modified: Wed, 16 Sep 2020 18:42:45 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:6c112270308e68d04839ed79b7710473af7bdf11831efc847602d01d00642202
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.8 MB (91790953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394779ac4db1db6d68246244e9c70e501777fdb03dd60e897b6986b3661ccadf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:06:47 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:13:19 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:13:21 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:13:28 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:13:29 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:13:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:13:33 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:41:29 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:41:32 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:41:33 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:41:34 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:42:14 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:42:16 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:42:17 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:42:18 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 18:48:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:48:11 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:48:11 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:48:12 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:48:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:48:13 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:48:14 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e868703658906ef78763cf488359c3dbc326345f292ece29d61e6199614f546`  
		Last Modified: Wed, 16 Sep 2020 18:21:03 GMT  
		Size: 21.9 MB (21857177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d591444f73ec93078045c94f0aeb3a8cafe3e90979493afefda8eb8d776ce2`  
		Last Modified: Wed, 16 Sep 2020 18:20:56 GMT  
		Size: 2.4 MB (2359864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8077bd96ec3dd9e9aeca44357bbb9eff82fbdea00bd78d382572ad9d337c79f5`  
		Last Modified: Wed, 16 Sep 2020 18:20:56 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c04845f10de3aeed40b5566ff2dfb02d0e9dc065b8ca69ceadf9c3e94bcfd5`  
		Last Modified: Wed, 16 Sep 2020 18:49:09 GMT  
		Size: 9.7 KB (9732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1d831020998a971d4fda8b544cd17f8e522bed4d6f00f4de41b6f433220d04`  
		Last Modified: Wed, 16 Sep 2020 18:49:09 GMT  
		Size: 733.5 KB (733455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9bc927203afc8cf7d371b8f67fe13667e98d97a690d15d9f68fe34d391633c`  
		Last Modified: Wed, 16 Sep 2020 18:49:14 GMT  
		Size: 7.3 MB (7300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d752d43c47a1d303db14a8afd0798e489fb4a77b82705e2f75a2099b213d50`  
		Last Modified: Wed, 16 Sep 2020 18:49:32 GMT  
		Size: 56.9 MB (56909572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e020667ff2ddb117285f6c99d4d5ca78c98df04fe0cbf8152040fd9d8fd657f`  
		Last Modified: Wed, 16 Sep 2020 18:49:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:ec90a9d11f0dce9d6f30b1fbbf7b9c878c934f12e4956eaa90daec89cf505f89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90706859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf93ee91cfca63c8e19c06d8999fb9d8af0b9d397740d494188d11827d1ce1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 00:11:46 GMT
ENV NODE_VERSION=10.22.0
# Wed, 22 Jul 2020 00:16:34 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 22 Jul 2020 00:16:38 GMT
ENV YARN_VERSION=1.22.4
# Wed, 22 Jul 2020 00:16:45 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 22 Jul 2020 00:16:46 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 22 Jul 2020 00:16:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:16:47 GMT
CMD ["node"]
# Wed, 22 Jul 2020 00:35:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 22 Jul 2020 00:35:57 GMT
RUN apk add --no-cache 		bash
# Wed, 22 Jul 2020 00:35:58 GMT
ENV NODE_ENV=production
# Wed, 22 Jul 2020 00:35:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 22 Jul 2020 00:36:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 22 Jul 2020 00:36:37 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 22 Jul 2020 00:36:41 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 22 Jul 2020 00:36:42 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 22 Jul 2020 00:41:01 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 22 Jul 2020 00:41:05 GMT
WORKDIR /var/lib/ghost
# Wed, 22 Jul 2020 00:41:06 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 22 Jul 2020 00:41:06 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 22 Jul 2020 00:41:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:41:09 GMT
EXPOSE 2368
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb6df863fb23fac4389fa026bb19f026d46d75a8f0c191f5e5452bc4808b720`  
		Last Modified: Wed, 22 Jul 2020 00:20:52 GMT  
		Size: 21.5 MB (21494222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482c98ca04888db38a14c3607fabb23c108fa5e2806f230a58b41064de4900c4`  
		Last Modified: Wed, 22 Jul 2020 00:20:44 GMT  
		Size: 2.4 MB (2372173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf11bc811e0d45877d108999e88d85c8181d3eab4decadbadb6e25f4f540f33`  
		Last Modified: Wed, 22 Jul 2020 00:20:43 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d35c1f9fff94855dd108a3f6fc11edde744ad2a4330bacc906c5750d3eca5a`  
		Last Modified: Wed, 22 Jul 2020 00:42:07 GMT  
		Size: 9.5 KB (9518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9bcb1dfaf30e6cec261d335e090ef62e3f33ac28ea89a9b93d4f355cc47ef9`  
		Last Modified: Wed, 22 Jul 2020 00:42:07 GMT  
		Size: 669.0 KB (669036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80be43bb09ff3d263092a8391b754d4e28a4a197871912a543c3aade5d179579`  
		Last Modified: Wed, 22 Jul 2020 00:42:12 GMT  
		Size: 7.3 MB (7293566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66cdf72cde4ef8803c0147dea96bfc92f7952caddc787b2a83f4733281e59de`  
		Last Modified: Wed, 22 Jul 2020 00:42:30 GMT  
		Size: 56.4 MB (56445458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bb191e401e98e6b4294e6a34fa15bae14f22a1a98777d45b710167eec8bdf0`  
		Last Modified: Wed, 22 Jul 2020 00:42:07 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:ac75cc01af7115ada345d27915c90ebdf50c149b2ac8349b672c284049c274b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (92964612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4103efca4c7c555094139712d79116c57d65a814be372d5f0544e9b247b3e77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:25:10 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:31:08 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:31:11 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:31:18 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:31:19 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:31:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:31:21 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:48:35 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:48:38 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:48:39 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:48:40 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:49:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:49:07 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:49:08 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:49:09 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:53:31 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:53:34 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:53:35 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:53:36 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:53:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:53:37 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:53:38 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee2c099378c4b936058fb6dfc460a827c36e72931f9e050b7b27325992f4ce7`  
		Last Modified: Wed, 16 Sep 2020 18:41:27 GMT  
		Size: 22.7 MB (22680857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a48b1602124ebb7d2d73fc2c60fb371e19e963fdc351afe70581fbde66b937`  
		Last Modified: Wed, 16 Sep 2020 18:41:21 GMT  
		Size: 2.4 MB (2400009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349061677383cc100f2b2ea95b6410a601ec53ed1f4c8917d4171787a794c8d`  
		Last Modified: Wed, 16 Sep 2020 18:41:20 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c89b0fa9c726d97a0ace1211f3f2a6bf83656c1087dbb1af02c6d9389815cb`  
		Last Modified: Wed, 16 Sep 2020 19:55:53 GMT  
		Size: 9.8 KB (9844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2ace9ee454011ffaa2760c825682a079d27d81799de4cda017d17196f826b5`  
		Last Modified: Wed, 16 Sep 2020 19:55:53 GMT  
		Size: 792.2 KB (792151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092b8de196c753b57b4f84860fa9ca983962271e3bfa62c82087a38047065efa`  
		Last Modified: Wed, 16 Sep 2020 19:55:57 GMT  
		Size: 7.3 MB (7300299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509bb753382efc1dcec10d7c482d6db8b358fc7dc68094f942e640f8dd3ac30b`  
		Last Modified: Wed, 16 Sep 2020 19:56:16 GMT  
		Size: 57.1 MB (57056205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf45b19358d7143d315454444ee5c9ad6672d2189a70c262c8f9793ea85ab42a`  
		Last Modified: Wed, 16 Sep 2020 19:55:54 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38-alpine` - linux; 386

```console
$ docker pull ghost@sha256:3e5603603d2f9895600c2bfe05a94274b1cd05d54e33ea115aefbb63ac72c699
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93105129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd2c212a00fe163815d3d5d46c1b1323133bc2b5b3464afab1563f3098158b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:31:39 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 19:05:38 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 19:05:38 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 19:05:41 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 19:05:41 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 19:05:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:05:42 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:19:22 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:19:23 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:19:23 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:19:23 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:19:43 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:19:43 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:19:44 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:19:44 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:22:49 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:22:50 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:22:51 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:22:51 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:22:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:22:51 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:22:51 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15902211d41f7605a5df8cf5df9217a3d96ccfd25e67151cc2b6d3dae6ec1f85`  
		Last Modified: Wed, 16 Sep 2020 19:06:44 GMT  
		Size: 22.7 MB (22654207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5215b865719ad8eb2b52d09ed13c4ab02ad87d485e42314f4eddad8d939d54e`  
		Last Modified: Wed, 16 Sep 2020 19:06:37 GMT  
		Size: 2.4 MB (2359947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d384d817744c421521d189470848adba8cb7eb590ae0b9c19da433878ecabe`  
		Last Modified: Wed, 16 Sep 2020 19:06:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f207c55bb687dd6d2ef7cf98de5219e3c582ca81244652a13eda8d1d8883e2`  
		Last Modified: Wed, 16 Sep 2020 19:23:14 GMT  
		Size: 10.0 KB (9984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f907e8daacc48275108c08c1f1abdf07da117a29d71c6a39453ca5157dbf257`  
		Last Modified: Wed, 16 Sep 2020 19:23:14 GMT  
		Size: 831.1 KB (831119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a71f29740d845f49d7e0e361255da5e9aa80ae32fe24a31a4e61ffcf8c94e2e`  
		Last Modified: Wed, 16 Sep 2020 19:23:19 GMT  
		Size: 7.3 MB (7300208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7812515c7d8b3ebe1f59101f409e453f0665fa3d55054f3c713105da596445f`  
		Last Modified: Wed, 16 Sep 2020 19:23:32 GMT  
		Size: 57.1 MB (57140421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a218cd79d182ceec18b0c99d33bc2d0f1afb00432725e440d6ac7de0d05236`  
		Last Modified: Wed, 16 Sep 2020 19:23:14 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:40e98ca5934d831ad7c7b96945a2863ff024dc7a6defb0244c8305bee1e56cf5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95784894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a7411aeb32bda5ae6dcb4a5d503d8aaa8739298785cb3382882536f0409042`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 01:20:01 GMT
ENV NODE_VERSION=10.22.0
# Wed, 22 Jul 2020 01:32:51 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 22 Jul 2020 01:32:57 GMT
ENV YARN_VERSION=1.22.4
# Wed, 22 Jul 2020 01:33:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 22 Jul 2020 01:33:16 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 22 Jul 2020 01:33:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 01:33:27 GMT
CMD ["node"]
# Wed, 22 Jul 2020 03:49:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 22 Jul 2020 03:49:27 GMT
RUN apk add --no-cache 		bash
# Wed, 22 Jul 2020 03:49:33 GMT
ENV NODE_ENV=production
# Wed, 22 Jul 2020 03:49:38 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 22 Jul 2020 03:50:53 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 22 Jul 2020 03:51:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 22 Jul 2020 03:51:09 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 22 Jul 2020 03:51:14 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 22 Jul 2020 03:55:38 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 22 Jul 2020 03:55:56 GMT
WORKDIR /var/lib/ghost
# Wed, 22 Jul 2020 03:56:00 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 22 Jul 2020 03:56:02 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 22 Jul 2020 03:56:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 03:56:14 GMT
EXPOSE 2368
# Wed, 22 Jul 2020 03:56:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc954aa2c027c77dea23be4fef3a9b5970847052c9110ca9e17e91ec3715150`  
		Last Modified: Wed, 22 Jul 2020 01:39:44 GMT  
		Size: 24.4 MB (24440216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc839a4ac8595a10c2ab83c33ec98009cad7f69a1cd9e8c7fbafc3c0501e780`  
		Last Modified: Wed, 22 Jul 2020 01:39:37 GMT  
		Size: 2.4 MB (2412465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1a09d80bcc9197e18422aee9e7108a18329435a95f44bd644f22fc65b61da7`  
		Last Modified: Wed, 22 Jul 2020 01:39:37 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ac42d144af8739e59624a406b404f66b0d4fe6c23ea789f2ce4c23b9f30369`  
		Last Modified: Wed, 22 Jul 2020 04:07:21 GMT  
		Size: 10.4 KB (10404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb3f5b63942c6126766138593038dcbbd32f3496846ef8c453214bd2ae14dc3`  
		Last Modified: Wed, 22 Jul 2020 04:07:21 GMT  
		Size: 862.6 KB (862614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba576c51d9dbbab92f484a50fc956e0268ba1ed12a4d4dbfa47830c7e3fc7795`  
		Last Modified: Wed, 22 Jul 2020 04:08:48 GMT  
		Size: 7.3 MB (7293630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea1a385b6425771a72054947acfe8a696f8f01e9bdab585faaa4ffd55f77a4b`  
		Last Modified: Wed, 22 Jul 2020 04:10:57 GMT  
		Size: 57.9 MB (57942894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8697f445baa55f1212d888b91a9cff74ff52ff11ee1b92e266347f9d1a8b74`  
		Last Modified: Wed, 22 Jul 2020 04:07:20 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2.38-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:fd83a23acb8efca12888c3947722edcfe744916600ac9355dcda55ee5aedcf8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92539300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11a94ad4b560ce2d683bc1fcdf3c360a1f926c23a5315ce5098f702dd8d31df5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 19:04:10 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 19:15:31 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 19:15:32 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 19:15:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 19:15:35 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 19:15:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:15:35 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:43:34 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:43:35 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:43:35 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:43:35 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:43:48 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:43:50 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:43:50 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:43:50 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:45:33 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:45:40 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:45:40 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:45:40 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:45:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:45:41 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:45:41 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ec6fe451b18fae47acacdf413b462eef19a808e610b6d0b2da9d6092ca441`  
		Last Modified: Wed, 16 Sep 2020 19:19:17 GMT  
		Size: 22.5 MB (22472216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edacb793d987e7222bd954be02f101ed0e510c7979d4c663bb117a36bcaf37a`  
		Last Modified: Wed, 16 Sep 2020 19:19:14 GMT  
		Size: 2.4 MB (2395691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9176a4389a323c7d021fcc67b3e8405c0e71662733ae2d6dd8dd97953060a1b`  
		Last Modified: Wed, 16 Sep 2020 19:19:22 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095bdea0bea9c528513647a25aa79fe39531ed5b20aa67a2e9fc8f83455feb6`  
		Last Modified: Wed, 16 Sep 2020 19:46:51 GMT  
		Size: 10.0 KB (10003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f08099b7c8eeffe922b4d35523df77ad80a26f382cd379004d534ea3c786b83`  
		Last Modified: Wed, 16 Sep 2020 19:46:51 GMT  
		Size: 813.9 KB (813883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d031decd4330d44952ef4d4079a9058b1799e00a112c5eb7f5638e3c650c7f86`  
		Last Modified: Wed, 16 Sep 2020 19:46:53 GMT  
		Size: 7.3 MB (7299944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a8a1b5fac6d1da1f57e21ae989d1ec1d5dec7414870db8314429dec3ecab03`  
		Last Modified: Wed, 16 Sep 2020 19:46:59 GMT  
		Size: 57.0 MB (56963878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a957831e162967c4598e0e95ed83e9d927ee6d9eadca4fc65fabfacde8d5bbb0`  
		Last Modified: Wed, 16 Sep 2020 19:46:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:2-alpine`

```console
$ docker pull ghost@sha256:ebd8ad1c773325d9036911b0b0e6f3c35b0eda67a59d118d630d358e0ce5235d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ghost:2-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:e13a47a9335a89dd60349a2ef254285778bbb13cd24cf27348f3ef4e3a064797
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107770276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98c43285a3975f01f38c5590f68baa44d1664c634db3d1d3dc3617aa20403f44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 15:27:27 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 15:27:32 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 15:27:32 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:27:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 15:27:35 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:27:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:27:35 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:38:14 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:38:16 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:38:16 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:38:17 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:38:47 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:38:48 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:38:48 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:38:48 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 18:40:27 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:40:29 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:40:29 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:40:30 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:40:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:40:30 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:40:31 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338e24a1fcf8d67fef4eabf85cbada0f25fe49d81ccff404312a3c1848d0aed8`  
		Last Modified: Wed, 16 Sep 2020 15:33:54 GMT  
		Size: 22.5 MB (22450934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c2b1f63a506a82234fb7890dece99ace91da6e4b89e3f497b6db7badf85b9a`  
		Last Modified: Wed, 16 Sep 2020 15:33:48 GMT  
		Size: 2.3 MB (2344655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70840f95d8e30211ed5a4ef1005cb515b5436d932f5fe002c5c791536e910b5e`  
		Last Modified: Wed, 16 Sep 2020 15:33:48 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd47901cea0996df6ecd5ecbcde0721c2e7b6b38d42d81943a3670947ffdff3d`  
		Last Modified: Wed, 16 Sep 2020 18:42:45 GMT  
		Size: 9.9 KB (9910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b867e205e06cb774b484ae8bd89acd678b943185936af220bd64d2e5c47ed8f2`  
		Last Modified: Wed, 16 Sep 2020 18:42:46 GMT  
		Size: 780.5 KB (780518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b034d3ae8a9a6323e5a9bebcf981dd495b648d6f3d8d2617c3e1499d2469349f`  
		Last Modified: Wed, 16 Sep 2020 18:42:51 GMT  
		Size: 7.3 MB (7300262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2174fc9807119de24bd4a0d5b8fc7fa0739c4eb7139b594a68693d972686043a`  
		Last Modified: Wed, 16 Sep 2020 18:43:06 GMT  
		Size: 72.1 MB (72069856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c52c98dec1e402b207a3cf15789ddf592d1bee33d3b4873c610f53e7235f7bf`  
		Last Modified: Wed, 16 Sep 2020 18:42:45 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:6c112270308e68d04839ed79b7710473af7bdf11831efc847602d01d00642202
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.8 MB (91790953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:394779ac4db1db6d68246244e9c70e501777fdb03dd60e897b6986b3661ccadf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:06:47 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:13:19 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:13:21 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:13:28 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:13:29 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:13:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:13:33 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:41:29 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:41:32 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:41:33 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:41:34 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:42:14 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:42:16 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:42:17 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:42:18 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 18:48:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:48:11 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:48:11 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:48:12 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:48:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:48:13 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:48:14 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e868703658906ef78763cf488359c3dbc326345f292ece29d61e6199614f546`  
		Last Modified: Wed, 16 Sep 2020 18:21:03 GMT  
		Size: 21.9 MB (21857177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d591444f73ec93078045c94f0aeb3a8cafe3e90979493afefda8eb8d776ce2`  
		Last Modified: Wed, 16 Sep 2020 18:20:56 GMT  
		Size: 2.4 MB (2359864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8077bd96ec3dd9e9aeca44357bbb9eff82fbdea00bd78d382572ad9d337c79f5`  
		Last Modified: Wed, 16 Sep 2020 18:20:56 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c04845f10de3aeed40b5566ff2dfb02d0e9dc065b8ca69ceadf9c3e94bcfd5`  
		Last Modified: Wed, 16 Sep 2020 18:49:09 GMT  
		Size: 9.7 KB (9732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1d831020998a971d4fda8b544cd17f8e522bed4d6f00f4de41b6f433220d04`  
		Last Modified: Wed, 16 Sep 2020 18:49:09 GMT  
		Size: 733.5 KB (733455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9bc927203afc8cf7d371b8f67fe13667e98d97a690d15d9f68fe34d391633c`  
		Last Modified: Wed, 16 Sep 2020 18:49:14 GMT  
		Size: 7.3 MB (7300393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d752d43c47a1d303db14a8afd0798e489fb4a77b82705e2f75a2099b213d50`  
		Last Modified: Wed, 16 Sep 2020 18:49:32 GMT  
		Size: 56.9 MB (56909572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e020667ff2ddb117285f6c99d4d5ca78c98df04fe0cbf8152040fd9d8fd657f`  
		Last Modified: Wed, 16 Sep 2020 18:49:09 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:ec90a9d11f0dce9d6f30b1fbbf7b9c878c934f12e4956eaa90daec89cf505f89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90706859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf93ee91cfca63c8e19c06d8999fb9d8af0b9d397740d494188d11827d1ce1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 00:11:46 GMT
ENV NODE_VERSION=10.22.0
# Wed, 22 Jul 2020 00:16:34 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 22 Jul 2020 00:16:38 GMT
ENV YARN_VERSION=1.22.4
# Wed, 22 Jul 2020 00:16:45 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 22 Jul 2020 00:16:46 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 22 Jul 2020 00:16:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:16:47 GMT
CMD ["node"]
# Wed, 22 Jul 2020 00:35:55 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 22 Jul 2020 00:35:57 GMT
RUN apk add --no-cache 		bash
# Wed, 22 Jul 2020 00:35:58 GMT
ENV NODE_ENV=production
# Wed, 22 Jul 2020 00:35:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 22 Jul 2020 00:36:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 22 Jul 2020 00:36:37 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 22 Jul 2020 00:36:41 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 22 Jul 2020 00:36:42 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 22 Jul 2020 00:41:01 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 22 Jul 2020 00:41:05 GMT
WORKDIR /var/lib/ghost
# Wed, 22 Jul 2020 00:41:06 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 22 Jul 2020 00:41:06 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 22 Jul 2020 00:41:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:41:09 GMT
EXPOSE 2368
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb6df863fb23fac4389fa026bb19f026d46d75a8f0c191f5e5452bc4808b720`  
		Last Modified: Wed, 22 Jul 2020 00:20:52 GMT  
		Size: 21.5 MB (21494222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482c98ca04888db38a14c3607fabb23c108fa5e2806f230a58b41064de4900c4`  
		Last Modified: Wed, 22 Jul 2020 00:20:44 GMT  
		Size: 2.4 MB (2372173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf11bc811e0d45877d108999e88d85c8181d3eab4decadbadb6e25f4f540f33`  
		Last Modified: Wed, 22 Jul 2020 00:20:43 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d35c1f9fff94855dd108a3f6fc11edde744ad2a4330bacc906c5750d3eca5a`  
		Last Modified: Wed, 22 Jul 2020 00:42:07 GMT  
		Size: 9.5 KB (9518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9bcb1dfaf30e6cec261d335e090ef62e3f33ac28ea89a9b93d4f355cc47ef9`  
		Last Modified: Wed, 22 Jul 2020 00:42:07 GMT  
		Size: 669.0 KB (669036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80be43bb09ff3d263092a8391b754d4e28a4a197871912a543c3aade5d179579`  
		Last Modified: Wed, 22 Jul 2020 00:42:12 GMT  
		Size: 7.3 MB (7293566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66cdf72cde4ef8803c0147dea96bfc92f7952caddc787b2a83f4733281e59de`  
		Last Modified: Wed, 22 Jul 2020 00:42:30 GMT  
		Size: 56.4 MB (56445458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bb191e401e98e6b4294e6a34fa15bae14f22a1a98777d45b710167eec8bdf0`  
		Last Modified: Wed, 22 Jul 2020 00:42:07 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:ac75cc01af7115ada345d27915c90ebdf50c149b2ac8349b672c284049c274b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (92964612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4103efca4c7c555094139712d79116c57d65a814be372d5f0544e9b247b3e77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:25:10 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 18:31:08 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:31:11 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:31:18 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:31:19 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:31:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:31:21 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:48:35 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:48:38 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:48:39 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:48:40 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:49:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:49:07 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:49:08 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:49:09 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:53:31 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:53:34 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:53:35 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:53:36 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:53:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:53:37 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:53:38 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee2c099378c4b936058fb6dfc460a827c36e72931f9e050b7b27325992f4ce7`  
		Last Modified: Wed, 16 Sep 2020 18:41:27 GMT  
		Size: 22.7 MB (22680857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a48b1602124ebb7d2d73fc2c60fb371e19e963fdc351afe70581fbde66b937`  
		Last Modified: Wed, 16 Sep 2020 18:41:21 GMT  
		Size: 2.4 MB (2400009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349061677383cc100f2b2ea95b6410a601ec53ed1f4c8917d4171787a794c8d`  
		Last Modified: Wed, 16 Sep 2020 18:41:20 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c89b0fa9c726d97a0ace1211f3f2a6bf83656c1087dbb1af02c6d9389815cb`  
		Last Modified: Wed, 16 Sep 2020 19:55:53 GMT  
		Size: 9.8 KB (9844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2ace9ee454011ffaa2760c825682a079d27d81799de4cda017d17196f826b5`  
		Last Modified: Wed, 16 Sep 2020 19:55:53 GMT  
		Size: 792.2 KB (792151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092b8de196c753b57b4f84860fa9ca983962271e3bfa62c82087a38047065efa`  
		Last Modified: Wed, 16 Sep 2020 19:55:57 GMT  
		Size: 7.3 MB (7300299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509bb753382efc1dcec10d7c482d6db8b358fc7dc68094f942e640f8dd3ac30b`  
		Last Modified: Wed, 16 Sep 2020 19:56:16 GMT  
		Size: 57.1 MB (57056205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf45b19358d7143d315454444ee5c9ad6672d2189a70c262c8f9793ea85ab42a`  
		Last Modified: Wed, 16 Sep 2020 19:55:54 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; 386

```console
$ docker pull ghost@sha256:3e5603603d2f9895600c2bfe05a94274b1cd05d54e33ea115aefbb63ac72c699
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93105129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd2c212a00fe163815d3d5d46c1b1323133bc2b5b3464afab1563f3098158b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:31:39 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 19:05:38 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 19:05:38 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 19:05:41 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 19:05:41 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 19:05:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:05:42 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:19:22 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:19:23 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:19:23 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:19:23 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:19:43 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:19:43 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:19:44 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:19:44 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:22:49 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:22:50 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:22:51 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:22:51 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:22:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:22:51 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:22:51 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15902211d41f7605a5df8cf5df9217a3d96ccfd25e67151cc2b6d3dae6ec1f85`  
		Last Modified: Wed, 16 Sep 2020 19:06:44 GMT  
		Size: 22.7 MB (22654207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5215b865719ad8eb2b52d09ed13c4ab02ad87d485e42314f4eddad8d939d54e`  
		Last Modified: Wed, 16 Sep 2020 19:06:37 GMT  
		Size: 2.4 MB (2359947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d384d817744c421521d189470848adba8cb7eb590ae0b9c19da433878ecabe`  
		Last Modified: Wed, 16 Sep 2020 19:06:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f207c55bb687dd6d2ef7cf98de5219e3c582ca81244652a13eda8d1d8883e2`  
		Last Modified: Wed, 16 Sep 2020 19:23:14 GMT  
		Size: 10.0 KB (9984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f907e8daacc48275108c08c1f1abdf07da117a29d71c6a39453ca5157dbf257`  
		Last Modified: Wed, 16 Sep 2020 19:23:14 GMT  
		Size: 831.1 KB (831119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a71f29740d845f49d7e0e361255da5e9aa80ae32fe24a31a4e61ffcf8c94e2e`  
		Last Modified: Wed, 16 Sep 2020 19:23:19 GMT  
		Size: 7.3 MB (7300208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7812515c7d8b3ebe1f59101f409e453f0665fa3d55054f3c713105da596445f`  
		Last Modified: Wed, 16 Sep 2020 19:23:32 GMT  
		Size: 57.1 MB (57140421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a218cd79d182ceec18b0c99d33bc2d0f1afb00432725e440d6ac7de0d05236`  
		Last Modified: Wed, 16 Sep 2020 19:23:14 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:40e98ca5934d831ad7c7b96945a2863ff024dc7a6defb0244c8305bee1e56cf5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95784894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4a7411aeb32bda5ae6dcb4a5d503d8aaa8739298785cb3382882536f0409042`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 01:20:01 GMT
ENV NODE_VERSION=10.22.0
# Wed, 22 Jul 2020 01:32:51 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 22 Jul 2020 01:32:57 GMT
ENV YARN_VERSION=1.22.4
# Wed, 22 Jul 2020 01:33:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 22 Jul 2020 01:33:16 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 22 Jul 2020 01:33:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 01:33:27 GMT
CMD ["node"]
# Wed, 22 Jul 2020 03:49:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 22 Jul 2020 03:49:27 GMT
RUN apk add --no-cache 		bash
# Wed, 22 Jul 2020 03:49:33 GMT
ENV NODE_ENV=production
# Wed, 22 Jul 2020 03:49:38 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 22 Jul 2020 03:50:53 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 22 Jul 2020 03:51:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 22 Jul 2020 03:51:09 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 22 Jul 2020 03:51:14 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 22 Jul 2020 03:55:38 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 22 Jul 2020 03:55:56 GMT
WORKDIR /var/lib/ghost
# Wed, 22 Jul 2020 03:56:00 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 22 Jul 2020 03:56:02 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 22 Jul 2020 03:56:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 03:56:14 GMT
EXPOSE 2368
# Wed, 22 Jul 2020 03:56:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc954aa2c027c77dea23be4fef3a9b5970847052c9110ca9e17e91ec3715150`  
		Last Modified: Wed, 22 Jul 2020 01:39:44 GMT  
		Size: 24.4 MB (24440216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc839a4ac8595a10c2ab83c33ec98009cad7f69a1cd9e8c7fbafc3c0501e780`  
		Last Modified: Wed, 22 Jul 2020 01:39:37 GMT  
		Size: 2.4 MB (2412465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1a09d80bcc9197e18422aee9e7108a18329435a95f44bd644f22fc65b61da7`  
		Last Modified: Wed, 22 Jul 2020 01:39:37 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ac42d144af8739e59624a406b404f66b0d4fe6c23ea789f2ce4c23b9f30369`  
		Last Modified: Wed, 22 Jul 2020 04:07:21 GMT  
		Size: 10.4 KB (10404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb3f5b63942c6126766138593038dcbbd32f3496846ef8c453214bd2ae14dc3`  
		Last Modified: Wed, 22 Jul 2020 04:07:21 GMT  
		Size: 862.6 KB (862614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba576c51d9dbbab92f484a50fc956e0268ba1ed12a4d4dbfa47830c7e3fc7795`  
		Last Modified: Wed, 22 Jul 2020 04:08:48 GMT  
		Size: 7.3 MB (7293630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea1a385b6425771a72054947acfe8a696f8f01e9bdab585faaa4ffd55f77a4b`  
		Last Modified: Wed, 22 Jul 2020 04:10:57 GMT  
		Size: 57.9 MB (57942894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8697f445baa55f1212d888b91a9cff74ff52ff11ee1b92e266347f9d1a8b74`  
		Last Modified: Wed, 22 Jul 2020 04:07:20 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:fd83a23acb8efca12888c3947722edcfe744916600ac9355dcda55ee5aedcf8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92539300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11a94ad4b560ce2d683bc1fcdf3c360a1f926c23a5315ce5098f702dd8d31df5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 19:04:10 GMT
ENV NODE_VERSION=10.22.1
# Wed, 16 Sep 2020 19:15:31 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 19:15:32 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 19:15:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 19:15:35 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 19:15:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:15:35 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:43:34 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:43:35 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:43:35 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:43:35 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:43:48 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:43:50 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:43:50 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:43:50 GMT
ENV GHOST_VERSION=2.38.2
# Wed, 16 Sep 2020 19:45:33 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:45:40 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:45:40 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:45:40 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:45:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:45:41 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:45:41 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ec6fe451b18fae47acacdf413b462eef19a808e610b6d0b2da9d6092ca441`  
		Last Modified: Wed, 16 Sep 2020 19:19:17 GMT  
		Size: 22.5 MB (22472216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edacb793d987e7222bd954be02f101ed0e510c7979d4c663bb117a36bcaf37a`  
		Last Modified: Wed, 16 Sep 2020 19:19:14 GMT  
		Size: 2.4 MB (2395691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9176a4389a323c7d021fcc67b3e8405c0e71662733ae2d6dd8dd97953060a1b`  
		Last Modified: Wed, 16 Sep 2020 19:19:22 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095bdea0bea9c528513647a25aa79fe39531ed5b20aa67a2e9fc8f83455feb6`  
		Last Modified: Wed, 16 Sep 2020 19:46:51 GMT  
		Size: 10.0 KB (10003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f08099b7c8eeffe922b4d35523df77ad80a26f382cd379004d534ea3c786b83`  
		Last Modified: Wed, 16 Sep 2020 19:46:51 GMT  
		Size: 813.9 KB (813883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d031decd4330d44952ef4d4079a9058b1799e00a112c5eb7f5638e3c650c7f86`  
		Last Modified: Wed, 16 Sep 2020 19:46:53 GMT  
		Size: 7.3 MB (7299944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a8a1b5fac6d1da1f57e21ae989d1ec1d5dec7414870db8314429dec3ecab03`  
		Last Modified: Wed, 16 Sep 2020 19:46:59 GMT  
		Size: 57.0 MB (56963878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a957831e162967c4598e0e95ed83e9d927ee6d9eadca4fc65fabfacde8d5bbb0`  
		Last Modified: Wed, 16 Sep 2020 19:46:51 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:3`

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

### `ghost:3` - linux; amd64

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

### `ghost:3` - linux; arm variant v7

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

### `ghost:3` - linux; arm64 variant v8

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

### `ghost:3` - linux; ppc64le

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

### `ghost:3` - linux; s390x

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

## `ghost:3.33`

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

### `ghost:3.33` - linux; amd64

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

### `ghost:3.33` - linux; arm variant v7

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

### `ghost:3.33` - linux; arm64 variant v8

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

### `ghost:3.33` - linux; ppc64le

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

### `ghost:3.33` - linux; s390x

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

## `ghost:3.33.0`

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

### `ghost:3.33.0` - linux; amd64

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

### `ghost:3.33.0` - linux; arm variant v7

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

### `ghost:3.33.0` - linux; arm64 variant v8

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

### `ghost:3.33.0` - linux; ppc64le

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

### `ghost:3.33.0` - linux; s390x

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

## `ghost:3.33.0-alpine`

```console
$ docker pull ghost@sha256:9c5c8e9a0585f46ea87be6f2fe6eb8e521ab5fcb9a2c1585d37b8230c0add9a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ghost:3.33.0-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:71422ddf0230e11db21c0c38298a7a57ec9c2bf2ea2f9044303ca25b5f7205a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114617502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40128288ca81dcda5779742757851149b0d7aee322f854b1a65a030d7a49e836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 15:24:55 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 15:25:00 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 15:25:00 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:25:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 15:25:03 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:25:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:25:03 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:32:09 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:32:11 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:32:12 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:32:12 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:32:46 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 18:35:05 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:35:08 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:35:08 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:35:09 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:35:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:35:09 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:35:10 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d481011659a13bdb095379d64b4b858612ae1b923da2247c8fc97d52920c72`  
		Last Modified: Wed, 16 Sep 2020 15:32:07 GMT  
		Size: 24.7 MB (24663724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fabc993f172c5fea591f7820f283ca6e238289b3414930dbc808a392f80e9f`  
		Last Modified: Wed, 16 Sep 2020 15:32:01 GMT  
		Size: 2.2 MB (2239084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834ca887ea10ccf5c773b01efa3b1331ba97b7b9fa6fc0c00f8577e96491ab05`  
		Last Modified: Wed, 16 Sep 2020 15:32:00 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad02ebe5fd045290b160178a369c06b5dcac3794f366b205e5322eb55104ec48`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 9.9 KB (9907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac08c3f0139584f5793c0781db31b35c5d858ec8bb3a1dfc10049ac143bf2ed`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 780.5 KB (780521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc087e6a7813bb7d52f69744d4345fb4f8ad65c14136cacc67425cb987a7e0`  
		Last Modified: Wed, 16 Sep 2020 18:41:45 GMT  
		Size: 7.3 MB (7300226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846777c8cbce526597e1ae3c9c3efb82431d2b2bbd9bbe50fa687c396e0d598e`  
		Last Modified: Wed, 16 Sep 2020 18:42:10 GMT  
		Size: 76.8 MB (76809897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ad64533e5521e02c68f5678ce64c996b9d824dd3a049424d43bf62a35f8599`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33.0-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:2f0461412b5a7d20d2b83d981ff288371bc0fe3b55ed276e7471c1ee9e228b4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97918500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80981f34643bb72ee481471e59a59cc4116735ae69e1dd1cc4cf8fc978a54d57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 17:40:49 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 17:52:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 17:52:05 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 17:52:11 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 17:52:12 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 17:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 17:52:13 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:32:16 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:32:19 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:32:20 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:32:20 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:33:04 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:33:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:33:06 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:33:07 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 18:41:13 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:41:17 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:41:18 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:41:19 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:41:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:41:20 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:41:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e605218299f7ebd25e155350c848b92a6f4810477b1083671724070a7aa964`  
		Last Modified: Wed, 16 Sep 2020 18:18:24 GMT  
		Size: 24.0 MB (24041343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13e15a2cc15c85379c3ab92c66be1ca42bab48af072297a6fb6b894b2421375`  
		Last Modified: Wed, 16 Sep 2020 18:18:17 GMT  
		Size: 2.3 MB (2285910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1d335135bbad11f2f7056cd20d0f827f75cc05f21ab4b34db1b1559104816d`  
		Last Modified: Wed, 16 Sep 2020 18:18:16 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c3aea8810324c5d99029432a38ed6d03f5cda6e3b9e882c6c7b61c63e0158a`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 9.7 KB (9730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db17565d2a0e255adb6b10c8202a9a1d1f4d866dc385fc85dec670ca6b4f659`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 733.5 KB (733459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d0c45c43f7049dbfe5986cf9409cadccf8daa91f9459157c988614b7de4a9`  
		Last Modified: Wed, 16 Sep 2020 18:48:33 GMT  
		Size: 7.3 MB (7300584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4e951a483befd38eee02289a488a49411bf6fd6c0d274da1ceace6f0466532`  
		Last Modified: Wed, 16 Sep 2020 18:48:59 GMT  
		Size: 60.9 MB (60926713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0407553e0478012410791ca34224a66b74ddd7f6782d713ad15b2b51f7f6f12`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33.0-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:2ce114fc60a7d6c37b9ad68e569206780f25d0bf9c1d90a3b511ebc308f57ac8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97152917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5de87dfb6964133b28f4841088e7ae8a7d8a9201e1bb7a2304fd3f393ce5dfcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Tue, 28 Jul 2020 23:02:12 GMT
ENV NODE_VERSION=12.18.3
# Tue, 28 Jul 2020 23:11:16 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="14dafe026366e7a9cc8d4737b1fcdcb6c534667e22bbeea63a29a1791ac6ac1f"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 28 Jul 2020 23:11:18 GMT
ENV YARN_VERSION=1.22.4
# Tue, 28 Jul 2020 23:11:24 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 28 Jul 2020 23:11:25 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Jul 2020 23:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jul 2020 23:11:26 GMT
CMD ["node"]
# Tue, 28 Jul 2020 23:42:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 28 Jul 2020 23:42:48 GMT
RUN apk add --no-cache 		bash
# Tue, 28 Jul 2020 23:42:49 GMT
ENV NODE_ENV=production
# Tue, 28 Jul 2020 23:42:50 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Tue, 28 Jul 2020 23:43:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 28 Jul 2020 23:43:25 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 28 Jul 2020 23:43:26 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 21:09:49 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 21:15:11 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 21:15:18 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 21:15:18 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 21:15:19 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 21:15:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 21:15:23 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 21:15:24 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f88341ca4dc0bb7536c1e100534891dc1a168d2c735d3d4a4f658e7aa2c266c`  
		Last Modified: Tue, 28 Jul 2020 23:20:06 GMT  
		Size: 23.6 MB (23598149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5765f8fb68cd71c84db4cb118d2ab3bd6a19013b9240ff2056f7fcfa559bc25c`  
		Last Modified: Tue, 28 Jul 2020 23:19:58 GMT  
		Size: 2.3 MB (2282799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6b46590934f315dfb60ee5b8226e4a8497a770741284fd71d5cd1da891a92a`  
		Last Modified: Tue, 28 Jul 2020 23:19:57 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c6422aa60b4062bf328de58bb22b8a65348f89bfc277d177475ff922a89ab1`  
		Last Modified: Tue, 28 Jul 2020 23:50:07 GMT  
		Size: 9.5 KB (9518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c480bb1a2cab70d156cea495576a482dde69143faad108ee5f628ecb9a22090`  
		Last Modified: Tue, 28 Jul 2020 23:50:07 GMT  
		Size: 669.0 KB (669039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b7a0b1789749d7d72bd946a8c6b5e179bfdf1f71a384787d8fbac65a68051e`  
		Last Modified: Tue, 28 Jul 2020 23:50:12 GMT  
		Size: 7.3 MB (7293372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1ea3a3423a43d694755d781da1619d6fc46212b7609b3e4a85a4b15794df`  
		Last Modified: Mon, 14 Sep 2020 21:17:17 GMT  
		Size: 60.9 MB (60877148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd85b50f3a4d49155beb33fcd84951af378509818299758723d78db1af9ef615`  
		Last Modified: Mon, 14 Sep 2020 21:16:48 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33.0-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:edbfa992b7732a11778ac27801400706e18da3467faf8ceb3a23d14983c832b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98969473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926eaaf8960d968624da1cc7493d138a2cc5c1b2d58dc45d2b564a2bb1801f59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 17:55:53 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 18:06:53 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:06:57 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:07:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:07:18 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:07:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:07:21 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:36:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:36:09 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:36:10 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:36:11 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:36:55 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:36:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:36:58 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:36:59 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:42:20 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:42:28 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:42:30 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:42:31 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:42:33 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:42:34 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cd5d2badbefd21b1a2bfeabb1fdc13a95ce2ec44782c6ecd0b77f3e6941c6`  
		Last Modified: Wed, 16 Sep 2020 18:38:54 GMT  
		Size: 24.8 MB (24756587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375b3dfef9959f5439912c8c672ef9c97530d682060b1482c26d52b5ec9cf53e`  
		Last Modified: Wed, 16 Sep 2020 18:38:46 GMT  
		Size: 2.3 MB (2295913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cf1c388f6776673bed88ff3a465609c960d04f3c890200fe6dfd38809c39`  
		Last Modified: Wed, 16 Sep 2020 18:38:45 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4efecdee57df77fa1df7bc627da0525636ad27b3e917bb2964d740cd7dfc4fc`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 9.8 KB (9846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57353ed8f63a6d635482a86f40236c3e970e0ef7d5e17ea3628dc69e32f26c`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 792.1 KB (792147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2905b594425e7dc51144ae220d8a8383f08191c81d2bb7ca6b3aa4b41de843c0`  
		Last Modified: Wed, 16 Sep 2020 19:54:47 GMT  
		Size: 7.3 MB (7300575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa26c519d4bdf9a2a160800d64aff80745163fd0b989b38570d7a80daed0aef3`  
		Last Modified: Wed, 16 Sep 2020 19:55:11 GMT  
		Size: 61.1 MB (61089153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e78475cfa090323364fa7f0b93245db4a7d6650fb852957aacde045fbe46a40`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33.0-alpine` - linux; 386

```console
$ docker pull ghost@sha256:70af1d6c5bccddf1659593d7ba73f953233a7ce30c2e0128a93d51ac51868456
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99653175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b09e291565fd5cc649a07817b589a1db940bf71e14ec9af3920966de1975136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 04:47:36 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 05:31:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 05:31:04 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 05:31:07 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 05:31:08 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 05:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 05:31:08 GMT
CMD ["node"]
# Wed, 29 Apr 2020 06:19:37 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 06:19:38 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 06:19:38 GMT
ENV NODE_ENV=production
# Wed, 10 Jun 2020 00:16:55 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 10 Jun 2020 00:17:29 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 10 Jun 2020 00:17:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 10 Jun 2020 00:17:30 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 18:38:26 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 18:41:54 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 18:41:55 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 18:41:55 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 18:41:56 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 18:41:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 18:41:56 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 18:41:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a146da8782b0a2b78256aaa25ee92fd617354f694aeace2b3951fab07b027563`  
		Last Modified: Wed, 29 Apr 2020 05:32:18 GMT  
		Size: 24.9 MB (24931595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cb15e48bd1247c878221de413f1942fb7a082c5b789c0b94a025b6e8a0acfe`  
		Last Modified: Wed, 29 Apr 2020 05:32:12 GMT  
		Size: 2.3 MB (2294631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795a10dfdcd143e79354ce37f2fcb9dd923fbc4d3e6281f1be5c8619b654624b`  
		Last Modified: Wed, 29 Apr 2020 05:32:11 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c2188990e50e91234b3066f2b83b08529f15057c14fda8799fdbbedfc33fd3`  
		Last Modified: Wed, 29 Apr 2020 06:23:16 GMT  
		Size: 10.0 KB (9986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987839397957204c0cb5fe48a8aac315882c2895e54e2588a761de6afe65c215`  
		Last Modified: Wed, 29 Apr 2020 06:23:16 GMT  
		Size: 829.5 KB (829504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1630953e291089e0490110657600604529e883f14b3002ddeac8ce34a93c16d7`  
		Last Modified: Wed, 10 Jun 2020 00:27:20 GMT  
		Size: 7.0 MB (7039287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925357b76e685eb00009b4ac955f8512ca5e579d5a042ee1ff3733587033f372`  
		Last Modified: Mon, 14 Sep 2020 18:42:45 GMT  
		Size: 61.7 MB (61738924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081dc2975c2444bf667c099101941a6d056065a0104e0232446cb8967d4c2cd9`  
		Last Modified: Mon, 14 Sep 2020 18:42:22 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33.0-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:43b9d662f9e9433d4830de84a3d8493b526a5df31ac8658e33ae704713ea0574
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102780220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfa0420ce1ad11f6d9a691e6d61f0ea27861e2e77b1cea8219a151cd98cf422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Tue, 28 Jul 2020 23:33:17 GMT
ENV NODE_VERSION=12.18.3
# Tue, 28 Jul 2020 23:51:22 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="14dafe026366e7a9cc8d4737b1fcdcb6c534667e22bbeea63a29a1791ac6ac1f"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 28 Jul 2020 23:51:34 GMT
ENV YARN_VERSION=1.22.4
# Tue, 28 Jul 2020 23:52:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 28 Jul 2020 23:52:39 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Jul 2020 23:52:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jul 2020 23:53:16 GMT
CMD ["node"]
# Wed, 29 Jul 2020 00:58:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Jul 2020 00:59:16 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Jul 2020 00:59:42 GMT
ENV NODE_ENV=production
# Wed, 29 Jul 2020 01:00:10 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 29 Jul 2020 01:02:23 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Jul 2020 01:02:41 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Jul 2020 01:02:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 18:47:52 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 19:02:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 19:03:08 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 19:03:16 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 19:03:20 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 19:03:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 19:03:35 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 19:03:42 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e63182081bd58ba56f2f6a735728ecb0ec58a515e53c2b51cd53a3b4d91267`  
		Last Modified: Wed, 29 Jul 2020 00:10:24 GMT  
		Size: 26.9 MB (26927412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eb37d28bad1d1c3b133e60bdd89387811b5663328c18e29146d8c8b6f11c50`  
		Last Modified: Wed, 29 Jul 2020 00:10:18 GMT  
		Size: 2.3 MB (2290366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79656e9e9a7bfb983771444038c32dbcc5e19fdd81d78f9c0ee464268bc06321`  
		Last Modified: Wed, 29 Jul 2020 00:10:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9114a35fd6126880d15252899fe21b48ba55e1e4c9fa03d888fb9a36d180f6c4`  
		Last Modified: Wed, 29 Jul 2020 01:27:15 GMT  
		Size: 10.4 KB (10403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28565886d5e4396566e6d78ed848e79d95df6b94cce9b93e6b8b4d580d95c20b`  
		Last Modified: Wed, 29 Jul 2020 01:27:24 GMT  
		Size: 862.6 KB (862611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bbd2d0bce62ba7d010e6469f3b646d5d46b6233b91daef6708ced4fc614e69`  
		Last Modified: Wed, 29 Jul 2020 01:28:43 GMT  
		Size: 7.3 MB (7293562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28abb5ff19322ee34b1efb387cc0204aff31935ccefdbc50988a478bd218e11c`  
		Last Modified: Mon, 14 Sep 2020 19:17:23 GMT  
		Size: 62.6 MB (62573194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54949e6aac2cab1e62021ca349d7b78c9a2e6fae68bc081a9f9b96cded0e4e`  
		Last Modified: Mon, 14 Sep 2020 19:11:56 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33.0-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:bd627e9ca1c40e4b19f18229baab850fef538ebeff614f3bbb0c4651e511330b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98684460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30c836dd8e506e4e2d8d7ab3e2d7cc03ca42100103b77a8c2da58883b3033ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:24:02 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 18:40:03 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:40:05 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:40:08 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:40:08 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:40:08 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:38:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:38:58 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:38:58 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:38:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:39:11 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:41:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:41:14 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:41:15 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:41:15 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:41:15 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:41:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e01d2cb5fa863d8474d4a62c71b1f35bcc70df77277e17a98f9231c06d7b035`  
		Last Modified: Wed, 16 Sep 2020 19:18:07 GMT  
		Size: 24.7 MB (24689695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec78b6807a9d38521411c53a6a242f5f37dc57c71daf298d5d3b6cf8f22445`  
		Last Modified: Wed, 16 Sep 2020 19:18:04 GMT  
		Size: 2.3 MB (2298669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3729460d3bf14be267588928707b7f6a9f8f5bfdf695a887a88a2d5a0741389`  
		Last Modified: Wed, 16 Sep 2020 19:18:03 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f02d4953acb0d7df070fb58758486206f2977caf26c5094197832400b84de4a`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 10.0 KB (9999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4248dea411b3dbc103d573a628ca9da62d3aeb14d620db9e8a298d8072272834`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 813.9 KB (813878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c05c149f86a3534ba1fc868d4c24836c5cb669464120d6e1362b45410dc55bc`  
		Last Modified: Wed, 16 Sep 2020 19:46:19 GMT  
		Size: 7.3 MB (7300073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f895c50e263cdc2860e552bd70347d292848576612330c786a126a6d3611907`  
		Last Modified: Wed, 16 Sep 2020 19:46:29 GMT  
		Size: 61.0 MB (60988464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ec89d9d1a434e84ff9a030fb2f07bf5cea8d8a0e36b668da65a06d7028846e`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:3.33-alpine`

```console
$ docker pull ghost@sha256:9c5c8e9a0585f46ea87be6f2fe6eb8e521ab5fcb9a2c1585d37b8230c0add9a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ghost:3.33-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:71422ddf0230e11db21c0c38298a7a57ec9c2bf2ea2f9044303ca25b5f7205a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114617502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40128288ca81dcda5779742757851149b0d7aee322f854b1a65a030d7a49e836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 15:24:55 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 15:25:00 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 15:25:00 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:25:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 15:25:03 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:25:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:25:03 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:32:09 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:32:11 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:32:12 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:32:12 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:32:46 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 18:35:05 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:35:08 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:35:08 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:35:09 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:35:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:35:09 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:35:10 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d481011659a13bdb095379d64b4b858612ae1b923da2247c8fc97d52920c72`  
		Last Modified: Wed, 16 Sep 2020 15:32:07 GMT  
		Size: 24.7 MB (24663724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fabc993f172c5fea591f7820f283ca6e238289b3414930dbc808a392f80e9f`  
		Last Modified: Wed, 16 Sep 2020 15:32:01 GMT  
		Size: 2.2 MB (2239084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834ca887ea10ccf5c773b01efa3b1331ba97b7b9fa6fc0c00f8577e96491ab05`  
		Last Modified: Wed, 16 Sep 2020 15:32:00 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad02ebe5fd045290b160178a369c06b5dcac3794f366b205e5322eb55104ec48`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 9.9 KB (9907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac08c3f0139584f5793c0781db31b35c5d858ec8bb3a1dfc10049ac143bf2ed`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 780.5 KB (780521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc087e6a7813bb7d52f69744d4345fb4f8ad65c14136cacc67425cb987a7e0`  
		Last Modified: Wed, 16 Sep 2020 18:41:45 GMT  
		Size: 7.3 MB (7300226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846777c8cbce526597e1ae3c9c3efb82431d2b2bbd9bbe50fa687c396e0d598e`  
		Last Modified: Wed, 16 Sep 2020 18:42:10 GMT  
		Size: 76.8 MB (76809897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ad64533e5521e02c68f5678ce64c996b9d824dd3a049424d43bf62a35f8599`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:2f0461412b5a7d20d2b83d981ff288371bc0fe3b55ed276e7471c1ee9e228b4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97918500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80981f34643bb72ee481471e59a59cc4116735ae69e1dd1cc4cf8fc978a54d57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 17:40:49 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 17:52:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 17:52:05 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 17:52:11 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 17:52:12 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 17:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 17:52:13 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:32:16 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:32:19 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:32:20 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:32:20 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:33:04 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:33:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:33:06 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:33:07 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 18:41:13 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:41:17 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:41:18 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:41:19 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:41:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:41:20 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:41:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e605218299f7ebd25e155350c848b92a6f4810477b1083671724070a7aa964`  
		Last Modified: Wed, 16 Sep 2020 18:18:24 GMT  
		Size: 24.0 MB (24041343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13e15a2cc15c85379c3ab92c66be1ca42bab48af072297a6fb6b894b2421375`  
		Last Modified: Wed, 16 Sep 2020 18:18:17 GMT  
		Size: 2.3 MB (2285910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1d335135bbad11f2f7056cd20d0f827f75cc05f21ab4b34db1b1559104816d`  
		Last Modified: Wed, 16 Sep 2020 18:18:16 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c3aea8810324c5d99029432a38ed6d03f5cda6e3b9e882c6c7b61c63e0158a`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 9.7 KB (9730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db17565d2a0e255adb6b10c8202a9a1d1f4d866dc385fc85dec670ca6b4f659`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 733.5 KB (733459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d0c45c43f7049dbfe5986cf9409cadccf8daa91f9459157c988614b7de4a9`  
		Last Modified: Wed, 16 Sep 2020 18:48:33 GMT  
		Size: 7.3 MB (7300584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4e951a483befd38eee02289a488a49411bf6fd6c0d274da1ceace6f0466532`  
		Last Modified: Wed, 16 Sep 2020 18:48:59 GMT  
		Size: 60.9 MB (60926713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0407553e0478012410791ca34224a66b74ddd7f6782d713ad15b2b51f7f6f12`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:2ce114fc60a7d6c37b9ad68e569206780f25d0bf9c1d90a3b511ebc308f57ac8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97152917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5de87dfb6964133b28f4841088e7ae8a7d8a9201e1bb7a2304fd3f393ce5dfcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Tue, 28 Jul 2020 23:02:12 GMT
ENV NODE_VERSION=12.18.3
# Tue, 28 Jul 2020 23:11:16 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="14dafe026366e7a9cc8d4737b1fcdcb6c534667e22bbeea63a29a1791ac6ac1f"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 28 Jul 2020 23:11:18 GMT
ENV YARN_VERSION=1.22.4
# Tue, 28 Jul 2020 23:11:24 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 28 Jul 2020 23:11:25 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Jul 2020 23:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jul 2020 23:11:26 GMT
CMD ["node"]
# Tue, 28 Jul 2020 23:42:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 28 Jul 2020 23:42:48 GMT
RUN apk add --no-cache 		bash
# Tue, 28 Jul 2020 23:42:49 GMT
ENV NODE_ENV=production
# Tue, 28 Jul 2020 23:42:50 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Tue, 28 Jul 2020 23:43:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 28 Jul 2020 23:43:25 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 28 Jul 2020 23:43:26 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 21:09:49 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 21:15:11 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 21:15:18 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 21:15:18 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 21:15:19 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 21:15:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 21:15:23 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 21:15:24 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f88341ca4dc0bb7536c1e100534891dc1a168d2c735d3d4a4f658e7aa2c266c`  
		Last Modified: Tue, 28 Jul 2020 23:20:06 GMT  
		Size: 23.6 MB (23598149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5765f8fb68cd71c84db4cb118d2ab3bd6a19013b9240ff2056f7fcfa559bc25c`  
		Last Modified: Tue, 28 Jul 2020 23:19:58 GMT  
		Size: 2.3 MB (2282799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6b46590934f315dfb60ee5b8226e4a8497a770741284fd71d5cd1da891a92a`  
		Last Modified: Tue, 28 Jul 2020 23:19:57 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c6422aa60b4062bf328de58bb22b8a65348f89bfc277d177475ff922a89ab1`  
		Last Modified: Tue, 28 Jul 2020 23:50:07 GMT  
		Size: 9.5 KB (9518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c480bb1a2cab70d156cea495576a482dde69143faad108ee5f628ecb9a22090`  
		Last Modified: Tue, 28 Jul 2020 23:50:07 GMT  
		Size: 669.0 KB (669039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b7a0b1789749d7d72bd946a8c6b5e179bfdf1f71a384787d8fbac65a68051e`  
		Last Modified: Tue, 28 Jul 2020 23:50:12 GMT  
		Size: 7.3 MB (7293372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1ea3a3423a43d694755d781da1619d6fc46212b7609b3e4a85a4b15794df`  
		Last Modified: Mon, 14 Sep 2020 21:17:17 GMT  
		Size: 60.9 MB (60877148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd85b50f3a4d49155beb33fcd84951af378509818299758723d78db1af9ef615`  
		Last Modified: Mon, 14 Sep 2020 21:16:48 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:edbfa992b7732a11778ac27801400706e18da3467faf8ceb3a23d14983c832b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98969473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926eaaf8960d968624da1cc7493d138a2cc5c1b2d58dc45d2b564a2bb1801f59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 17:55:53 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 18:06:53 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:06:57 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:07:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:07:18 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:07:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:07:21 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:36:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:36:09 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:36:10 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:36:11 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:36:55 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:36:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:36:58 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:36:59 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:42:20 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:42:28 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:42:30 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:42:31 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:42:33 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:42:34 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cd5d2badbefd21b1a2bfeabb1fdc13a95ce2ec44782c6ecd0b77f3e6941c6`  
		Last Modified: Wed, 16 Sep 2020 18:38:54 GMT  
		Size: 24.8 MB (24756587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375b3dfef9959f5439912c8c672ef9c97530d682060b1482c26d52b5ec9cf53e`  
		Last Modified: Wed, 16 Sep 2020 18:38:46 GMT  
		Size: 2.3 MB (2295913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cf1c388f6776673bed88ff3a465609c960d04f3c890200fe6dfd38809c39`  
		Last Modified: Wed, 16 Sep 2020 18:38:45 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4efecdee57df77fa1df7bc627da0525636ad27b3e917bb2964d740cd7dfc4fc`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 9.8 KB (9846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57353ed8f63a6d635482a86f40236c3e970e0ef7d5e17ea3628dc69e32f26c`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 792.1 KB (792147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2905b594425e7dc51144ae220d8a8383f08191c81d2bb7ca6b3aa4b41de843c0`  
		Last Modified: Wed, 16 Sep 2020 19:54:47 GMT  
		Size: 7.3 MB (7300575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa26c519d4bdf9a2a160800d64aff80745163fd0b989b38570d7a80daed0aef3`  
		Last Modified: Wed, 16 Sep 2020 19:55:11 GMT  
		Size: 61.1 MB (61089153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e78475cfa090323364fa7f0b93245db4a7d6650fb852957aacde045fbe46a40`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33-alpine` - linux; 386

```console
$ docker pull ghost@sha256:70af1d6c5bccddf1659593d7ba73f953233a7ce30c2e0128a93d51ac51868456
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99653175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b09e291565fd5cc649a07817b589a1db940bf71e14ec9af3920966de1975136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 04:47:36 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 05:31:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 05:31:04 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 05:31:07 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 05:31:08 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 05:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 05:31:08 GMT
CMD ["node"]
# Wed, 29 Apr 2020 06:19:37 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 06:19:38 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 06:19:38 GMT
ENV NODE_ENV=production
# Wed, 10 Jun 2020 00:16:55 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 10 Jun 2020 00:17:29 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 10 Jun 2020 00:17:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 10 Jun 2020 00:17:30 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 18:38:26 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 18:41:54 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 18:41:55 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 18:41:55 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 18:41:56 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 18:41:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 18:41:56 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 18:41:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a146da8782b0a2b78256aaa25ee92fd617354f694aeace2b3951fab07b027563`  
		Last Modified: Wed, 29 Apr 2020 05:32:18 GMT  
		Size: 24.9 MB (24931595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cb15e48bd1247c878221de413f1942fb7a082c5b789c0b94a025b6e8a0acfe`  
		Last Modified: Wed, 29 Apr 2020 05:32:12 GMT  
		Size: 2.3 MB (2294631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795a10dfdcd143e79354ce37f2fcb9dd923fbc4d3e6281f1be5c8619b654624b`  
		Last Modified: Wed, 29 Apr 2020 05:32:11 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c2188990e50e91234b3066f2b83b08529f15057c14fda8799fdbbedfc33fd3`  
		Last Modified: Wed, 29 Apr 2020 06:23:16 GMT  
		Size: 10.0 KB (9986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987839397957204c0cb5fe48a8aac315882c2895e54e2588a761de6afe65c215`  
		Last Modified: Wed, 29 Apr 2020 06:23:16 GMT  
		Size: 829.5 KB (829504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1630953e291089e0490110657600604529e883f14b3002ddeac8ce34a93c16d7`  
		Last Modified: Wed, 10 Jun 2020 00:27:20 GMT  
		Size: 7.0 MB (7039287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925357b76e685eb00009b4ac955f8512ca5e579d5a042ee1ff3733587033f372`  
		Last Modified: Mon, 14 Sep 2020 18:42:45 GMT  
		Size: 61.7 MB (61738924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081dc2975c2444bf667c099101941a6d056065a0104e0232446cb8967d4c2cd9`  
		Last Modified: Mon, 14 Sep 2020 18:42:22 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:43b9d662f9e9433d4830de84a3d8493b526a5df31ac8658e33ae704713ea0574
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102780220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfa0420ce1ad11f6d9a691e6d61f0ea27861e2e77b1cea8219a151cd98cf422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Tue, 28 Jul 2020 23:33:17 GMT
ENV NODE_VERSION=12.18.3
# Tue, 28 Jul 2020 23:51:22 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="14dafe026366e7a9cc8d4737b1fcdcb6c534667e22bbeea63a29a1791ac6ac1f"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 28 Jul 2020 23:51:34 GMT
ENV YARN_VERSION=1.22.4
# Tue, 28 Jul 2020 23:52:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 28 Jul 2020 23:52:39 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Jul 2020 23:52:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jul 2020 23:53:16 GMT
CMD ["node"]
# Wed, 29 Jul 2020 00:58:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Jul 2020 00:59:16 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Jul 2020 00:59:42 GMT
ENV NODE_ENV=production
# Wed, 29 Jul 2020 01:00:10 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 29 Jul 2020 01:02:23 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Jul 2020 01:02:41 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Jul 2020 01:02:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 18:47:52 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 19:02:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 19:03:08 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 19:03:16 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 19:03:20 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 19:03:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 19:03:35 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 19:03:42 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e63182081bd58ba56f2f6a735728ecb0ec58a515e53c2b51cd53a3b4d91267`  
		Last Modified: Wed, 29 Jul 2020 00:10:24 GMT  
		Size: 26.9 MB (26927412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eb37d28bad1d1c3b133e60bdd89387811b5663328c18e29146d8c8b6f11c50`  
		Last Modified: Wed, 29 Jul 2020 00:10:18 GMT  
		Size: 2.3 MB (2290366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79656e9e9a7bfb983771444038c32dbcc5e19fdd81d78f9c0ee464268bc06321`  
		Last Modified: Wed, 29 Jul 2020 00:10:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9114a35fd6126880d15252899fe21b48ba55e1e4c9fa03d888fb9a36d180f6c4`  
		Last Modified: Wed, 29 Jul 2020 01:27:15 GMT  
		Size: 10.4 KB (10403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28565886d5e4396566e6d78ed848e79d95df6b94cce9b93e6b8b4d580d95c20b`  
		Last Modified: Wed, 29 Jul 2020 01:27:24 GMT  
		Size: 862.6 KB (862611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bbd2d0bce62ba7d010e6469f3b646d5d46b6233b91daef6708ced4fc614e69`  
		Last Modified: Wed, 29 Jul 2020 01:28:43 GMT  
		Size: 7.3 MB (7293562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28abb5ff19322ee34b1efb387cc0204aff31935ccefdbc50988a478bd218e11c`  
		Last Modified: Mon, 14 Sep 2020 19:17:23 GMT  
		Size: 62.6 MB (62573194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54949e6aac2cab1e62021ca349d7b78c9a2e6fae68bc081a9f9b96cded0e4e`  
		Last Modified: Mon, 14 Sep 2020 19:11:56 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3.33-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:bd627e9ca1c40e4b19f18229baab850fef538ebeff614f3bbb0c4651e511330b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98684460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30c836dd8e506e4e2d8d7ab3e2d7cc03ca42100103b77a8c2da58883b3033ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:24:02 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 18:40:03 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:40:05 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:40:08 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:40:08 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:40:08 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:38:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:38:58 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:38:58 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:38:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:39:11 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:41:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:41:14 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:41:15 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:41:15 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:41:15 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:41:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e01d2cb5fa863d8474d4a62c71b1f35bcc70df77277e17a98f9231c06d7b035`  
		Last Modified: Wed, 16 Sep 2020 19:18:07 GMT  
		Size: 24.7 MB (24689695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec78b6807a9d38521411c53a6a242f5f37dc57c71daf298d5d3b6cf8f22445`  
		Last Modified: Wed, 16 Sep 2020 19:18:04 GMT  
		Size: 2.3 MB (2298669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3729460d3bf14be267588928707b7f6a9f8f5bfdf695a887a88a2d5a0741389`  
		Last Modified: Wed, 16 Sep 2020 19:18:03 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f02d4953acb0d7df070fb58758486206f2977caf26c5094197832400b84de4a`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 10.0 KB (9999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4248dea411b3dbc103d573a628ca9da62d3aeb14d620db9e8a298d8072272834`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 813.9 KB (813878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c05c149f86a3534ba1fc868d4c24836c5cb669464120d6e1362b45410dc55bc`  
		Last Modified: Wed, 16 Sep 2020 19:46:19 GMT  
		Size: 7.3 MB (7300073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f895c50e263cdc2860e552bd70347d292848576612330c786a126a6d3611907`  
		Last Modified: Wed, 16 Sep 2020 19:46:29 GMT  
		Size: 61.0 MB (60988464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ec89d9d1a434e84ff9a030fb2f07bf5cea8d8a0e36b668da65a06d7028846e`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:3-alpine`

```console
$ docker pull ghost@sha256:9c5c8e9a0585f46ea87be6f2fe6eb8e521ab5fcb9a2c1585d37b8230c0add9a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ghost:3-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:71422ddf0230e11db21c0c38298a7a57ec9c2bf2ea2f9044303ca25b5f7205a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114617502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40128288ca81dcda5779742757851149b0d7aee322f854b1a65a030d7a49e836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 15:24:55 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 15:25:00 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 15:25:00 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:25:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 15:25:03 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:25:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:25:03 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:32:09 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:32:11 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:32:12 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:32:12 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:32:46 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 18:35:05 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:35:08 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:35:08 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:35:09 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:35:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:35:09 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:35:10 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d481011659a13bdb095379d64b4b858612ae1b923da2247c8fc97d52920c72`  
		Last Modified: Wed, 16 Sep 2020 15:32:07 GMT  
		Size: 24.7 MB (24663724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fabc993f172c5fea591f7820f283ca6e238289b3414930dbc808a392f80e9f`  
		Last Modified: Wed, 16 Sep 2020 15:32:01 GMT  
		Size: 2.2 MB (2239084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834ca887ea10ccf5c773b01efa3b1331ba97b7b9fa6fc0c00f8577e96491ab05`  
		Last Modified: Wed, 16 Sep 2020 15:32:00 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad02ebe5fd045290b160178a369c06b5dcac3794f366b205e5322eb55104ec48`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 9.9 KB (9907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac08c3f0139584f5793c0781db31b35c5d858ec8bb3a1dfc10049ac143bf2ed`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 780.5 KB (780521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc087e6a7813bb7d52f69744d4345fb4f8ad65c14136cacc67425cb987a7e0`  
		Last Modified: Wed, 16 Sep 2020 18:41:45 GMT  
		Size: 7.3 MB (7300226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846777c8cbce526597e1ae3c9c3efb82431d2b2bbd9bbe50fa687c396e0d598e`  
		Last Modified: Wed, 16 Sep 2020 18:42:10 GMT  
		Size: 76.8 MB (76809897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ad64533e5521e02c68f5678ce64c996b9d824dd3a049424d43bf62a35f8599`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:2f0461412b5a7d20d2b83d981ff288371bc0fe3b55ed276e7471c1ee9e228b4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97918500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80981f34643bb72ee481471e59a59cc4116735ae69e1dd1cc4cf8fc978a54d57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 17:40:49 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 17:52:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 17:52:05 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 17:52:11 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 17:52:12 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 17:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 17:52:13 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:32:16 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:32:19 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:32:20 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:32:20 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:33:04 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:33:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:33:06 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:33:07 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 18:41:13 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:41:17 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:41:18 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:41:19 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:41:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:41:20 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:41:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e605218299f7ebd25e155350c848b92a6f4810477b1083671724070a7aa964`  
		Last Modified: Wed, 16 Sep 2020 18:18:24 GMT  
		Size: 24.0 MB (24041343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13e15a2cc15c85379c3ab92c66be1ca42bab48af072297a6fb6b894b2421375`  
		Last Modified: Wed, 16 Sep 2020 18:18:17 GMT  
		Size: 2.3 MB (2285910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1d335135bbad11f2f7056cd20d0f827f75cc05f21ab4b34db1b1559104816d`  
		Last Modified: Wed, 16 Sep 2020 18:18:16 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c3aea8810324c5d99029432a38ed6d03f5cda6e3b9e882c6c7b61c63e0158a`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 9.7 KB (9730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db17565d2a0e255adb6b10c8202a9a1d1f4d866dc385fc85dec670ca6b4f659`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 733.5 KB (733459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d0c45c43f7049dbfe5986cf9409cadccf8daa91f9459157c988614b7de4a9`  
		Last Modified: Wed, 16 Sep 2020 18:48:33 GMT  
		Size: 7.3 MB (7300584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4e951a483befd38eee02289a488a49411bf6fd6c0d274da1ceace6f0466532`  
		Last Modified: Wed, 16 Sep 2020 18:48:59 GMT  
		Size: 60.9 MB (60926713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0407553e0478012410791ca34224a66b74ddd7f6782d713ad15b2b51f7f6f12`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:2ce114fc60a7d6c37b9ad68e569206780f25d0bf9c1d90a3b511ebc308f57ac8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97152917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5de87dfb6964133b28f4841088e7ae8a7d8a9201e1bb7a2304fd3f393ce5dfcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Tue, 28 Jul 2020 23:02:12 GMT
ENV NODE_VERSION=12.18.3
# Tue, 28 Jul 2020 23:11:16 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="14dafe026366e7a9cc8d4737b1fcdcb6c534667e22bbeea63a29a1791ac6ac1f"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 28 Jul 2020 23:11:18 GMT
ENV YARN_VERSION=1.22.4
# Tue, 28 Jul 2020 23:11:24 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 28 Jul 2020 23:11:25 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Jul 2020 23:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jul 2020 23:11:26 GMT
CMD ["node"]
# Tue, 28 Jul 2020 23:42:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 28 Jul 2020 23:42:48 GMT
RUN apk add --no-cache 		bash
# Tue, 28 Jul 2020 23:42:49 GMT
ENV NODE_ENV=production
# Tue, 28 Jul 2020 23:42:50 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Tue, 28 Jul 2020 23:43:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 28 Jul 2020 23:43:25 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 28 Jul 2020 23:43:26 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 21:09:49 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 21:15:11 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 21:15:18 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 21:15:18 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 21:15:19 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 21:15:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 21:15:23 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 21:15:24 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f88341ca4dc0bb7536c1e100534891dc1a168d2c735d3d4a4f658e7aa2c266c`  
		Last Modified: Tue, 28 Jul 2020 23:20:06 GMT  
		Size: 23.6 MB (23598149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5765f8fb68cd71c84db4cb118d2ab3bd6a19013b9240ff2056f7fcfa559bc25c`  
		Last Modified: Tue, 28 Jul 2020 23:19:58 GMT  
		Size: 2.3 MB (2282799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6b46590934f315dfb60ee5b8226e4a8497a770741284fd71d5cd1da891a92a`  
		Last Modified: Tue, 28 Jul 2020 23:19:57 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c6422aa60b4062bf328de58bb22b8a65348f89bfc277d177475ff922a89ab1`  
		Last Modified: Tue, 28 Jul 2020 23:50:07 GMT  
		Size: 9.5 KB (9518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c480bb1a2cab70d156cea495576a482dde69143faad108ee5f628ecb9a22090`  
		Last Modified: Tue, 28 Jul 2020 23:50:07 GMT  
		Size: 669.0 KB (669039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b7a0b1789749d7d72bd946a8c6b5e179bfdf1f71a384787d8fbac65a68051e`  
		Last Modified: Tue, 28 Jul 2020 23:50:12 GMT  
		Size: 7.3 MB (7293372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1ea3a3423a43d694755d781da1619d6fc46212b7609b3e4a85a4b15794df`  
		Last Modified: Mon, 14 Sep 2020 21:17:17 GMT  
		Size: 60.9 MB (60877148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd85b50f3a4d49155beb33fcd84951af378509818299758723d78db1af9ef615`  
		Last Modified: Mon, 14 Sep 2020 21:16:48 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:edbfa992b7732a11778ac27801400706e18da3467faf8ceb3a23d14983c832b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98969473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926eaaf8960d968624da1cc7493d138a2cc5c1b2d58dc45d2b564a2bb1801f59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 17:55:53 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 18:06:53 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:06:57 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:07:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:07:18 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:07:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:07:21 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:36:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:36:09 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:36:10 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:36:11 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:36:55 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:36:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:36:58 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:36:59 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:42:20 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:42:28 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:42:30 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:42:31 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:42:33 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:42:34 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cd5d2badbefd21b1a2bfeabb1fdc13a95ce2ec44782c6ecd0b77f3e6941c6`  
		Last Modified: Wed, 16 Sep 2020 18:38:54 GMT  
		Size: 24.8 MB (24756587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375b3dfef9959f5439912c8c672ef9c97530d682060b1482c26d52b5ec9cf53e`  
		Last Modified: Wed, 16 Sep 2020 18:38:46 GMT  
		Size: 2.3 MB (2295913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cf1c388f6776673bed88ff3a465609c960d04f3c890200fe6dfd38809c39`  
		Last Modified: Wed, 16 Sep 2020 18:38:45 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4efecdee57df77fa1df7bc627da0525636ad27b3e917bb2964d740cd7dfc4fc`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 9.8 KB (9846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57353ed8f63a6d635482a86f40236c3e970e0ef7d5e17ea3628dc69e32f26c`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 792.1 KB (792147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2905b594425e7dc51144ae220d8a8383f08191c81d2bb7ca6b3aa4b41de843c0`  
		Last Modified: Wed, 16 Sep 2020 19:54:47 GMT  
		Size: 7.3 MB (7300575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa26c519d4bdf9a2a160800d64aff80745163fd0b989b38570d7a80daed0aef3`  
		Last Modified: Wed, 16 Sep 2020 19:55:11 GMT  
		Size: 61.1 MB (61089153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e78475cfa090323364fa7f0b93245db4a7d6650fb852957aacde045fbe46a40`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; 386

```console
$ docker pull ghost@sha256:70af1d6c5bccddf1659593d7ba73f953233a7ce30c2e0128a93d51ac51868456
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99653175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b09e291565fd5cc649a07817b589a1db940bf71e14ec9af3920966de1975136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 04:47:36 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 05:31:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 05:31:04 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 05:31:07 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 05:31:08 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 05:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 05:31:08 GMT
CMD ["node"]
# Wed, 29 Apr 2020 06:19:37 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 06:19:38 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 06:19:38 GMT
ENV NODE_ENV=production
# Wed, 10 Jun 2020 00:16:55 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 10 Jun 2020 00:17:29 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 10 Jun 2020 00:17:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 10 Jun 2020 00:17:30 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 18:38:26 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 18:41:54 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 18:41:55 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 18:41:55 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 18:41:56 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 18:41:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 18:41:56 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 18:41:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a146da8782b0a2b78256aaa25ee92fd617354f694aeace2b3951fab07b027563`  
		Last Modified: Wed, 29 Apr 2020 05:32:18 GMT  
		Size: 24.9 MB (24931595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cb15e48bd1247c878221de413f1942fb7a082c5b789c0b94a025b6e8a0acfe`  
		Last Modified: Wed, 29 Apr 2020 05:32:12 GMT  
		Size: 2.3 MB (2294631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795a10dfdcd143e79354ce37f2fcb9dd923fbc4d3e6281f1be5c8619b654624b`  
		Last Modified: Wed, 29 Apr 2020 05:32:11 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c2188990e50e91234b3066f2b83b08529f15057c14fda8799fdbbedfc33fd3`  
		Last Modified: Wed, 29 Apr 2020 06:23:16 GMT  
		Size: 10.0 KB (9986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987839397957204c0cb5fe48a8aac315882c2895e54e2588a761de6afe65c215`  
		Last Modified: Wed, 29 Apr 2020 06:23:16 GMT  
		Size: 829.5 KB (829504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1630953e291089e0490110657600604529e883f14b3002ddeac8ce34a93c16d7`  
		Last Modified: Wed, 10 Jun 2020 00:27:20 GMT  
		Size: 7.0 MB (7039287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925357b76e685eb00009b4ac955f8512ca5e579d5a042ee1ff3733587033f372`  
		Last Modified: Mon, 14 Sep 2020 18:42:45 GMT  
		Size: 61.7 MB (61738924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081dc2975c2444bf667c099101941a6d056065a0104e0232446cb8967d4c2cd9`  
		Last Modified: Mon, 14 Sep 2020 18:42:22 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:43b9d662f9e9433d4830de84a3d8493b526a5df31ac8658e33ae704713ea0574
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102780220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfa0420ce1ad11f6d9a691e6d61f0ea27861e2e77b1cea8219a151cd98cf422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Tue, 28 Jul 2020 23:33:17 GMT
ENV NODE_VERSION=12.18.3
# Tue, 28 Jul 2020 23:51:22 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="14dafe026366e7a9cc8d4737b1fcdcb6c534667e22bbeea63a29a1791ac6ac1f"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 28 Jul 2020 23:51:34 GMT
ENV YARN_VERSION=1.22.4
# Tue, 28 Jul 2020 23:52:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 28 Jul 2020 23:52:39 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Jul 2020 23:52:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jul 2020 23:53:16 GMT
CMD ["node"]
# Wed, 29 Jul 2020 00:58:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Jul 2020 00:59:16 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Jul 2020 00:59:42 GMT
ENV NODE_ENV=production
# Wed, 29 Jul 2020 01:00:10 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 29 Jul 2020 01:02:23 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Jul 2020 01:02:41 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Jul 2020 01:02:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 18:47:52 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 19:02:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 19:03:08 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 19:03:16 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 19:03:20 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 19:03:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 19:03:35 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 19:03:42 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e63182081bd58ba56f2f6a735728ecb0ec58a515e53c2b51cd53a3b4d91267`  
		Last Modified: Wed, 29 Jul 2020 00:10:24 GMT  
		Size: 26.9 MB (26927412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eb37d28bad1d1c3b133e60bdd89387811b5663328c18e29146d8c8b6f11c50`  
		Last Modified: Wed, 29 Jul 2020 00:10:18 GMT  
		Size: 2.3 MB (2290366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79656e9e9a7bfb983771444038c32dbcc5e19fdd81d78f9c0ee464268bc06321`  
		Last Modified: Wed, 29 Jul 2020 00:10:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9114a35fd6126880d15252899fe21b48ba55e1e4c9fa03d888fb9a36d180f6c4`  
		Last Modified: Wed, 29 Jul 2020 01:27:15 GMT  
		Size: 10.4 KB (10403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28565886d5e4396566e6d78ed848e79d95df6b94cce9b93e6b8b4d580d95c20b`  
		Last Modified: Wed, 29 Jul 2020 01:27:24 GMT  
		Size: 862.6 KB (862611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bbd2d0bce62ba7d010e6469f3b646d5d46b6233b91daef6708ced4fc614e69`  
		Last Modified: Wed, 29 Jul 2020 01:28:43 GMT  
		Size: 7.3 MB (7293562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28abb5ff19322ee34b1efb387cc0204aff31935ccefdbc50988a478bd218e11c`  
		Last Modified: Mon, 14 Sep 2020 19:17:23 GMT  
		Size: 62.6 MB (62573194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54949e6aac2cab1e62021ca349d7b78c9a2e6fae68bc081a9f9b96cded0e4e`  
		Last Modified: Mon, 14 Sep 2020 19:11:56 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:bd627e9ca1c40e4b19f18229baab850fef538ebeff614f3bbb0c4651e511330b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98684460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30c836dd8e506e4e2d8d7ab3e2d7cc03ca42100103b77a8c2da58883b3033ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:24:02 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 18:40:03 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:40:05 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:40:08 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:40:08 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:40:08 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:38:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:38:58 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:38:58 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:38:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:39:11 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:41:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:41:14 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:41:15 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:41:15 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:41:15 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:41:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e01d2cb5fa863d8474d4a62c71b1f35bcc70df77277e17a98f9231c06d7b035`  
		Last Modified: Wed, 16 Sep 2020 19:18:07 GMT  
		Size: 24.7 MB (24689695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec78b6807a9d38521411c53a6a242f5f37dc57c71daf298d5d3b6cf8f22445`  
		Last Modified: Wed, 16 Sep 2020 19:18:04 GMT  
		Size: 2.3 MB (2298669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3729460d3bf14be267588928707b7f6a9f8f5bfdf695a887a88a2d5a0741389`  
		Last Modified: Wed, 16 Sep 2020 19:18:03 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f02d4953acb0d7df070fb58758486206f2977caf26c5094197832400b84de4a`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 10.0 KB (9999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4248dea411b3dbc103d573a628ca9da62d3aeb14d620db9e8a298d8072272834`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 813.9 KB (813878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c05c149f86a3534ba1fc868d4c24836c5cb669464120d6e1362b45410dc55bc`  
		Last Modified: Wed, 16 Sep 2020 19:46:19 GMT  
		Size: 7.3 MB (7300073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f895c50e263cdc2860e552bd70347d292848576612330c786a126a6d3611907`  
		Last Modified: Wed, 16 Sep 2020 19:46:29 GMT  
		Size: 61.0 MB (60988464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ec89d9d1a434e84ff9a030fb2f07bf5cea8d8a0e36b668da65a06d7028846e`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:alpine`

```console
$ docker pull ghost@sha256:9c5c8e9a0585f46ea87be6f2fe6eb8e521ab5fcb9a2c1585d37b8230c0add9a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ghost:alpine` - linux; amd64

```console
$ docker pull ghost@sha256:71422ddf0230e11db21c0c38298a7a57ec9c2bf2ea2f9044303ca25b5f7205a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114617502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40128288ca81dcda5779742757851149b0d7aee322f854b1a65a030d7a49e836`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 15:24:55 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 15:25:00 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 15:25:00 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 15:25:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 15:25:03 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 15:25:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 15:25:03 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:32:09 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:32:11 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:32:12 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:32:12 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:32:46 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:32:47 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 18:35:05 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:35:08 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:35:08 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:35:09 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:35:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:35:09 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:35:10 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d481011659a13bdb095379d64b4b858612ae1b923da2247c8fc97d52920c72`  
		Last Modified: Wed, 16 Sep 2020 15:32:07 GMT  
		Size: 24.7 MB (24663724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fabc993f172c5fea591f7820f283ca6e238289b3414930dbc808a392f80e9f`  
		Last Modified: Wed, 16 Sep 2020 15:32:01 GMT  
		Size: 2.2 MB (2239084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834ca887ea10ccf5c773b01efa3b1331ba97b7b9fa6fc0c00f8577e96491ab05`  
		Last Modified: Wed, 16 Sep 2020 15:32:00 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad02ebe5fd045290b160178a369c06b5dcac3794f366b205e5322eb55104ec48`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 9.9 KB (9907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac08c3f0139584f5793c0781db31b35c5d858ec8bb3a1dfc10049ac143bf2ed`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 780.5 KB (780521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fc087e6a7813bb7d52f69744d4345fb4f8ad65c14136cacc67425cb987a7e0`  
		Last Modified: Wed, 16 Sep 2020 18:41:45 GMT  
		Size: 7.3 MB (7300226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846777c8cbce526597e1ae3c9c3efb82431d2b2bbd9bbe50fa687c396e0d598e`  
		Last Modified: Wed, 16 Sep 2020 18:42:10 GMT  
		Size: 76.8 MB (76809897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ad64533e5521e02c68f5678ce64c996b9d824dd3a049424d43bf62a35f8599`  
		Last Modified: Wed, 16 Sep 2020 18:41:39 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:2f0461412b5a7d20d2b83d981ff288371bc0fe3b55ed276e7471c1ee9e228b4c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97918500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80981f34643bb72ee481471e59a59cc4116735ae69e1dd1cc4cf8fc978a54d57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 17:40:49 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 17:52:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 17:52:05 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 17:52:11 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 17:52:12 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 17:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 17:52:13 GMT
CMD ["node"]
# Wed, 16 Sep 2020 18:32:16 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 18:32:19 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 18:32:20 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 18:32:20 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 18:33:04 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 18:33:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 18:33:06 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 18:33:07 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 18:41:13 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 18:41:17 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 18:41:18 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 18:41:19 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 18:41:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:41:20 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 18:41:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e605218299f7ebd25e155350c848b92a6f4810477b1083671724070a7aa964`  
		Last Modified: Wed, 16 Sep 2020 18:18:24 GMT  
		Size: 24.0 MB (24041343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13e15a2cc15c85379c3ab92c66be1ca42bab48af072297a6fb6b894b2421375`  
		Last Modified: Wed, 16 Sep 2020 18:18:17 GMT  
		Size: 2.3 MB (2285910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1d335135bbad11f2f7056cd20d0f827f75cc05f21ab4b34db1b1559104816d`  
		Last Modified: Wed, 16 Sep 2020 18:18:16 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c3aea8810324c5d99029432a38ed6d03f5cda6e3b9e882c6c7b61c63e0158a`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 9.7 KB (9730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db17565d2a0e255adb6b10c8202a9a1d1f4d866dc385fc85dec670ca6b4f659`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 733.5 KB (733459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53d0c45c43f7049dbfe5986cf9409cadccf8daa91f9459157c988614b7de4a9`  
		Last Modified: Wed, 16 Sep 2020 18:48:33 GMT  
		Size: 7.3 MB (7300584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4e951a483befd38eee02289a488a49411bf6fd6c0d274da1ceace6f0466532`  
		Last Modified: Wed, 16 Sep 2020 18:48:59 GMT  
		Size: 60.9 MB (60926713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0407553e0478012410791ca34224a66b74ddd7f6782d713ad15b2b51f7f6f12`  
		Last Modified: Wed, 16 Sep 2020 18:48:28 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:2ce114fc60a7d6c37b9ad68e569206780f25d0bf9c1d90a3b511ebc308f57ac8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97152917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5de87dfb6964133b28f4841088e7ae8a7d8a9201e1bb7a2304fd3f393ce5dfcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Tue, 28 Jul 2020 23:02:12 GMT
ENV NODE_VERSION=12.18.3
# Tue, 28 Jul 2020 23:11:16 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="14dafe026366e7a9cc8d4737b1fcdcb6c534667e22bbeea63a29a1791ac6ac1f"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 28 Jul 2020 23:11:18 GMT
ENV YARN_VERSION=1.22.4
# Tue, 28 Jul 2020 23:11:24 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 28 Jul 2020 23:11:25 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Jul 2020 23:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jul 2020 23:11:26 GMT
CMD ["node"]
# Tue, 28 Jul 2020 23:42:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 28 Jul 2020 23:42:48 GMT
RUN apk add --no-cache 		bash
# Tue, 28 Jul 2020 23:42:49 GMT
ENV NODE_ENV=production
# Tue, 28 Jul 2020 23:42:50 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Tue, 28 Jul 2020 23:43:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 28 Jul 2020 23:43:25 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 28 Jul 2020 23:43:26 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 21:09:49 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 21:15:11 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 21:15:18 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 21:15:18 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 21:15:19 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 21:15:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 21:15:23 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 21:15:24 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f88341ca4dc0bb7536c1e100534891dc1a168d2c735d3d4a4f658e7aa2c266c`  
		Last Modified: Tue, 28 Jul 2020 23:20:06 GMT  
		Size: 23.6 MB (23598149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5765f8fb68cd71c84db4cb118d2ab3bd6a19013b9240ff2056f7fcfa559bc25c`  
		Last Modified: Tue, 28 Jul 2020 23:19:58 GMT  
		Size: 2.3 MB (2282799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6b46590934f315dfb60ee5b8226e4a8497a770741284fd71d5cd1da891a92a`  
		Last Modified: Tue, 28 Jul 2020 23:19:57 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c6422aa60b4062bf328de58bb22b8a65348f89bfc277d177475ff922a89ab1`  
		Last Modified: Tue, 28 Jul 2020 23:50:07 GMT  
		Size: 9.5 KB (9518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c480bb1a2cab70d156cea495576a482dde69143faad108ee5f628ecb9a22090`  
		Last Modified: Tue, 28 Jul 2020 23:50:07 GMT  
		Size: 669.0 KB (669039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b7a0b1789749d7d72bd946a8c6b5e179bfdf1f71a384787d8fbac65a68051e`  
		Last Modified: Tue, 28 Jul 2020 23:50:12 GMT  
		Size: 7.3 MB (7293372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fef1ea3a3423a43d694755d781da1619d6fc46212b7609b3e4a85a4b15794df`  
		Last Modified: Mon, 14 Sep 2020 21:17:17 GMT  
		Size: 60.9 MB (60877148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd85b50f3a4d49155beb33fcd84951af378509818299758723d78db1af9ef615`  
		Last Modified: Mon, 14 Sep 2020 21:16:48 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:edbfa992b7732a11778ac27801400706e18da3467faf8ceb3a23d14983c832b7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98969473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926eaaf8960d968624da1cc7493d138a2cc5c1b2d58dc45d2b564a2bb1801f59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 17:55:53 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 18:06:53 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:06:57 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:07:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:07:18 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:07:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:07:21 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:36:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:36:09 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:36:10 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:36:11 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:36:55 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:36:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:36:58 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:36:59 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:42:20 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:42:28 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:42:30 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:42:31 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:42:33 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:42:34 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1cd5d2badbefd21b1a2bfeabb1fdc13a95ce2ec44782c6ecd0b77f3e6941c6`  
		Last Modified: Wed, 16 Sep 2020 18:38:54 GMT  
		Size: 24.8 MB (24756587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375b3dfef9959f5439912c8c672ef9c97530d682060b1482c26d52b5ec9cf53e`  
		Last Modified: Wed, 16 Sep 2020 18:38:46 GMT  
		Size: 2.3 MB (2295913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8810cf1c388f6776673bed88ff3a465609c960d04f3c890200fe6dfd38809c39`  
		Last Modified: Wed, 16 Sep 2020 18:38:45 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4efecdee57df77fa1df7bc627da0525636ad27b3e917bb2964d740cd7dfc4fc`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 9.8 KB (9846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57353ed8f63a6d635482a86f40236c3e970e0ef7d5e17ea3628dc69e32f26c`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 792.1 KB (792147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2905b594425e7dc51144ae220d8a8383f08191c81d2bb7ca6b3aa4b41de843c0`  
		Last Modified: Wed, 16 Sep 2020 19:54:47 GMT  
		Size: 7.3 MB (7300575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa26c519d4bdf9a2a160800d64aff80745163fd0b989b38570d7a80daed0aef3`  
		Last Modified: Wed, 16 Sep 2020 19:55:11 GMT  
		Size: 61.1 MB (61089153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e78475cfa090323364fa7f0b93245db4a7d6650fb852957aacde045fbe46a40`  
		Last Modified: Wed, 16 Sep 2020 19:54:43 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; 386

```console
$ docker pull ghost@sha256:70af1d6c5bccddf1659593d7ba73f953233a7ce30c2e0128a93d51ac51868456
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99653175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b09e291565fd5cc649a07817b589a1db940bf71e14ec9af3920966de1975136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 04:47:36 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 05:31:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 05:31:04 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 05:31:07 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 05:31:08 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 05:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 05:31:08 GMT
CMD ["node"]
# Wed, 29 Apr 2020 06:19:37 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 06:19:38 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 06:19:38 GMT
ENV NODE_ENV=production
# Wed, 10 Jun 2020 00:16:55 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 10 Jun 2020 00:17:29 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 10 Jun 2020 00:17:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 10 Jun 2020 00:17:30 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 18:38:26 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 18:41:54 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 18:41:55 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 18:41:55 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 18:41:56 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 18:41:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 18:41:56 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 18:41:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a146da8782b0a2b78256aaa25ee92fd617354f694aeace2b3951fab07b027563`  
		Last Modified: Wed, 29 Apr 2020 05:32:18 GMT  
		Size: 24.9 MB (24931595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cb15e48bd1247c878221de413f1942fb7a082c5b789c0b94a025b6e8a0acfe`  
		Last Modified: Wed, 29 Apr 2020 05:32:12 GMT  
		Size: 2.3 MB (2294631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795a10dfdcd143e79354ce37f2fcb9dd923fbc4d3e6281f1be5c8619b654624b`  
		Last Modified: Wed, 29 Apr 2020 05:32:11 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c2188990e50e91234b3066f2b83b08529f15057c14fda8799fdbbedfc33fd3`  
		Last Modified: Wed, 29 Apr 2020 06:23:16 GMT  
		Size: 10.0 KB (9986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987839397957204c0cb5fe48a8aac315882c2895e54e2588a761de6afe65c215`  
		Last Modified: Wed, 29 Apr 2020 06:23:16 GMT  
		Size: 829.5 KB (829504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1630953e291089e0490110657600604529e883f14b3002ddeac8ce34a93c16d7`  
		Last Modified: Wed, 10 Jun 2020 00:27:20 GMT  
		Size: 7.0 MB (7039287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925357b76e685eb00009b4ac955f8512ca5e579d5a042ee1ff3733587033f372`  
		Last Modified: Mon, 14 Sep 2020 18:42:45 GMT  
		Size: 61.7 MB (61738924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081dc2975c2444bf667c099101941a6d056065a0104e0232446cb8967d4c2cd9`  
		Last Modified: Mon, 14 Sep 2020 18:42:22 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:43b9d662f9e9433d4830de84a3d8493b526a5df31ac8658e33ae704713ea0574
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102780220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfa0420ce1ad11f6d9a691e6d61f0ea27861e2e77b1cea8219a151cd98cf422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Tue, 28 Jul 2020 23:33:17 GMT
ENV NODE_VERSION=12.18.3
# Tue, 28 Jul 2020 23:51:22 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="14dafe026366e7a9cc8d4737b1fcdcb6c534667e22bbeea63a29a1791ac6ac1f"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 28 Jul 2020 23:51:34 GMT
ENV YARN_VERSION=1.22.4
# Tue, 28 Jul 2020 23:52:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 28 Jul 2020 23:52:39 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Jul 2020 23:52:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Jul 2020 23:53:16 GMT
CMD ["node"]
# Wed, 29 Jul 2020 00:58:42 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Jul 2020 00:59:16 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Jul 2020 00:59:42 GMT
ENV NODE_ENV=production
# Wed, 29 Jul 2020 01:00:10 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 29 Jul 2020 01:02:23 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Jul 2020 01:02:41 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Jul 2020 01:02:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 14 Sep 2020 18:47:52 GMT
ENV GHOST_VERSION=3.33.0
# Mon, 14 Sep 2020 19:02:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 14 Sep 2020 19:03:08 GMT
WORKDIR /var/lib/ghost
# Mon, 14 Sep 2020 19:03:16 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 14 Sep 2020 19:03:20 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 14 Sep 2020 19:03:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Sep 2020 19:03:35 GMT
EXPOSE 2368
# Mon, 14 Sep 2020 19:03:42 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e63182081bd58ba56f2f6a735728ecb0ec58a515e53c2b51cd53a3b4d91267`  
		Last Modified: Wed, 29 Jul 2020 00:10:24 GMT  
		Size: 26.9 MB (26927412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66eb37d28bad1d1c3b133e60bdd89387811b5663328c18e29146d8c8b6f11c50`  
		Last Modified: Wed, 29 Jul 2020 00:10:18 GMT  
		Size: 2.3 MB (2290366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79656e9e9a7bfb983771444038c32dbcc5e19fdd81d78f9c0ee464268bc06321`  
		Last Modified: Wed, 29 Jul 2020 00:10:17 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9114a35fd6126880d15252899fe21b48ba55e1e4c9fa03d888fb9a36d180f6c4`  
		Last Modified: Wed, 29 Jul 2020 01:27:15 GMT  
		Size: 10.4 KB (10403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28565886d5e4396566e6d78ed848e79d95df6b94cce9b93e6b8b4d580d95c20b`  
		Last Modified: Wed, 29 Jul 2020 01:27:24 GMT  
		Size: 862.6 KB (862611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bbd2d0bce62ba7d010e6469f3b646d5d46b6233b91daef6708ced4fc614e69`  
		Last Modified: Wed, 29 Jul 2020 01:28:43 GMT  
		Size: 7.3 MB (7293562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28abb5ff19322ee34b1efb387cc0204aff31935ccefdbc50988a478bd218e11c`  
		Last Modified: Mon, 14 Sep 2020 19:17:23 GMT  
		Size: 62.6 MB (62573194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d54949e6aac2cab1e62021ca349d7b78c9a2e6fae68bc081a9f9b96cded0e4e`  
		Last Modified: Mon, 14 Sep 2020 19:11:56 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; s390x

```console
$ docker pull ghost@sha256:bd627e9ca1c40e4b19f18229baab850fef538ebeff614f3bbb0c4651e511330b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98684460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30c836dd8e506e4e2d8d7ab3e2d7cc03ca42100103b77a8c2da58883b3033ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:24:02 GMT
ENV NODE_VERSION=12.18.4
# Wed, 16 Sep 2020 18:40:03 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="99715657ad621bd364070f176d27c6902ce49441af88e5df2dbe63392a3097da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 16 Sep 2020 18:40:05 GMT
ENV YARN_VERSION=1.22.4
# Wed, 16 Sep 2020 18:40:08 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 16 Sep 2020 18:40:08 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 16 Sep 2020 18:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 18:40:08 GMT
CMD ["node"]
# Wed, 16 Sep 2020 19:38:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 16 Sep 2020 19:38:58 GMT
RUN apk add --no-cache 		bash
# Wed, 16 Sep 2020 19:38:58 GMT
ENV NODE_ENV=production
# Wed, 16 Sep 2020 19:38:58 GMT
ENV GHOST_CLI_VERSION=1.14.1
# Wed, 16 Sep 2020 19:39:11 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 16 Sep 2020 19:39:13 GMT
ENV GHOST_VERSION=3.33.0
# Wed, 16 Sep 2020 19:41:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 16 Sep 2020 19:41:14 GMT
WORKDIR /var/lib/ghost
# Wed, 16 Sep 2020 19:41:15 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 16 Sep 2020 19:41:15 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 16 Sep 2020 19:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Sep 2020 19:41:15 GMT
EXPOSE 2368
# Wed, 16 Sep 2020 19:41:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e01d2cb5fa863d8474d4a62c71b1f35bcc70df77277e17a98f9231c06d7b035`  
		Last Modified: Wed, 16 Sep 2020 19:18:07 GMT  
		Size: 24.7 MB (24689695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ec78b6807a9d38521411c53a6a242f5f37dc57c71daf298d5d3b6cf8f22445`  
		Last Modified: Wed, 16 Sep 2020 19:18:04 GMT  
		Size: 2.3 MB (2298669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3729460d3bf14be267588928707b7f6a9f8f5bfdf695a887a88a2d5a0741389`  
		Last Modified: Wed, 16 Sep 2020 19:18:03 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f02d4953acb0d7df070fb58758486206f2977caf26c5094197832400b84de4a`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 10.0 KB (9999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4248dea411b3dbc103d573a628ca9da62d3aeb14d620db9e8a298d8072272834`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 813.9 KB (813878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c05c149f86a3534ba1fc868d4c24836c5cb669464120d6e1362b45410dc55bc`  
		Last Modified: Wed, 16 Sep 2020 19:46:19 GMT  
		Size: 7.3 MB (7300073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f895c50e263cdc2860e552bd70347d292848576612330c786a126a6d3611907`  
		Last Modified: Wed, 16 Sep 2020 19:46:29 GMT  
		Size: 61.0 MB (60988464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ec89d9d1a434e84ff9a030fb2f07bf5cea8d8a0e36b668da65a06d7028846e`  
		Last Modified: Wed, 16 Sep 2020 19:46:18 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
