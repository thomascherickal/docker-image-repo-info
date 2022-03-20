<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ghost`

-	[`ghost:4`](#ghost4)
-	[`ghost:4-alpine`](#ghost4-alpine)
-	[`ghost:4.39`](#ghost439)
-	[`ghost:4.39-alpine`](#ghost439-alpine)
-	[`ghost:4.39.1`](#ghost4391)
-	[`ghost:4.39.1-alpine`](#ghost4391-alpine)
-	[`ghost:alpine`](#ghostalpine)
-	[`ghost:latest`](#ghostlatest)

## `ghost:4`

```console
$ docker pull ghost@sha256:8dbf032df937aee9b24ea5bce598e76560fedfa8a3c3bf9ab53478be8053dd22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:4` - linux; amd64

```console
$ docker pull ghost@sha256:7df40e0443f1348977c629d0c6739332c60a93a59a864cf0c059e9081f69b538
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.3 MB (148271097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:669ab852b2633345fef2005c32cf301d19548ef7485faea31af70a7e4fcfd45e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 13:00:01 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 21:50:00 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 21:50:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 21:50:35 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:50:47 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 21:50:47 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:50:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:50:47 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:04:25 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 00:04:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 00:04:43 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:04:44 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 00:05:16 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 00:06:45 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 00:06:47 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 00:06:47 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 00:06:47 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 00:06:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:06:48 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 00:06:48 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bc29d3bc64ca0852101d86667b4a0d1908f05fe0bfead140cf838c0be01bc3`  
		Last Modified: Thu, 17 Mar 2022 13:19:15 GMT  
		Size: 4.2 KB (4183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a71a1d6cc6986624592a148f866355b9b90ddcd4a1f24be36b0f849d8c1044`  
		Last Modified: Fri, 18 Mar 2022 22:14:33 GMT  
		Size: 36.0 MB (36048047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5afd073302f60aad2c5067b89a976a5572fa262d0b60478970f307f8f94b97`  
		Last Modified: Fri, 18 Mar 2022 22:14:27 GMT  
		Size: 2.8 MB (2781848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5878f59eaa39846dd1173083e2e77dc140082be0efc61f7838c3403c6254b113`  
		Last Modified: Fri, 18 Mar 2022 22:14:26 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753aec878444f5bbf5b9e13544f6a3caf78aae1d01d506806f4b342c32623f2a`  
		Last Modified: Sat, 19 Mar 2022 00:09:27 GMT  
		Size: 1.4 MB (1448123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e282a0a274714713330c2ae37bb9aa1be203226d7ffd7de6eec07f2e35270c8`  
		Last Modified: Sat, 19 Mar 2022 00:09:31 GMT  
		Size: 9.6 MB (9567975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6128fb86f0f4e39a32aa4c08d17f607dd59d85e5f88743f9c8e88dd758997be6`  
		Last Modified: Sat, 19 Mar 2022 00:09:44 GMT  
		Size: 67.0 MB (67043352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f7cfac26d6d851aa8ff0c01c9d486dbea8e2db7dc31aa28842be210035fb5`  
		Last Modified: Sat, 19 Mar 2022 00:09:26 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4` - linux; arm variant v7

```console
$ docker pull ghost@sha256:78719e5300fc6838cdfe4fe7bc7b089fcae5c3970dee91fbcbc37e9c6d3c7475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147043059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34fb82b494adf39572f85b07c9779bb0b0724e4e29049dc5ad3404f173ba3abd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 14:47:47 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 22:50:57 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:51:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 22:51:48 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:52:22 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 22:52:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:52:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:52:23 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:22:42 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 23:23:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 23:23:10 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:23:10 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:23:59 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 23:31:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 23:31:50 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 23:31:50 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 23:31:50 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 23:31:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:31:51 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 23:31:52 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c69f71c16ec3df2b7d124845d1b3b6e6495150f4ea3398c32a390afffbf142`  
		Last Modified: Fri, 18 Mar 2022 17:06:49 GMT  
		Size: 4.2 KB (4166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b32ca858e17b62400e3e3939b76745bd091c2302dcb5a659f98f4036c58ad`  
		Last Modified: Sat, 19 Mar 2022 00:07:18 GMT  
		Size: 34.2 MB (34206692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2605fefc93565569e993984be795855508fc11258205a2f0ab736807a40c2c`  
		Last Modified: Sat, 19 Mar 2022 00:06:56 GMT  
		Size: 2.8 MB (2772408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a649abf5b9f938b138570d940f0d8c3af7d265d4e26a25cf69fbd121df9381c`  
		Last Modified: Sat, 19 Mar 2022 00:06:54 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4041d8d2d15b52a58284107ec1fbc633900cce1fc07418607ed52ea1564428aa`  
		Last Modified: Sat, 19 Mar 2022 23:41:13 GMT  
		Size: 1.4 MB (1400322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04c308287b4673d9ba168fbb3d4cec8b9c7e8a9fe4ce8e8bab11f7a83658e18`  
		Last Modified: Sat, 19 Mar 2022 23:41:27 GMT  
		Size: 9.6 MB (9569190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25431520d805b108ecaf6cbf6e20b77e5401b5e75a367d828d99d0a68a2612d0`  
		Last Modified: Sat, 19 Mar 2022 23:42:23 GMT  
		Size: 72.5 MB (72514183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb31846b09f2de8a7bb58d2524fb744ac8124092cd9ee0a6f2ba64f8e8cf782`  
		Last Modified: Sat, 19 Mar 2022 23:41:12 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:f4a663d141c3204ae4bc882b0fc57cb214361f6b4c8bde126b67c24aad420674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154343013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a20e32182de795f606b46f40248f7b94fc474d808fe5fd7d57d6417b85d50fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:20:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 23:50:24 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:50:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 23:50:49 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:51:01 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 23:51:03 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:51:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:51:04 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:41:23 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 17:41:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 17:41:34 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:41:35 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 17:42:09 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 17:42:11 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 17:42:12 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 17:42:13 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 17:45:21 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 17:45:24 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 17:45:26 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 17:45:29 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 17:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:45:34 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 17:45:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e302ce9f0603b4af265c90ba2a4807900c24096808fb68bf44300bd440542`  
		Last Modified: Thu, 17 Mar 2022 13:54:35 GMT  
		Size: 4.0 KB (4042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98badb25d325c02976fab44804955d995b60a19fc609da8e3f1e642c52d898f9`  
		Last Modified: Sat, 19 Mar 2022 00:54:11 GMT  
		Size: 36.2 MB (36154505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5d43df9c11963e4b0e365e779e63981833ea41bdcc5d4db11c675fcc84fab3`  
		Last Modified: Sat, 19 Mar 2022 00:54:06 GMT  
		Size: 2.8 MB (2781278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad002987a7bae850089e45777bc9a362a9f8e3c656bdbbb26980ec4776d4704b`  
		Last Modified: Sat, 19 Mar 2022 00:54:05 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643f6d4797a5cc96449c367b48271ff6c2fdb6908b35b0b9c4c548113d8535a9`  
		Last Modified: Sat, 19 Mar 2022 17:50:44 GMT  
		Size: 1.4 MB (1383662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cde83364d3aeeba3311efa235a8b37ae7bbe49fd46d82e326c8c363b094c82`  
		Last Modified: Sat, 19 Mar 2022 17:50:46 GMT  
		Size: 9.6 MB (9568502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f817e8e904ee939974f5e8f516b174c335682a40a40694832630f3270b0e296`  
		Last Modified: Sat, 19 Mar 2022 17:50:58 GMT  
		Size: 74.4 MB (74387013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d099ce69b402eb198ddea013bbe31fe8ba1a37a42105d092444d276d82d59d61`  
		Last Modified: Sat, 19 Mar 2022 17:50:43 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4` - linux; ppc64le

```console
$ docker pull ghost@sha256:ce8b4d8f9715c7c70c7e6e1746f7535091887d178ca17dc773a8bd7dfb673f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155730905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97937daf1eb28848ecc7f38f97257c3d3573a82441d3c76be44346b51497cc36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 11:17:54 GMT
ADD file:e8555f1cb439a45786b92e929cfa154b51f668c5b4cd69e4ce98340c5998fe0c in / 
# Thu, 17 Mar 2022 11:18:00 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 03:54:03 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 23:06:48 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:11:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 23:11:09 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:14:42 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 23:14:44 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:14:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:14:53 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:46:25 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 23:47:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 23:47:53 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:47:55 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:49:09 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:49:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:49:15 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:49:17 GMT
ENV GHOST_VERSION=4.39.1
# Sun, 20 Mar 2022 00:11:36 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sun, 20 Mar 2022 00:11:46 GMT
WORKDIR /var/lib/ghost
# Sun, 20 Mar 2022 00:11:51 GMT
VOLUME [/var/lib/ghost/content]
# Sun, 20 Mar 2022 00:11:52 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sun, 20 Mar 2022 00:11:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 00:11:59 GMT
EXPOSE 2368
# Sun, 20 Mar 2022 00:12:01 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:aec78dc45d7b3df12df0672d13e22005592b453f03ff2580efac2598dddd680b`  
		Last Modified: Thu, 17 Mar 2022 11:28:17 GMT  
		Size: 35.3 MB (35279758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca53b81b04fce4349fb7d53e6c96231409ea54bc6d07808c393a268d8fcd78c3`  
		Last Modified: Fri, 18 Mar 2022 08:33:21 GMT  
		Size: 4.2 KB (4190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307e188a803758441743ab6c2c16c58d32cd25920f05e601d9fa75c13f8ec1f4`  
		Last Modified: Sat, 19 Mar 2022 02:15:29 GMT  
		Size: 38.0 MB (37978420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6a74008e734f41eb1091af470bca5677108b1eb61729b017bd6e96944fc1c1`  
		Last Modified: Sat, 19 Mar 2022 02:15:22 GMT  
		Size: 2.8 MB (2782569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9e81db75711e347d46105e0daee9e64692433ad3141a1cf1a52bca316993e`  
		Last Modified: Sat, 19 Mar 2022 02:15:22 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d14ae585ca54d978c72b25f6580d1c2986a60f049aefed6a7146e58b8eb07da`  
		Last Modified: Sun, 20 Mar 2022 00:12:26 GMT  
		Size: 1.4 MB (1367834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4904132a0f018373255a9418743ef13604d402190eaf4737c0de15b28964951`  
		Last Modified: Sun, 20 Mar 2022 00:12:31 GMT  
		Size: 9.6 MB (9568608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12320605293f45afa67cc47adf173b0888368bb06886b3b219e3cd4a68fafac`  
		Last Modified: Sun, 20 Mar 2022 00:12:43 GMT  
		Size: 68.7 MB (68748529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270139457a810a99e7dd44848741575b541fe0de273a395f04a5c15fb54ccb23`  
		Last Modified: Sun, 20 Mar 2022 00:12:26 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4` - linux; s390x

```console
$ docker pull ghost@sha256:45b1aa5e819038cf640e167b5a5a4ee3b7b1f8f534b9eef0696dbfe88a14e27c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.5 MB (147499556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a439d42fd5331e4df800fb4597e9eb5c12e1e4aa7a72b029fc59b3b884edd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:50:36 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 22:14:52 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:15:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 22:15:12 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:15:21 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 22:15:21 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:15:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:15:22 GMT
CMD ["node"]
# Sat, 19 Mar 2022 04:38:44 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 04:38:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 04:38:53 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 04:38:53 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 04:39:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 04:39:24 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 04:39:24 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 04:39:25 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 04:42:06 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 04:42:15 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 04:42:15 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 04:42:16 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 04:42:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 04:42:16 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 04:42:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722821cfaf9b99e01207f42d38caa8d0eea9818925d58a5d590057ff6271525d`  
		Last Modified: Thu, 17 Mar 2022 14:21:32 GMT  
		Size: 4.2 KB (4189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924acd2003e404035ae30769a9ed0531c116ccfe4965f354999da4c593b38dc`  
		Last Modified: Fri, 18 Mar 2022 23:10:07 GMT  
		Size: 35.9 MB (35913738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1c92724e1dbac9baa9b4949197499bd94e7abda3f1392dd48cc6f78fb23589`  
		Last Modified: Fri, 18 Mar 2022 23:10:03 GMT  
		Size: 2.8 MB (2782997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f42e3d4bc22c450816fb2255b83b884ec091394d12aff4a84c65c1193e935a`  
		Last Modified: Fri, 18 Mar 2022 23:10:03 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a61fd10dbc4124b4be87498e57bca3e89cab9d50ed7acf9934d6103e2b32eb`  
		Last Modified: Sat, 19 Mar 2022 04:42:48 GMT  
		Size: 1.4 MB (1434956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d6f9332f2c9557e6d14acdf3a51fb916f10fa41d64027309df97ce26b51dbc`  
		Last Modified: Sat, 19 Mar 2022 04:42:49 GMT  
		Size: 9.6 MB (9567431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b22e8969248f953b6c6d82f75ca2021591edf483759ad1672850841c2b90299`  
		Last Modified: Sat, 19 Mar 2022 04:42:59 GMT  
		Size: 68.1 MB (68139455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db7bc896fefc28b64d7f40ca85f1aed46b128fcde04b0748a3ddfe437daa11`  
		Last Modified: Sat, 19 Mar 2022 04:42:47 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4-alpine`

```console
$ docker pull ghost@sha256:ef482080ea2121a9bb8d3fd13500cb4efebe814f88c336ca51a8d38ed7c116cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:4-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:7fba69cb1b1ab7ab7e22bcaaec6fd1374e7aecf667c734610d9df7c42b93870f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120407221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:847bc2aee68921734b296bc3253f6636fd8eb311b664e6282eb6be1f5f91ea44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 21:48:35 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 21:48:49 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 21:48:49 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:48:55 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 21:48:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:48:56 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:07:05 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 00:07:07 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 00:07:07 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:07:07 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 00:07:34 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 00:08:56 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 00:08:58 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 00:08:58 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 00:08:59 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 00:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:08:59 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 00:08:59 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580248b309d4fecaf2f75f42a36796a166140238395d38d36e0d47b20dded70`  
		Last Modified: Fri, 18 Mar 2022 22:13:15 GMT  
		Size: 37.1 MB (37132855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539902d50a314143ea1ff8b98bee2aae6a9e66b7f102cd5b0ba0b3b21650132e`  
		Last Modified: Fri, 18 Mar 2022 22:13:07 GMT  
		Size: 2.4 MB (2358489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44d60032af439ffa29833ceee54906865bfc7e32949f8a0643d3e1f7307d6e`  
		Last Modified: Fri, 18 Mar 2022 22:13:06 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d799310e8353a5bf7d35c0a576c8cc8a22f423a2268da6c937e55e512240daf`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 11.2 KB (11209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c87a58ecffcb615b1c9af4968b84fdfb44fd7f432d7d7c6087a14f7ba7f201e`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 816.9 KB (816859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf689cb927dd935805d71b57cb514cc956df63b009fc1453a79c668d2dad985d`  
		Last Modified: Sat, 19 Mar 2022 00:10:04 GMT  
		Size: 9.6 MB (9567883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b38a95a7d42f2ed48ffada1b7b31d395594b24e4b51d8eef0ddf93afe6b8595`  
		Last Modified: Sat, 19 Mar 2022 00:10:17 GMT  
		Size: 67.7 MB (67702755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddb7f12b2dcac2bc19d55fffdc3e5ada0a10ab45407f0e313834954f852e2b0`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:6108db40dd7418795073f3d3bfd9fe0366cbd252d11bef46e6dbad514176d85e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121612527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5444505489f48c5995f748bb4d4bce479dc4e9eb1d995986a6fa7455bf9886c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 19:31:23 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 19:47:55 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 19:47:56 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 19:48:04 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 19:48:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 19:48:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 19:48:06 GMT
CMD ["node"]
# Fri, 18 Mar 2022 21:05:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 18 Mar 2022 21:05:06 GMT
RUN apk add --no-cache 		bash
# Fri, 18 Mar 2022 21:05:06 GMT
ENV NODE_ENV=production
# Fri, 18 Mar 2022 21:05:06 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Fri, 18 Mar 2022 21:06:20 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 18 Mar 2022 21:06:21 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 18 Mar 2022 21:06:22 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 18 Mar 2022 21:06:22 GMT
ENV GHOST_VERSION=4.39.1
# Fri, 18 Mar 2022 21:16:25 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 18 Mar 2022 21:16:29 GMT
WORKDIR /var/lib/ghost
# Fri, 18 Mar 2022 21:16:29 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 18 Mar 2022 21:16:30 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 18 Mar 2022 21:16:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:16:32 GMT
EXPOSE 2368
# Fri, 18 Mar 2022 21:16:33 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd48496521270c1ba2c1d855bd715f617b59d6498e2e407b804b566b7678087`  
		Last Modified: Fri, 18 Mar 2022 20:47:14 GMT  
		Size: 36.2 MB (36198526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5599fde36163c1ebda1ad804a5b327cc1609b46263a91060b9fc3a835d328be9`  
		Last Modified: Fri, 18 Mar 2022 20:47:01 GMT  
		Size: 2.4 MB (2418192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18709050207fe0cf4803ac4f14090c67a8729cd62b866e31ae708d3b6e7b9166`  
		Last Modified: Fri, 18 Mar 2022 20:46:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af606d946314fedea65ebbae67cbd1cecf6a786558facb4b88f3f5739e15c45b`  
		Last Modified: Fri, 18 Mar 2022 21:17:09 GMT  
		Size: 11.0 KB (10977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0954b81f1ae01a7d7b8339d694eef033a3a078ca6a23c44e8934eb1c6229c0`  
		Last Modified: Fri, 18 Mar 2022 21:17:10 GMT  
		Size: 771.0 KB (770953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455c516cdd5fda37a751a4a4b7ef0e58ecb18b7c3fb786fb1f485daa97406bee`  
		Last Modified: Fri, 18 Mar 2022 21:17:19 GMT  
		Size: 9.6 MB (9569616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8e836532b22085f33122bfa92e57f9b6cb7f6679237f396b7493ac9a1c5833`  
		Last Modified: Fri, 18 Mar 2022 21:17:55 GMT  
		Size: 70.0 MB (70013905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece8cd2cd02390a0b0e5b514593ce36f25efaab79f731bbf280d80f1450a7d01`  
		Last Modified: Fri, 18 Mar 2022 21:17:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:ce4864a56a2ec745d71119586a3a6ead3bb50b57952c003eb737d823fee66c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120368095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a90bb3b146463403b2cb1d5e44a034d0bd3a9e5c2c31efdf31f6f4b48d62f36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 17:21:06 GMT
ADD file:c25fcf153ea349f64e08a1bd0756ce550f2a081ad56cc40c89027d85d1bc26da in / 
# Thu, 17 Mar 2022 17:21:06 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 22:22:50 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:36:08 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 22:36:09 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:36:16 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 22:36:17 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:36:18 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:32:10 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 23:32:12 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 23:32:13 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:32:13 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:33:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:33:06 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:33:07 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:33:07 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 23:40:19 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 23:40:22 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 23:40:23 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 23:40:23 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 23:40:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:40:24 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 23:40:25 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c3a1157c36d8d156f7664fa098212ab2149a64bcb59767cdf4595a86617c17fd`  
		Last Modified: Thu, 17 Mar 2022 17:22:45 GMT  
		Size: 2.4 MB (2430456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7fb7593e1ec2c0060c773dbbf85fcbe77df0a45cbc891cd7f775442f959ce6`  
		Last Modified: Sat, 19 Mar 2022 00:04:50 GMT  
		Size: 35.8 MB (35750941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b531d0f3fa4a8c1e5c8c32c0c6a9de8cda1e078ed43db62853858f7ef792044b`  
		Last Modified: Sat, 19 Mar 2022 00:04:27 GMT  
		Size: 2.4 MB (2418360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ead18221dfbeb2afd1c7044892b00c01b6b056d5feb01c74684dff97d67e8eb`  
		Last Modified: Sat, 19 Mar 2022 00:04:26 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1faeeef23a40a6e07406285a95e3f94a86314cef806a54bbf3e2672288624dc`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 10.8 KB (10772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41729cace1ddd94023eba72c5c881b17ee1ab0e939be1d113c4f144fdae876c1`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 703.9 KB (703890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1f8edf6ec39144c3fa34019e53bf9892978c935ab4b45e035f61c9cd7e32b`  
		Last Modified: Sat, 19 Mar 2022 23:42:57 GMT  
		Size: 9.6 MB (9569052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8628b5b59160ec4766d80912273c9024695381f2b717407a91177b03925b4dd9`  
		Last Modified: Sat, 19 Mar 2022 23:43:56 GMT  
		Size: 69.5 MB (69483628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678ef4fd7c46697fe04cca3f1ecc814f51b56a03ea9abb66a3c1fb7c22093eb6`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:4f35663f73dfc11751365716b7d6a9d08e66e2cd0b7b6d6d276e9167c66dbe21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140115021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b197627739a94af9bff95a19a902e84b7a352936df176d8b8dc38f329a3c9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 23:07:29 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:28:15 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 23:28:15 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:28:21 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 23:28:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:28:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:28:23 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:45:45 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 17:45:47 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 17:45:47 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:45:48 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 17:46:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 17:46:27 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 17:46:28 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 17:46:29 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 17:49:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 17:49:59 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 17:50:01 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 17:50:04 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 17:50:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:50:08 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 17:50:11 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c992e90d8c9f9d1552190d2c0c3fa8fb5e94e39970cd9453e2819dc8b40ec1`  
		Last Modified: Sat, 19 Mar 2022 00:52:52 GMT  
		Size: 37.0 MB (37013909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77e26b629b7d5ec72075b9db80763d03618483ac484e3129801b1b8131c6fe`  
		Last Modified: Sat, 19 Mar 2022 00:52:45 GMT  
		Size: 2.4 MB (2425472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36be0e7c4d5b1efb3a4be2317e16421a2d536fefec860c776192b0e5447a112`  
		Last Modified: Sat, 19 Mar 2022 00:52:44 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f881f7c1a27e3be051f3f7a6dc8e2234929511ade4258d41308f3b54ac77285`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 11.0 KB (10998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010ed0c2707cfd63880efce177bce0dc0dcb620859f33f8eb2c8661ad10a49e5`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 826.0 KB (826035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e719b3448e3e9cafa84aaabc148a2d7dff4a9270250a65345e20bf35c1c76c37`  
		Last Modified: Sat, 19 Mar 2022 17:51:19 GMT  
		Size: 9.6 MB (9567877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1d97f9f627913a5b6dc23c20ffd479ab36bf7c28953fc4c3b4c0edd429b89`  
		Last Modified: Sat, 19 Mar 2022 17:51:33 GMT  
		Size: 87.6 MB (87553844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5845b747e168c1f1735cafd197dad4457d79ab2f392bd7645e166687392e3da`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4.39`

```console
$ docker pull ghost@sha256:8dbf032df937aee9b24ea5bce598e76560fedfa8a3c3bf9ab53478be8053dd22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:4.39` - linux; amd64

```console
$ docker pull ghost@sha256:7df40e0443f1348977c629d0c6739332c60a93a59a864cf0c059e9081f69b538
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.3 MB (148271097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:669ab852b2633345fef2005c32cf301d19548ef7485faea31af70a7e4fcfd45e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 13:00:01 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 21:50:00 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 21:50:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 21:50:35 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:50:47 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 21:50:47 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:50:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:50:47 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:04:25 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 00:04:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 00:04:43 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:04:44 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 00:05:16 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 00:06:45 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 00:06:47 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 00:06:47 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 00:06:47 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 00:06:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:06:48 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 00:06:48 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bc29d3bc64ca0852101d86667b4a0d1908f05fe0bfead140cf838c0be01bc3`  
		Last Modified: Thu, 17 Mar 2022 13:19:15 GMT  
		Size: 4.2 KB (4183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a71a1d6cc6986624592a148f866355b9b90ddcd4a1f24be36b0f849d8c1044`  
		Last Modified: Fri, 18 Mar 2022 22:14:33 GMT  
		Size: 36.0 MB (36048047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5afd073302f60aad2c5067b89a976a5572fa262d0b60478970f307f8f94b97`  
		Last Modified: Fri, 18 Mar 2022 22:14:27 GMT  
		Size: 2.8 MB (2781848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5878f59eaa39846dd1173083e2e77dc140082be0efc61f7838c3403c6254b113`  
		Last Modified: Fri, 18 Mar 2022 22:14:26 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753aec878444f5bbf5b9e13544f6a3caf78aae1d01d506806f4b342c32623f2a`  
		Last Modified: Sat, 19 Mar 2022 00:09:27 GMT  
		Size: 1.4 MB (1448123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e282a0a274714713330c2ae37bb9aa1be203226d7ffd7de6eec07f2e35270c8`  
		Last Modified: Sat, 19 Mar 2022 00:09:31 GMT  
		Size: 9.6 MB (9567975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6128fb86f0f4e39a32aa4c08d17f607dd59d85e5f88743f9c8e88dd758997be6`  
		Last Modified: Sat, 19 Mar 2022 00:09:44 GMT  
		Size: 67.0 MB (67043352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f7cfac26d6d851aa8ff0c01c9d486dbea8e2db7dc31aa28842be210035fb5`  
		Last Modified: Sat, 19 Mar 2022 00:09:26 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39` - linux; arm variant v7

```console
$ docker pull ghost@sha256:78719e5300fc6838cdfe4fe7bc7b089fcae5c3970dee91fbcbc37e9c6d3c7475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147043059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34fb82b494adf39572f85b07c9779bb0b0724e4e29049dc5ad3404f173ba3abd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 14:47:47 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 22:50:57 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:51:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 22:51:48 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:52:22 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 22:52:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:52:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:52:23 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:22:42 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 23:23:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 23:23:10 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:23:10 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:23:59 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 23:31:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 23:31:50 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 23:31:50 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 23:31:50 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 23:31:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:31:51 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 23:31:52 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c69f71c16ec3df2b7d124845d1b3b6e6495150f4ea3398c32a390afffbf142`  
		Last Modified: Fri, 18 Mar 2022 17:06:49 GMT  
		Size: 4.2 KB (4166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b32ca858e17b62400e3e3939b76745bd091c2302dcb5a659f98f4036c58ad`  
		Last Modified: Sat, 19 Mar 2022 00:07:18 GMT  
		Size: 34.2 MB (34206692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2605fefc93565569e993984be795855508fc11258205a2f0ab736807a40c2c`  
		Last Modified: Sat, 19 Mar 2022 00:06:56 GMT  
		Size: 2.8 MB (2772408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a649abf5b9f938b138570d940f0d8c3af7d265d4e26a25cf69fbd121df9381c`  
		Last Modified: Sat, 19 Mar 2022 00:06:54 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4041d8d2d15b52a58284107ec1fbc633900cce1fc07418607ed52ea1564428aa`  
		Last Modified: Sat, 19 Mar 2022 23:41:13 GMT  
		Size: 1.4 MB (1400322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04c308287b4673d9ba168fbb3d4cec8b9c7e8a9fe4ce8e8bab11f7a83658e18`  
		Last Modified: Sat, 19 Mar 2022 23:41:27 GMT  
		Size: 9.6 MB (9569190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25431520d805b108ecaf6cbf6e20b77e5401b5e75a367d828d99d0a68a2612d0`  
		Last Modified: Sat, 19 Mar 2022 23:42:23 GMT  
		Size: 72.5 MB (72514183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb31846b09f2de8a7bb58d2524fb744ac8124092cd9ee0a6f2ba64f8e8cf782`  
		Last Modified: Sat, 19 Mar 2022 23:41:12 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:f4a663d141c3204ae4bc882b0fc57cb214361f6b4c8bde126b67c24aad420674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154343013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a20e32182de795f606b46f40248f7b94fc474d808fe5fd7d57d6417b85d50fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:20:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 23:50:24 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:50:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 23:50:49 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:51:01 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 23:51:03 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:51:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:51:04 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:41:23 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 17:41:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 17:41:34 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:41:35 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 17:42:09 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 17:42:11 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 17:42:12 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 17:42:13 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 17:45:21 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 17:45:24 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 17:45:26 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 17:45:29 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 17:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:45:34 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 17:45:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e302ce9f0603b4af265c90ba2a4807900c24096808fb68bf44300bd440542`  
		Last Modified: Thu, 17 Mar 2022 13:54:35 GMT  
		Size: 4.0 KB (4042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98badb25d325c02976fab44804955d995b60a19fc609da8e3f1e642c52d898f9`  
		Last Modified: Sat, 19 Mar 2022 00:54:11 GMT  
		Size: 36.2 MB (36154505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5d43df9c11963e4b0e365e779e63981833ea41bdcc5d4db11c675fcc84fab3`  
		Last Modified: Sat, 19 Mar 2022 00:54:06 GMT  
		Size: 2.8 MB (2781278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad002987a7bae850089e45777bc9a362a9f8e3c656bdbbb26980ec4776d4704b`  
		Last Modified: Sat, 19 Mar 2022 00:54:05 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643f6d4797a5cc96449c367b48271ff6c2fdb6908b35b0b9c4c548113d8535a9`  
		Last Modified: Sat, 19 Mar 2022 17:50:44 GMT  
		Size: 1.4 MB (1383662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cde83364d3aeeba3311efa235a8b37ae7bbe49fd46d82e326c8c363b094c82`  
		Last Modified: Sat, 19 Mar 2022 17:50:46 GMT  
		Size: 9.6 MB (9568502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f817e8e904ee939974f5e8f516b174c335682a40a40694832630f3270b0e296`  
		Last Modified: Sat, 19 Mar 2022 17:50:58 GMT  
		Size: 74.4 MB (74387013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d099ce69b402eb198ddea013bbe31fe8ba1a37a42105d092444d276d82d59d61`  
		Last Modified: Sat, 19 Mar 2022 17:50:43 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39` - linux; ppc64le

```console
$ docker pull ghost@sha256:ce8b4d8f9715c7c70c7e6e1746f7535091887d178ca17dc773a8bd7dfb673f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155730905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97937daf1eb28848ecc7f38f97257c3d3573a82441d3c76be44346b51497cc36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 11:17:54 GMT
ADD file:e8555f1cb439a45786b92e929cfa154b51f668c5b4cd69e4ce98340c5998fe0c in / 
# Thu, 17 Mar 2022 11:18:00 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 03:54:03 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 23:06:48 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:11:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 23:11:09 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:14:42 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 23:14:44 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:14:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:14:53 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:46:25 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 23:47:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 23:47:53 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:47:55 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:49:09 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:49:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:49:15 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:49:17 GMT
ENV GHOST_VERSION=4.39.1
# Sun, 20 Mar 2022 00:11:36 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sun, 20 Mar 2022 00:11:46 GMT
WORKDIR /var/lib/ghost
# Sun, 20 Mar 2022 00:11:51 GMT
VOLUME [/var/lib/ghost/content]
# Sun, 20 Mar 2022 00:11:52 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sun, 20 Mar 2022 00:11:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 00:11:59 GMT
EXPOSE 2368
# Sun, 20 Mar 2022 00:12:01 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:aec78dc45d7b3df12df0672d13e22005592b453f03ff2580efac2598dddd680b`  
		Last Modified: Thu, 17 Mar 2022 11:28:17 GMT  
		Size: 35.3 MB (35279758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca53b81b04fce4349fb7d53e6c96231409ea54bc6d07808c393a268d8fcd78c3`  
		Last Modified: Fri, 18 Mar 2022 08:33:21 GMT  
		Size: 4.2 KB (4190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307e188a803758441743ab6c2c16c58d32cd25920f05e601d9fa75c13f8ec1f4`  
		Last Modified: Sat, 19 Mar 2022 02:15:29 GMT  
		Size: 38.0 MB (37978420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6a74008e734f41eb1091af470bca5677108b1eb61729b017bd6e96944fc1c1`  
		Last Modified: Sat, 19 Mar 2022 02:15:22 GMT  
		Size: 2.8 MB (2782569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9e81db75711e347d46105e0daee9e64692433ad3141a1cf1a52bca316993e`  
		Last Modified: Sat, 19 Mar 2022 02:15:22 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d14ae585ca54d978c72b25f6580d1c2986a60f049aefed6a7146e58b8eb07da`  
		Last Modified: Sun, 20 Mar 2022 00:12:26 GMT  
		Size: 1.4 MB (1367834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4904132a0f018373255a9418743ef13604d402190eaf4737c0de15b28964951`  
		Last Modified: Sun, 20 Mar 2022 00:12:31 GMT  
		Size: 9.6 MB (9568608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12320605293f45afa67cc47adf173b0888368bb06886b3b219e3cd4a68fafac`  
		Last Modified: Sun, 20 Mar 2022 00:12:43 GMT  
		Size: 68.7 MB (68748529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270139457a810a99e7dd44848741575b541fe0de273a395f04a5c15fb54ccb23`  
		Last Modified: Sun, 20 Mar 2022 00:12:26 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39` - linux; s390x

```console
$ docker pull ghost@sha256:45b1aa5e819038cf640e167b5a5a4ee3b7b1f8f534b9eef0696dbfe88a14e27c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.5 MB (147499556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a439d42fd5331e4df800fb4597e9eb5c12e1e4aa7a72b029fc59b3b884edd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:50:36 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 22:14:52 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:15:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 22:15:12 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:15:21 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 22:15:21 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:15:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:15:22 GMT
CMD ["node"]
# Sat, 19 Mar 2022 04:38:44 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 04:38:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 04:38:53 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 04:38:53 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 04:39:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 04:39:24 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 04:39:24 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 04:39:25 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 04:42:06 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 04:42:15 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 04:42:15 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 04:42:16 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 04:42:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 04:42:16 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 04:42:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722821cfaf9b99e01207f42d38caa8d0eea9818925d58a5d590057ff6271525d`  
		Last Modified: Thu, 17 Mar 2022 14:21:32 GMT  
		Size: 4.2 KB (4189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924acd2003e404035ae30769a9ed0531c116ccfe4965f354999da4c593b38dc`  
		Last Modified: Fri, 18 Mar 2022 23:10:07 GMT  
		Size: 35.9 MB (35913738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1c92724e1dbac9baa9b4949197499bd94e7abda3f1392dd48cc6f78fb23589`  
		Last Modified: Fri, 18 Mar 2022 23:10:03 GMT  
		Size: 2.8 MB (2782997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f42e3d4bc22c450816fb2255b83b884ec091394d12aff4a84c65c1193e935a`  
		Last Modified: Fri, 18 Mar 2022 23:10:03 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a61fd10dbc4124b4be87498e57bca3e89cab9d50ed7acf9934d6103e2b32eb`  
		Last Modified: Sat, 19 Mar 2022 04:42:48 GMT  
		Size: 1.4 MB (1434956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d6f9332f2c9557e6d14acdf3a51fb916f10fa41d64027309df97ce26b51dbc`  
		Last Modified: Sat, 19 Mar 2022 04:42:49 GMT  
		Size: 9.6 MB (9567431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b22e8969248f953b6c6d82f75ca2021591edf483759ad1672850841c2b90299`  
		Last Modified: Sat, 19 Mar 2022 04:42:59 GMT  
		Size: 68.1 MB (68139455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db7bc896fefc28b64d7f40ca85f1aed46b128fcde04b0748a3ddfe437daa11`  
		Last Modified: Sat, 19 Mar 2022 04:42:47 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4.39-alpine`

```console
$ docker pull ghost@sha256:ef482080ea2121a9bb8d3fd13500cb4efebe814f88c336ca51a8d38ed7c116cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:4.39-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:7fba69cb1b1ab7ab7e22bcaaec6fd1374e7aecf667c734610d9df7c42b93870f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120407221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:847bc2aee68921734b296bc3253f6636fd8eb311b664e6282eb6be1f5f91ea44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 21:48:35 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 21:48:49 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 21:48:49 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:48:55 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 21:48:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:48:56 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:07:05 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 00:07:07 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 00:07:07 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:07:07 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 00:07:34 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 00:08:56 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 00:08:58 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 00:08:58 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 00:08:59 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 00:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:08:59 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 00:08:59 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580248b309d4fecaf2f75f42a36796a166140238395d38d36e0d47b20dded70`  
		Last Modified: Fri, 18 Mar 2022 22:13:15 GMT  
		Size: 37.1 MB (37132855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539902d50a314143ea1ff8b98bee2aae6a9e66b7f102cd5b0ba0b3b21650132e`  
		Last Modified: Fri, 18 Mar 2022 22:13:07 GMT  
		Size: 2.4 MB (2358489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44d60032af439ffa29833ceee54906865bfc7e32949f8a0643d3e1f7307d6e`  
		Last Modified: Fri, 18 Mar 2022 22:13:06 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d799310e8353a5bf7d35c0a576c8cc8a22f423a2268da6c937e55e512240daf`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 11.2 KB (11209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c87a58ecffcb615b1c9af4968b84fdfb44fd7f432d7d7c6087a14f7ba7f201e`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 816.9 KB (816859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf689cb927dd935805d71b57cb514cc956df63b009fc1453a79c668d2dad985d`  
		Last Modified: Sat, 19 Mar 2022 00:10:04 GMT  
		Size: 9.6 MB (9567883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b38a95a7d42f2ed48ffada1b7b31d395594b24e4b51d8eef0ddf93afe6b8595`  
		Last Modified: Sat, 19 Mar 2022 00:10:17 GMT  
		Size: 67.7 MB (67702755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddb7f12b2dcac2bc19d55fffdc3e5ada0a10ab45407f0e313834954f852e2b0`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:6108db40dd7418795073f3d3bfd9fe0366cbd252d11bef46e6dbad514176d85e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121612527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5444505489f48c5995f748bb4d4bce479dc4e9eb1d995986a6fa7455bf9886c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 19:31:23 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 19:47:55 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 19:47:56 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 19:48:04 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 19:48:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 19:48:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 19:48:06 GMT
CMD ["node"]
# Fri, 18 Mar 2022 21:05:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 18 Mar 2022 21:05:06 GMT
RUN apk add --no-cache 		bash
# Fri, 18 Mar 2022 21:05:06 GMT
ENV NODE_ENV=production
# Fri, 18 Mar 2022 21:05:06 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Fri, 18 Mar 2022 21:06:20 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 18 Mar 2022 21:06:21 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 18 Mar 2022 21:06:22 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 18 Mar 2022 21:06:22 GMT
ENV GHOST_VERSION=4.39.1
# Fri, 18 Mar 2022 21:16:25 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 18 Mar 2022 21:16:29 GMT
WORKDIR /var/lib/ghost
# Fri, 18 Mar 2022 21:16:29 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 18 Mar 2022 21:16:30 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 18 Mar 2022 21:16:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:16:32 GMT
EXPOSE 2368
# Fri, 18 Mar 2022 21:16:33 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd48496521270c1ba2c1d855bd715f617b59d6498e2e407b804b566b7678087`  
		Last Modified: Fri, 18 Mar 2022 20:47:14 GMT  
		Size: 36.2 MB (36198526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5599fde36163c1ebda1ad804a5b327cc1609b46263a91060b9fc3a835d328be9`  
		Last Modified: Fri, 18 Mar 2022 20:47:01 GMT  
		Size: 2.4 MB (2418192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18709050207fe0cf4803ac4f14090c67a8729cd62b866e31ae708d3b6e7b9166`  
		Last Modified: Fri, 18 Mar 2022 20:46:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af606d946314fedea65ebbae67cbd1cecf6a786558facb4b88f3f5739e15c45b`  
		Last Modified: Fri, 18 Mar 2022 21:17:09 GMT  
		Size: 11.0 KB (10977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0954b81f1ae01a7d7b8339d694eef033a3a078ca6a23c44e8934eb1c6229c0`  
		Last Modified: Fri, 18 Mar 2022 21:17:10 GMT  
		Size: 771.0 KB (770953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455c516cdd5fda37a751a4a4b7ef0e58ecb18b7c3fb786fb1f485daa97406bee`  
		Last Modified: Fri, 18 Mar 2022 21:17:19 GMT  
		Size: 9.6 MB (9569616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8e836532b22085f33122bfa92e57f9b6cb7f6679237f396b7493ac9a1c5833`  
		Last Modified: Fri, 18 Mar 2022 21:17:55 GMT  
		Size: 70.0 MB (70013905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece8cd2cd02390a0b0e5b514593ce36f25efaab79f731bbf280d80f1450a7d01`  
		Last Modified: Fri, 18 Mar 2022 21:17:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:ce4864a56a2ec745d71119586a3a6ead3bb50b57952c003eb737d823fee66c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120368095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a90bb3b146463403b2cb1d5e44a034d0bd3a9e5c2c31efdf31f6f4b48d62f36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 17:21:06 GMT
ADD file:c25fcf153ea349f64e08a1bd0756ce550f2a081ad56cc40c89027d85d1bc26da in / 
# Thu, 17 Mar 2022 17:21:06 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 22:22:50 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:36:08 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 22:36:09 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:36:16 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 22:36:17 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:36:18 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:32:10 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 23:32:12 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 23:32:13 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:32:13 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:33:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:33:06 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:33:07 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:33:07 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 23:40:19 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 23:40:22 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 23:40:23 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 23:40:23 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 23:40:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:40:24 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 23:40:25 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c3a1157c36d8d156f7664fa098212ab2149a64bcb59767cdf4595a86617c17fd`  
		Last Modified: Thu, 17 Mar 2022 17:22:45 GMT  
		Size: 2.4 MB (2430456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7fb7593e1ec2c0060c773dbbf85fcbe77df0a45cbc891cd7f775442f959ce6`  
		Last Modified: Sat, 19 Mar 2022 00:04:50 GMT  
		Size: 35.8 MB (35750941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b531d0f3fa4a8c1e5c8c32c0c6a9de8cda1e078ed43db62853858f7ef792044b`  
		Last Modified: Sat, 19 Mar 2022 00:04:27 GMT  
		Size: 2.4 MB (2418360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ead18221dfbeb2afd1c7044892b00c01b6b056d5feb01c74684dff97d67e8eb`  
		Last Modified: Sat, 19 Mar 2022 00:04:26 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1faeeef23a40a6e07406285a95e3f94a86314cef806a54bbf3e2672288624dc`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 10.8 KB (10772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41729cace1ddd94023eba72c5c881b17ee1ab0e939be1d113c4f144fdae876c1`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 703.9 KB (703890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1f8edf6ec39144c3fa34019e53bf9892978c935ab4b45e035f61c9cd7e32b`  
		Last Modified: Sat, 19 Mar 2022 23:42:57 GMT  
		Size: 9.6 MB (9569052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8628b5b59160ec4766d80912273c9024695381f2b717407a91177b03925b4dd9`  
		Last Modified: Sat, 19 Mar 2022 23:43:56 GMT  
		Size: 69.5 MB (69483628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678ef4fd7c46697fe04cca3f1ecc814f51b56a03ea9abb66a3c1fb7c22093eb6`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:4f35663f73dfc11751365716b7d6a9d08e66e2cd0b7b6d6d276e9167c66dbe21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140115021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b197627739a94af9bff95a19a902e84b7a352936df176d8b8dc38f329a3c9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 23:07:29 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:28:15 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 23:28:15 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:28:21 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 23:28:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:28:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:28:23 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:45:45 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 17:45:47 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 17:45:47 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:45:48 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 17:46:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 17:46:27 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 17:46:28 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 17:46:29 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 17:49:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 17:49:59 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 17:50:01 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 17:50:04 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 17:50:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:50:08 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 17:50:11 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c992e90d8c9f9d1552190d2c0c3fa8fb5e94e39970cd9453e2819dc8b40ec1`  
		Last Modified: Sat, 19 Mar 2022 00:52:52 GMT  
		Size: 37.0 MB (37013909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77e26b629b7d5ec72075b9db80763d03618483ac484e3129801b1b8131c6fe`  
		Last Modified: Sat, 19 Mar 2022 00:52:45 GMT  
		Size: 2.4 MB (2425472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36be0e7c4d5b1efb3a4be2317e16421a2d536fefec860c776192b0e5447a112`  
		Last Modified: Sat, 19 Mar 2022 00:52:44 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f881f7c1a27e3be051f3f7a6dc8e2234929511ade4258d41308f3b54ac77285`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 11.0 KB (10998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010ed0c2707cfd63880efce177bce0dc0dcb620859f33f8eb2c8661ad10a49e5`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 826.0 KB (826035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e719b3448e3e9cafa84aaabc148a2d7dff4a9270250a65345e20bf35c1c76c37`  
		Last Modified: Sat, 19 Mar 2022 17:51:19 GMT  
		Size: 9.6 MB (9567877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1d97f9f627913a5b6dc23c20ffd479ab36bf7c28953fc4c3b4c0edd429b89`  
		Last Modified: Sat, 19 Mar 2022 17:51:33 GMT  
		Size: 87.6 MB (87553844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5845b747e168c1f1735cafd197dad4457d79ab2f392bd7645e166687392e3da`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4.39.1`

```console
$ docker pull ghost@sha256:8dbf032df937aee9b24ea5bce598e76560fedfa8a3c3bf9ab53478be8053dd22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:4.39.1` - linux; amd64

```console
$ docker pull ghost@sha256:7df40e0443f1348977c629d0c6739332c60a93a59a864cf0c059e9081f69b538
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.3 MB (148271097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:669ab852b2633345fef2005c32cf301d19548ef7485faea31af70a7e4fcfd45e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 13:00:01 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 21:50:00 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 21:50:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 21:50:35 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:50:47 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 21:50:47 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:50:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:50:47 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:04:25 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 00:04:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 00:04:43 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:04:44 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 00:05:16 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 00:06:45 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 00:06:47 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 00:06:47 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 00:06:47 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 00:06:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:06:48 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 00:06:48 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bc29d3bc64ca0852101d86667b4a0d1908f05fe0bfead140cf838c0be01bc3`  
		Last Modified: Thu, 17 Mar 2022 13:19:15 GMT  
		Size: 4.2 KB (4183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a71a1d6cc6986624592a148f866355b9b90ddcd4a1f24be36b0f849d8c1044`  
		Last Modified: Fri, 18 Mar 2022 22:14:33 GMT  
		Size: 36.0 MB (36048047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5afd073302f60aad2c5067b89a976a5572fa262d0b60478970f307f8f94b97`  
		Last Modified: Fri, 18 Mar 2022 22:14:27 GMT  
		Size: 2.8 MB (2781848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5878f59eaa39846dd1173083e2e77dc140082be0efc61f7838c3403c6254b113`  
		Last Modified: Fri, 18 Mar 2022 22:14:26 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753aec878444f5bbf5b9e13544f6a3caf78aae1d01d506806f4b342c32623f2a`  
		Last Modified: Sat, 19 Mar 2022 00:09:27 GMT  
		Size: 1.4 MB (1448123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e282a0a274714713330c2ae37bb9aa1be203226d7ffd7de6eec07f2e35270c8`  
		Last Modified: Sat, 19 Mar 2022 00:09:31 GMT  
		Size: 9.6 MB (9567975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6128fb86f0f4e39a32aa4c08d17f607dd59d85e5f88743f9c8e88dd758997be6`  
		Last Modified: Sat, 19 Mar 2022 00:09:44 GMT  
		Size: 67.0 MB (67043352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f7cfac26d6d851aa8ff0c01c9d486dbea8e2db7dc31aa28842be210035fb5`  
		Last Modified: Sat, 19 Mar 2022 00:09:26 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39.1` - linux; arm variant v7

```console
$ docker pull ghost@sha256:78719e5300fc6838cdfe4fe7bc7b089fcae5c3970dee91fbcbc37e9c6d3c7475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147043059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34fb82b494adf39572f85b07c9779bb0b0724e4e29049dc5ad3404f173ba3abd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 14:47:47 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 22:50:57 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:51:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 22:51:48 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:52:22 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 22:52:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:52:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:52:23 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:22:42 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 23:23:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 23:23:10 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:23:10 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:23:59 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 23:31:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 23:31:50 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 23:31:50 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 23:31:50 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 23:31:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:31:51 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 23:31:52 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c69f71c16ec3df2b7d124845d1b3b6e6495150f4ea3398c32a390afffbf142`  
		Last Modified: Fri, 18 Mar 2022 17:06:49 GMT  
		Size: 4.2 KB (4166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b32ca858e17b62400e3e3939b76745bd091c2302dcb5a659f98f4036c58ad`  
		Last Modified: Sat, 19 Mar 2022 00:07:18 GMT  
		Size: 34.2 MB (34206692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2605fefc93565569e993984be795855508fc11258205a2f0ab736807a40c2c`  
		Last Modified: Sat, 19 Mar 2022 00:06:56 GMT  
		Size: 2.8 MB (2772408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a649abf5b9f938b138570d940f0d8c3af7d265d4e26a25cf69fbd121df9381c`  
		Last Modified: Sat, 19 Mar 2022 00:06:54 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4041d8d2d15b52a58284107ec1fbc633900cce1fc07418607ed52ea1564428aa`  
		Last Modified: Sat, 19 Mar 2022 23:41:13 GMT  
		Size: 1.4 MB (1400322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04c308287b4673d9ba168fbb3d4cec8b9c7e8a9fe4ce8e8bab11f7a83658e18`  
		Last Modified: Sat, 19 Mar 2022 23:41:27 GMT  
		Size: 9.6 MB (9569190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25431520d805b108ecaf6cbf6e20b77e5401b5e75a367d828d99d0a68a2612d0`  
		Last Modified: Sat, 19 Mar 2022 23:42:23 GMT  
		Size: 72.5 MB (72514183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb31846b09f2de8a7bb58d2524fb744ac8124092cd9ee0a6f2ba64f8e8cf782`  
		Last Modified: Sat, 19 Mar 2022 23:41:12 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39.1` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:f4a663d141c3204ae4bc882b0fc57cb214361f6b4c8bde126b67c24aad420674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154343013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a20e32182de795f606b46f40248f7b94fc474d808fe5fd7d57d6417b85d50fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:20:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 23:50:24 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:50:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 23:50:49 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:51:01 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 23:51:03 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:51:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:51:04 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:41:23 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 17:41:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 17:41:34 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:41:35 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 17:42:09 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 17:42:11 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 17:42:12 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 17:42:13 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 17:45:21 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 17:45:24 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 17:45:26 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 17:45:29 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 17:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:45:34 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 17:45:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e302ce9f0603b4af265c90ba2a4807900c24096808fb68bf44300bd440542`  
		Last Modified: Thu, 17 Mar 2022 13:54:35 GMT  
		Size: 4.0 KB (4042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98badb25d325c02976fab44804955d995b60a19fc609da8e3f1e642c52d898f9`  
		Last Modified: Sat, 19 Mar 2022 00:54:11 GMT  
		Size: 36.2 MB (36154505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5d43df9c11963e4b0e365e779e63981833ea41bdcc5d4db11c675fcc84fab3`  
		Last Modified: Sat, 19 Mar 2022 00:54:06 GMT  
		Size: 2.8 MB (2781278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad002987a7bae850089e45777bc9a362a9f8e3c656bdbbb26980ec4776d4704b`  
		Last Modified: Sat, 19 Mar 2022 00:54:05 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643f6d4797a5cc96449c367b48271ff6c2fdb6908b35b0b9c4c548113d8535a9`  
		Last Modified: Sat, 19 Mar 2022 17:50:44 GMT  
		Size: 1.4 MB (1383662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cde83364d3aeeba3311efa235a8b37ae7bbe49fd46d82e326c8c363b094c82`  
		Last Modified: Sat, 19 Mar 2022 17:50:46 GMT  
		Size: 9.6 MB (9568502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f817e8e904ee939974f5e8f516b174c335682a40a40694832630f3270b0e296`  
		Last Modified: Sat, 19 Mar 2022 17:50:58 GMT  
		Size: 74.4 MB (74387013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d099ce69b402eb198ddea013bbe31fe8ba1a37a42105d092444d276d82d59d61`  
		Last Modified: Sat, 19 Mar 2022 17:50:43 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39.1` - linux; ppc64le

```console
$ docker pull ghost@sha256:ce8b4d8f9715c7c70c7e6e1746f7535091887d178ca17dc773a8bd7dfb673f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155730905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97937daf1eb28848ecc7f38f97257c3d3573a82441d3c76be44346b51497cc36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 11:17:54 GMT
ADD file:e8555f1cb439a45786b92e929cfa154b51f668c5b4cd69e4ce98340c5998fe0c in / 
# Thu, 17 Mar 2022 11:18:00 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 03:54:03 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 23:06:48 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:11:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 23:11:09 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:14:42 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 23:14:44 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:14:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:14:53 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:46:25 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 23:47:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 23:47:53 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:47:55 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:49:09 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:49:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:49:15 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:49:17 GMT
ENV GHOST_VERSION=4.39.1
# Sun, 20 Mar 2022 00:11:36 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sun, 20 Mar 2022 00:11:46 GMT
WORKDIR /var/lib/ghost
# Sun, 20 Mar 2022 00:11:51 GMT
VOLUME [/var/lib/ghost/content]
# Sun, 20 Mar 2022 00:11:52 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sun, 20 Mar 2022 00:11:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 00:11:59 GMT
EXPOSE 2368
# Sun, 20 Mar 2022 00:12:01 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:aec78dc45d7b3df12df0672d13e22005592b453f03ff2580efac2598dddd680b`  
		Last Modified: Thu, 17 Mar 2022 11:28:17 GMT  
		Size: 35.3 MB (35279758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca53b81b04fce4349fb7d53e6c96231409ea54bc6d07808c393a268d8fcd78c3`  
		Last Modified: Fri, 18 Mar 2022 08:33:21 GMT  
		Size: 4.2 KB (4190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307e188a803758441743ab6c2c16c58d32cd25920f05e601d9fa75c13f8ec1f4`  
		Last Modified: Sat, 19 Mar 2022 02:15:29 GMT  
		Size: 38.0 MB (37978420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6a74008e734f41eb1091af470bca5677108b1eb61729b017bd6e96944fc1c1`  
		Last Modified: Sat, 19 Mar 2022 02:15:22 GMT  
		Size: 2.8 MB (2782569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9e81db75711e347d46105e0daee9e64692433ad3141a1cf1a52bca316993e`  
		Last Modified: Sat, 19 Mar 2022 02:15:22 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d14ae585ca54d978c72b25f6580d1c2986a60f049aefed6a7146e58b8eb07da`  
		Last Modified: Sun, 20 Mar 2022 00:12:26 GMT  
		Size: 1.4 MB (1367834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4904132a0f018373255a9418743ef13604d402190eaf4737c0de15b28964951`  
		Last Modified: Sun, 20 Mar 2022 00:12:31 GMT  
		Size: 9.6 MB (9568608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12320605293f45afa67cc47adf173b0888368bb06886b3b219e3cd4a68fafac`  
		Last Modified: Sun, 20 Mar 2022 00:12:43 GMT  
		Size: 68.7 MB (68748529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270139457a810a99e7dd44848741575b541fe0de273a395f04a5c15fb54ccb23`  
		Last Modified: Sun, 20 Mar 2022 00:12:26 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39.1` - linux; s390x

```console
$ docker pull ghost@sha256:45b1aa5e819038cf640e167b5a5a4ee3b7b1f8f534b9eef0696dbfe88a14e27c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.5 MB (147499556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a439d42fd5331e4df800fb4597e9eb5c12e1e4aa7a72b029fc59b3b884edd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:50:36 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 22:14:52 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:15:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 22:15:12 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:15:21 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 22:15:21 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:15:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:15:22 GMT
CMD ["node"]
# Sat, 19 Mar 2022 04:38:44 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 04:38:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 04:38:53 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 04:38:53 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 04:39:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 04:39:24 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 04:39:24 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 04:39:25 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 04:42:06 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 04:42:15 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 04:42:15 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 04:42:16 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 04:42:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 04:42:16 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 04:42:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722821cfaf9b99e01207f42d38caa8d0eea9818925d58a5d590057ff6271525d`  
		Last Modified: Thu, 17 Mar 2022 14:21:32 GMT  
		Size: 4.2 KB (4189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924acd2003e404035ae30769a9ed0531c116ccfe4965f354999da4c593b38dc`  
		Last Modified: Fri, 18 Mar 2022 23:10:07 GMT  
		Size: 35.9 MB (35913738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1c92724e1dbac9baa9b4949197499bd94e7abda3f1392dd48cc6f78fb23589`  
		Last Modified: Fri, 18 Mar 2022 23:10:03 GMT  
		Size: 2.8 MB (2782997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f42e3d4bc22c450816fb2255b83b884ec091394d12aff4a84c65c1193e935a`  
		Last Modified: Fri, 18 Mar 2022 23:10:03 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a61fd10dbc4124b4be87498e57bca3e89cab9d50ed7acf9934d6103e2b32eb`  
		Last Modified: Sat, 19 Mar 2022 04:42:48 GMT  
		Size: 1.4 MB (1434956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d6f9332f2c9557e6d14acdf3a51fb916f10fa41d64027309df97ce26b51dbc`  
		Last Modified: Sat, 19 Mar 2022 04:42:49 GMT  
		Size: 9.6 MB (9567431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b22e8969248f953b6c6d82f75ca2021591edf483759ad1672850841c2b90299`  
		Last Modified: Sat, 19 Mar 2022 04:42:59 GMT  
		Size: 68.1 MB (68139455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db7bc896fefc28b64d7f40ca85f1aed46b128fcde04b0748a3ddfe437daa11`  
		Last Modified: Sat, 19 Mar 2022 04:42:47 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4.39.1-alpine`

```console
$ docker pull ghost@sha256:ef482080ea2121a9bb8d3fd13500cb4efebe814f88c336ca51a8d38ed7c116cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:4.39.1-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:7fba69cb1b1ab7ab7e22bcaaec6fd1374e7aecf667c734610d9df7c42b93870f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120407221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:847bc2aee68921734b296bc3253f6636fd8eb311b664e6282eb6be1f5f91ea44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 21:48:35 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 21:48:49 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 21:48:49 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:48:55 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 21:48:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:48:56 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:07:05 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 00:07:07 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 00:07:07 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:07:07 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 00:07:34 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 00:08:56 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 00:08:58 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 00:08:58 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 00:08:59 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 00:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:08:59 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 00:08:59 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580248b309d4fecaf2f75f42a36796a166140238395d38d36e0d47b20dded70`  
		Last Modified: Fri, 18 Mar 2022 22:13:15 GMT  
		Size: 37.1 MB (37132855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539902d50a314143ea1ff8b98bee2aae6a9e66b7f102cd5b0ba0b3b21650132e`  
		Last Modified: Fri, 18 Mar 2022 22:13:07 GMT  
		Size: 2.4 MB (2358489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44d60032af439ffa29833ceee54906865bfc7e32949f8a0643d3e1f7307d6e`  
		Last Modified: Fri, 18 Mar 2022 22:13:06 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d799310e8353a5bf7d35c0a576c8cc8a22f423a2268da6c937e55e512240daf`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 11.2 KB (11209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c87a58ecffcb615b1c9af4968b84fdfb44fd7f432d7d7c6087a14f7ba7f201e`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 816.9 KB (816859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf689cb927dd935805d71b57cb514cc956df63b009fc1453a79c668d2dad985d`  
		Last Modified: Sat, 19 Mar 2022 00:10:04 GMT  
		Size: 9.6 MB (9567883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b38a95a7d42f2ed48ffada1b7b31d395594b24e4b51d8eef0ddf93afe6b8595`  
		Last Modified: Sat, 19 Mar 2022 00:10:17 GMT  
		Size: 67.7 MB (67702755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddb7f12b2dcac2bc19d55fffdc3e5ada0a10ab45407f0e313834954f852e2b0`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39.1-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:6108db40dd7418795073f3d3bfd9fe0366cbd252d11bef46e6dbad514176d85e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121612527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5444505489f48c5995f748bb4d4bce479dc4e9eb1d995986a6fa7455bf9886c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 19:31:23 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 19:47:55 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 19:47:56 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 19:48:04 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 19:48:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 19:48:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 19:48:06 GMT
CMD ["node"]
# Fri, 18 Mar 2022 21:05:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 18 Mar 2022 21:05:06 GMT
RUN apk add --no-cache 		bash
# Fri, 18 Mar 2022 21:05:06 GMT
ENV NODE_ENV=production
# Fri, 18 Mar 2022 21:05:06 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Fri, 18 Mar 2022 21:06:20 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 18 Mar 2022 21:06:21 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 18 Mar 2022 21:06:22 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 18 Mar 2022 21:06:22 GMT
ENV GHOST_VERSION=4.39.1
# Fri, 18 Mar 2022 21:16:25 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 18 Mar 2022 21:16:29 GMT
WORKDIR /var/lib/ghost
# Fri, 18 Mar 2022 21:16:29 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 18 Mar 2022 21:16:30 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 18 Mar 2022 21:16:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:16:32 GMT
EXPOSE 2368
# Fri, 18 Mar 2022 21:16:33 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd48496521270c1ba2c1d855bd715f617b59d6498e2e407b804b566b7678087`  
		Last Modified: Fri, 18 Mar 2022 20:47:14 GMT  
		Size: 36.2 MB (36198526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5599fde36163c1ebda1ad804a5b327cc1609b46263a91060b9fc3a835d328be9`  
		Last Modified: Fri, 18 Mar 2022 20:47:01 GMT  
		Size: 2.4 MB (2418192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18709050207fe0cf4803ac4f14090c67a8729cd62b866e31ae708d3b6e7b9166`  
		Last Modified: Fri, 18 Mar 2022 20:46:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af606d946314fedea65ebbae67cbd1cecf6a786558facb4b88f3f5739e15c45b`  
		Last Modified: Fri, 18 Mar 2022 21:17:09 GMT  
		Size: 11.0 KB (10977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0954b81f1ae01a7d7b8339d694eef033a3a078ca6a23c44e8934eb1c6229c0`  
		Last Modified: Fri, 18 Mar 2022 21:17:10 GMT  
		Size: 771.0 KB (770953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455c516cdd5fda37a751a4a4b7ef0e58ecb18b7c3fb786fb1f485daa97406bee`  
		Last Modified: Fri, 18 Mar 2022 21:17:19 GMT  
		Size: 9.6 MB (9569616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8e836532b22085f33122bfa92e57f9b6cb7f6679237f396b7493ac9a1c5833`  
		Last Modified: Fri, 18 Mar 2022 21:17:55 GMT  
		Size: 70.0 MB (70013905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece8cd2cd02390a0b0e5b514593ce36f25efaab79f731bbf280d80f1450a7d01`  
		Last Modified: Fri, 18 Mar 2022 21:17:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39.1-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:ce4864a56a2ec745d71119586a3a6ead3bb50b57952c003eb737d823fee66c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120368095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a90bb3b146463403b2cb1d5e44a034d0bd3a9e5c2c31efdf31f6f4b48d62f36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 17:21:06 GMT
ADD file:c25fcf153ea349f64e08a1bd0756ce550f2a081ad56cc40c89027d85d1bc26da in / 
# Thu, 17 Mar 2022 17:21:06 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 22:22:50 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:36:08 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 22:36:09 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:36:16 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 22:36:17 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:36:18 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:32:10 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 23:32:12 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 23:32:13 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:32:13 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:33:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:33:06 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:33:07 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:33:07 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 23:40:19 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 23:40:22 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 23:40:23 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 23:40:23 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 23:40:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:40:24 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 23:40:25 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c3a1157c36d8d156f7664fa098212ab2149a64bcb59767cdf4595a86617c17fd`  
		Last Modified: Thu, 17 Mar 2022 17:22:45 GMT  
		Size: 2.4 MB (2430456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7fb7593e1ec2c0060c773dbbf85fcbe77df0a45cbc891cd7f775442f959ce6`  
		Last Modified: Sat, 19 Mar 2022 00:04:50 GMT  
		Size: 35.8 MB (35750941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b531d0f3fa4a8c1e5c8c32c0c6a9de8cda1e078ed43db62853858f7ef792044b`  
		Last Modified: Sat, 19 Mar 2022 00:04:27 GMT  
		Size: 2.4 MB (2418360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ead18221dfbeb2afd1c7044892b00c01b6b056d5feb01c74684dff97d67e8eb`  
		Last Modified: Sat, 19 Mar 2022 00:04:26 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1faeeef23a40a6e07406285a95e3f94a86314cef806a54bbf3e2672288624dc`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 10.8 KB (10772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41729cace1ddd94023eba72c5c881b17ee1ab0e939be1d113c4f144fdae876c1`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 703.9 KB (703890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1f8edf6ec39144c3fa34019e53bf9892978c935ab4b45e035f61c9cd7e32b`  
		Last Modified: Sat, 19 Mar 2022 23:42:57 GMT  
		Size: 9.6 MB (9569052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8628b5b59160ec4766d80912273c9024695381f2b717407a91177b03925b4dd9`  
		Last Modified: Sat, 19 Mar 2022 23:43:56 GMT  
		Size: 69.5 MB (69483628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678ef4fd7c46697fe04cca3f1ecc814f51b56a03ea9abb66a3c1fb7c22093eb6`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.39.1-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:4f35663f73dfc11751365716b7d6a9d08e66e2cd0b7b6d6d276e9167c66dbe21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140115021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b197627739a94af9bff95a19a902e84b7a352936df176d8b8dc38f329a3c9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 23:07:29 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:28:15 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 23:28:15 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:28:21 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 23:28:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:28:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:28:23 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:45:45 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 17:45:47 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 17:45:47 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:45:48 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 17:46:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 17:46:27 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 17:46:28 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 17:46:29 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 17:49:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 17:49:59 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 17:50:01 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 17:50:04 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 17:50:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:50:08 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 17:50:11 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c992e90d8c9f9d1552190d2c0c3fa8fb5e94e39970cd9453e2819dc8b40ec1`  
		Last Modified: Sat, 19 Mar 2022 00:52:52 GMT  
		Size: 37.0 MB (37013909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77e26b629b7d5ec72075b9db80763d03618483ac484e3129801b1b8131c6fe`  
		Last Modified: Sat, 19 Mar 2022 00:52:45 GMT  
		Size: 2.4 MB (2425472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36be0e7c4d5b1efb3a4be2317e16421a2d536fefec860c776192b0e5447a112`  
		Last Modified: Sat, 19 Mar 2022 00:52:44 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f881f7c1a27e3be051f3f7a6dc8e2234929511ade4258d41308f3b54ac77285`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 11.0 KB (10998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010ed0c2707cfd63880efce177bce0dc0dcb620859f33f8eb2c8661ad10a49e5`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 826.0 KB (826035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e719b3448e3e9cafa84aaabc148a2d7dff4a9270250a65345e20bf35c1c76c37`  
		Last Modified: Sat, 19 Mar 2022 17:51:19 GMT  
		Size: 9.6 MB (9567877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1d97f9f627913a5b6dc23c20ffd479ab36bf7c28953fc4c3b4c0edd429b89`  
		Last Modified: Sat, 19 Mar 2022 17:51:33 GMT  
		Size: 87.6 MB (87553844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5845b747e168c1f1735cafd197dad4457d79ab2f392bd7645e166687392e3da`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:alpine`

```console
$ docker pull ghost@sha256:ef482080ea2121a9bb8d3fd13500cb4efebe814f88c336ca51a8d38ed7c116cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:alpine` - linux; amd64

```console
$ docker pull ghost@sha256:7fba69cb1b1ab7ab7e22bcaaec6fd1374e7aecf667c734610d9df7c42b93870f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120407221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:847bc2aee68921734b296bc3253f6636fd8eb311b664e6282eb6be1f5f91ea44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 21:48:35 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 21:48:49 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 21:48:49 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:48:55 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 21:48:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:48:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:48:56 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:07:05 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 00:07:07 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 00:07:07 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:07:07 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 00:07:34 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 00:07:35 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 00:08:56 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 00:08:58 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 00:08:58 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 00:08:59 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 00:08:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:08:59 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 00:08:59 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0580248b309d4fecaf2f75f42a36796a166140238395d38d36e0d47b20dded70`  
		Last Modified: Fri, 18 Mar 2022 22:13:15 GMT  
		Size: 37.1 MB (37132855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539902d50a314143ea1ff8b98bee2aae6a9e66b7f102cd5b0ba0b3b21650132e`  
		Last Modified: Fri, 18 Mar 2022 22:13:07 GMT  
		Size: 2.4 MB (2358489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44d60032af439ffa29833ceee54906865bfc7e32949f8a0643d3e1f7307d6e`  
		Last Modified: Fri, 18 Mar 2022 22:13:06 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d799310e8353a5bf7d35c0a576c8cc8a22f423a2268da6c937e55e512240daf`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 11.2 KB (11209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c87a58ecffcb615b1c9af4968b84fdfb44fd7f432d7d7c6087a14f7ba7f201e`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 816.9 KB (816859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf689cb927dd935805d71b57cb514cc956df63b009fc1453a79c668d2dad985d`  
		Last Modified: Sat, 19 Mar 2022 00:10:04 GMT  
		Size: 9.6 MB (9567883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b38a95a7d42f2ed48ffada1b7b31d395594b24e4b51d8eef0ddf93afe6b8595`  
		Last Modified: Sat, 19 Mar 2022 00:10:17 GMT  
		Size: 67.7 MB (67702755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddb7f12b2dcac2bc19d55fffdc3e5ada0a10ab45407f0e313834954f852e2b0`  
		Last Modified: Sat, 19 Mar 2022 00:10:01 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:6108db40dd7418795073f3d3bfd9fe0366cbd252d11bef46e6dbad514176d85e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121612527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5444505489f48c5995f748bb4d4bce479dc4e9eb1d995986a6fa7455bf9886c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:33 GMT
ADD file:8f1611b9334907a82945fdb21e17ee41541ab95050fc199c60fca662759171a5 in / 
# Thu, 17 Mar 2022 14:32:33 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 19:31:23 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 19:47:55 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 19:47:56 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 19:48:04 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 19:48:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 19:48:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 19:48:06 GMT
CMD ["node"]
# Fri, 18 Mar 2022 21:05:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 18 Mar 2022 21:05:06 GMT
RUN apk add --no-cache 		bash
# Fri, 18 Mar 2022 21:05:06 GMT
ENV NODE_ENV=production
# Fri, 18 Mar 2022 21:05:06 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Fri, 18 Mar 2022 21:06:20 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 18 Mar 2022 21:06:21 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 18 Mar 2022 21:06:22 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 18 Mar 2022 21:06:22 GMT
ENV GHOST_VERSION=4.39.1
# Fri, 18 Mar 2022 21:16:25 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 18 Mar 2022 21:16:29 GMT
WORKDIR /var/lib/ghost
# Fri, 18 Mar 2022 21:16:29 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 18 Mar 2022 21:16:30 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 18 Mar 2022 21:16:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:16:32 GMT
EXPOSE 2368
# Fri, 18 Mar 2022 21:16:33 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:4025825e6ef43541c3a3e1ecb0092bc1b098e792051c7e338d6da54f66b19661`  
		Last Modified: Thu, 17 Mar 2022 14:34:09 GMT  
		Size: 2.6 MB (2629364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd48496521270c1ba2c1d855bd715f617b59d6498e2e407b804b566b7678087`  
		Last Modified: Fri, 18 Mar 2022 20:47:14 GMT  
		Size: 36.2 MB (36198526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5599fde36163c1ebda1ad804a5b327cc1609b46263a91060b9fc3a835d328be9`  
		Last Modified: Fri, 18 Mar 2022 20:47:01 GMT  
		Size: 2.4 MB (2418192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18709050207fe0cf4803ac4f14090c67a8729cd62b866e31ae708d3b6e7b9166`  
		Last Modified: Fri, 18 Mar 2022 20:46:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af606d946314fedea65ebbae67cbd1cecf6a786558facb4b88f3f5739e15c45b`  
		Last Modified: Fri, 18 Mar 2022 21:17:09 GMT  
		Size: 11.0 KB (10977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0954b81f1ae01a7d7b8339d694eef033a3a078ca6a23c44e8934eb1c6229c0`  
		Last Modified: Fri, 18 Mar 2022 21:17:10 GMT  
		Size: 771.0 KB (770953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455c516cdd5fda37a751a4a4b7ef0e58ecb18b7c3fb786fb1f485daa97406bee`  
		Last Modified: Fri, 18 Mar 2022 21:17:19 GMT  
		Size: 9.6 MB (9569616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8e836532b22085f33122bfa92e57f9b6cb7f6679237f396b7493ac9a1c5833`  
		Last Modified: Fri, 18 Mar 2022 21:17:55 GMT  
		Size: 70.0 MB (70013905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece8cd2cd02390a0b0e5b514593ce36f25efaab79f731bbf280d80f1450a7d01`  
		Last Modified: Fri, 18 Mar 2022 21:17:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:ce4864a56a2ec745d71119586a3a6ead3bb50b57952c003eb737d823fee66c5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120368095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a90bb3b146463403b2cb1d5e44a034d0bd3a9e5c2c31efdf31f6f4b48d62f36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 17:21:06 GMT
ADD file:c25fcf153ea349f64e08a1bd0756ce550f2a081ad56cc40c89027d85d1bc26da in / 
# Thu, 17 Mar 2022 17:21:06 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 22:22:50 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:36:08 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 22:36:09 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:36:16 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 22:36:17 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:36:18 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:32:10 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 23:32:12 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 23:32:13 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:32:13 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:33:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:33:06 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:33:07 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:33:07 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 23:40:19 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 23:40:22 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 23:40:23 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 23:40:23 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 23:40:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:40:24 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 23:40:25 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c3a1157c36d8d156f7664fa098212ab2149a64bcb59767cdf4595a86617c17fd`  
		Last Modified: Thu, 17 Mar 2022 17:22:45 GMT  
		Size: 2.4 MB (2430456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7fb7593e1ec2c0060c773dbbf85fcbe77df0a45cbc891cd7f775442f959ce6`  
		Last Modified: Sat, 19 Mar 2022 00:04:50 GMT  
		Size: 35.8 MB (35750941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b531d0f3fa4a8c1e5c8c32c0c6a9de8cda1e078ed43db62853858f7ef792044b`  
		Last Modified: Sat, 19 Mar 2022 00:04:27 GMT  
		Size: 2.4 MB (2418360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ead18221dfbeb2afd1c7044892b00c01b6b056d5feb01c74684dff97d67e8eb`  
		Last Modified: Sat, 19 Mar 2022 00:04:26 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1faeeef23a40a6e07406285a95e3f94a86314cef806a54bbf3e2672288624dc`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 10.8 KB (10772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41729cace1ddd94023eba72c5c881b17ee1ab0e939be1d113c4f144fdae876c1`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 703.9 KB (703890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca1f8edf6ec39144c3fa34019e53bf9892978c935ab4b45e035f61c9cd7e32b`  
		Last Modified: Sat, 19 Mar 2022 23:42:57 GMT  
		Size: 9.6 MB (9569052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8628b5b59160ec4766d80912273c9024695381f2b717407a91177b03925b4dd9`  
		Last Modified: Sat, 19 Mar 2022 23:43:56 GMT  
		Size: 69.5 MB (69483628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678ef4fd7c46697fe04cca3f1ecc814f51b56a03ea9abb66a3c1fb7c22093eb6`  
		Last Modified: Sat, 19 Mar 2022 23:42:42 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:4f35663f73dfc11751365716b7d6a9d08e66e2cd0b7b6d6d276e9167c66dbe21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140115021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91b197627739a94af9bff95a19a902e84b7a352936df176d8b8dc38f329a3c9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 23:07:29 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:28:15 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="094790128069eccc9534214e7435c70bcafa221a0ef0f229c59418f8762704fa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 23:28:15 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:28:21 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 23:28:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:28:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:28:23 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:45:45 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 19 Mar 2022 17:45:47 GMT
RUN apk add --no-cache 		bash
# Sat, 19 Mar 2022 17:45:47 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:45:48 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 17:46:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 17:46:27 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 17:46:28 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 17:46:29 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 17:49:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 17:49:59 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 17:50:01 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 17:50:04 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 19 Mar 2022 17:50:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:50:08 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 17:50:11 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c992e90d8c9f9d1552190d2c0c3fa8fb5e94e39970cd9453e2819dc8b40ec1`  
		Last Modified: Sat, 19 Mar 2022 00:52:52 GMT  
		Size: 37.0 MB (37013909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc77e26b629b7d5ec72075b9db80763d03618483ac484e3129801b1b8131c6fe`  
		Last Modified: Sat, 19 Mar 2022 00:52:45 GMT  
		Size: 2.4 MB (2425472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36be0e7c4d5b1efb3a4be2317e16421a2d536fefec860c776192b0e5447a112`  
		Last Modified: Sat, 19 Mar 2022 00:52:44 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f881f7c1a27e3be051f3f7a6dc8e2234929511ade4258d41308f3b54ac77285`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 11.0 KB (10998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010ed0c2707cfd63880efce177bce0dc0dcb620859f33f8eb2c8661ad10a49e5`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 826.0 KB (826035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e719b3448e3e9cafa84aaabc148a2d7dff4a9270250a65345e20bf35c1c76c37`  
		Last Modified: Sat, 19 Mar 2022 17:51:19 GMT  
		Size: 9.6 MB (9567877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d1d97f9f627913a5b6dc23c20ffd479ab36bf7c28953fc4c3b4c0edd429b89`  
		Last Modified: Sat, 19 Mar 2022 17:51:33 GMT  
		Size: 87.6 MB (87553844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5845b747e168c1f1735cafd197dad4457d79ab2f392bd7645e166687392e3da`  
		Last Modified: Sat, 19 Mar 2022 17:51:16 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:latest`

```console
$ docker pull ghost@sha256:8dbf032df937aee9b24ea5bce598e76560fedfa8a3c3bf9ab53478be8053dd22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:latest` - linux; amd64

```console
$ docker pull ghost@sha256:7df40e0443f1348977c629d0c6739332c60a93a59a864cf0c059e9081f69b538
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.3 MB (148271097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:669ab852b2633345fef2005c32cf301d19548ef7485faea31af70a7e4fcfd45e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:59 GMT
ADD file:36919ae6bb25e3269eff949443129a01a8a43fb967fe6563939ebe1e1e9b8228 in / 
# Thu, 17 Mar 2022 04:03:59 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 13:00:01 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 21:50:00 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 21:50:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 21:50:35 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:50:47 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 21:50:47 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:50:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:50:47 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:04:25 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 00:04:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 00:04:43 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:04:44 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 00:05:16 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 00:05:17 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 00:06:45 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 00:06:47 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 00:06:47 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 00:06:47 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 00:06:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:06:48 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 00:06:48 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:ae13dd57832654086618a81dbc128846aa092489260c326ee95429b63c3cf213`  
		Last Modified: Thu, 17 Mar 2022 04:10:05 GMT  
		Size: 31.4 MB (31376572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bc29d3bc64ca0852101d86667b4a0d1908f05fe0bfead140cf838c0be01bc3`  
		Last Modified: Thu, 17 Mar 2022 13:19:15 GMT  
		Size: 4.2 KB (4183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a71a1d6cc6986624592a148f866355b9b90ddcd4a1f24be36b0f849d8c1044`  
		Last Modified: Fri, 18 Mar 2022 22:14:33 GMT  
		Size: 36.0 MB (36048047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5afd073302f60aad2c5067b89a976a5572fa262d0b60478970f307f8f94b97`  
		Last Modified: Fri, 18 Mar 2022 22:14:27 GMT  
		Size: 2.8 MB (2781848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5878f59eaa39846dd1173083e2e77dc140082be0efc61f7838c3403c6254b113`  
		Last Modified: Fri, 18 Mar 2022 22:14:26 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753aec878444f5bbf5b9e13544f6a3caf78aae1d01d506806f4b342c32623f2a`  
		Last Modified: Sat, 19 Mar 2022 00:09:27 GMT  
		Size: 1.4 MB (1448123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e282a0a274714713330c2ae37bb9aa1be203226d7ffd7de6eec07f2e35270c8`  
		Last Modified: Sat, 19 Mar 2022 00:09:31 GMT  
		Size: 9.6 MB (9567975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6128fb86f0f4e39a32aa4c08d17f607dd59d85e5f88743f9c8e88dd758997be6`  
		Last Modified: Sat, 19 Mar 2022 00:09:44 GMT  
		Size: 67.0 MB (67043352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509f7cfac26d6d851aa8ff0c01c9d486dbea8e2db7dc31aa28842be210035fb5`  
		Last Modified: Sat, 19 Mar 2022 00:09:26 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; arm variant v7

```console
$ docker pull ghost@sha256:78719e5300fc6838cdfe4fe7bc7b089fcae5c3970dee91fbcbc37e9c6d3c7475
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.0 MB (147043059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34fb82b494adf39572f85b07c9779bb0b0724e4e29049dc5ad3404f173ba3abd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 14:47:47 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 22:50:57 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:51:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 22:51:48 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:52:22 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 22:52:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:52:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:52:23 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:22:42 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 23:23:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 23:23:10 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:23:10 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:23:59 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:24:01 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 23:31:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 23:31:50 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 23:31:50 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 23:31:50 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 23:31:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 23:31:51 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 23:31:52 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c69f71c16ec3df2b7d124845d1b3b6e6495150f4ea3398c32a390afffbf142`  
		Last Modified: Fri, 18 Mar 2022 17:06:49 GMT  
		Size: 4.2 KB (4166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b32ca858e17b62400e3e3939b76745bd091c2302dcb5a659f98f4036c58ad`  
		Last Modified: Sat, 19 Mar 2022 00:07:18 GMT  
		Size: 34.2 MB (34206692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2605fefc93565569e993984be795855508fc11258205a2f0ab736807a40c2c`  
		Last Modified: Sat, 19 Mar 2022 00:06:56 GMT  
		Size: 2.8 MB (2772408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a649abf5b9f938b138570d940f0d8c3af7d265d4e26a25cf69fbd121df9381c`  
		Last Modified: Sat, 19 Mar 2022 00:06:54 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4041d8d2d15b52a58284107ec1fbc633900cce1fc07418607ed52ea1564428aa`  
		Last Modified: Sat, 19 Mar 2022 23:41:13 GMT  
		Size: 1.4 MB (1400322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04c308287b4673d9ba168fbb3d4cec8b9c7e8a9fe4ce8e8bab11f7a83658e18`  
		Last Modified: Sat, 19 Mar 2022 23:41:27 GMT  
		Size: 9.6 MB (9569190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25431520d805b108ecaf6cbf6e20b77e5401b5e75a367d828d99d0a68a2612d0`  
		Last Modified: Sat, 19 Mar 2022 23:42:23 GMT  
		Size: 72.5 MB (72514183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb31846b09f2de8a7bb58d2524fb744ac8124092cd9ee0a6f2ba64f8e8cf782`  
		Last Modified: Sat, 19 Mar 2022 23:41:12 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:f4a663d141c3204ae4bc882b0fc57cb214361f6b4c8bde126b67c24aad420674
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154343013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a20e32182de795f606b46f40248f7b94fc474d808fe5fd7d57d6417b85d50fb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:57 GMT
ADD file:e52e032f1ace6abd44b3647d43c1b8ae30bac6de804eef09c6ccd793057996fd in / 
# Thu, 17 Mar 2022 03:21:58 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:20:12 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 23:50:24 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:50:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 23:50:49 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:51:01 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 23:51:03 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:51:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:51:04 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:41:23 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 17:41:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 17:41:34 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:41:35 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 17:42:09 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 17:42:11 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 17:42:12 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 17:42:13 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 17:45:21 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 17:45:24 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 17:45:26 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 17:45:29 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 17:45:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:45:34 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 17:45:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:32252aec0777ac025a158bc2a8317650a4f2a0a875387011b1165013874f8723`  
		Last Modified: Thu, 17 Mar 2022 03:28:36 GMT  
		Size: 30.1 MB (30063013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e302ce9f0603b4af265c90ba2a4807900c24096808fb68bf44300bd440542`  
		Last Modified: Thu, 17 Mar 2022 13:54:35 GMT  
		Size: 4.0 KB (4042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98badb25d325c02976fab44804955d995b60a19fc609da8e3f1e642c52d898f9`  
		Last Modified: Sat, 19 Mar 2022 00:54:11 GMT  
		Size: 36.2 MB (36154505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5d43df9c11963e4b0e365e779e63981833ea41bdcc5d4db11c675fcc84fab3`  
		Last Modified: Sat, 19 Mar 2022 00:54:06 GMT  
		Size: 2.8 MB (2781278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad002987a7bae850089e45777bc9a362a9f8e3c656bdbbb26980ec4776d4704b`  
		Last Modified: Sat, 19 Mar 2022 00:54:05 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643f6d4797a5cc96449c367b48271ff6c2fdb6908b35b0b9c4c548113d8535a9`  
		Last Modified: Sat, 19 Mar 2022 17:50:44 GMT  
		Size: 1.4 MB (1383662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cde83364d3aeeba3311efa235a8b37ae7bbe49fd46d82e326c8c363b094c82`  
		Last Modified: Sat, 19 Mar 2022 17:50:46 GMT  
		Size: 9.6 MB (9568502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f817e8e904ee939974f5e8f516b174c335682a40a40694832630f3270b0e296`  
		Last Modified: Sat, 19 Mar 2022 17:50:58 GMT  
		Size: 74.4 MB (74387013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d099ce69b402eb198ddea013bbe31fe8ba1a37a42105d092444d276d82d59d61`  
		Last Modified: Sat, 19 Mar 2022 17:50:43 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; ppc64le

```console
$ docker pull ghost@sha256:ce8b4d8f9715c7c70c7e6e1746f7535091887d178ca17dc773a8bd7dfb673f4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155730905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97937daf1eb28848ecc7f38f97257c3d3573a82441d3c76be44346b51497cc36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 11:17:54 GMT
ADD file:e8555f1cb439a45786b92e929cfa154b51f668c5b4cd69e4ce98340c5998fe0c in / 
# Thu, 17 Mar 2022 11:18:00 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 03:54:03 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 23:06:48 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 23:11:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 23:11:09 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 23:14:42 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 23:14:44 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:14:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:14:53 GMT
CMD ["node"]
# Sat, 19 Mar 2022 23:46:25 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 23:47:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 23:47:53 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 23:47:55 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 23:49:09 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 23:49:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 23:49:15 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 23:49:17 GMT
ENV GHOST_VERSION=4.39.1
# Sun, 20 Mar 2022 00:11:36 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sun, 20 Mar 2022 00:11:46 GMT
WORKDIR /var/lib/ghost
# Sun, 20 Mar 2022 00:11:51 GMT
VOLUME [/var/lib/ghost/content]
# Sun, 20 Mar 2022 00:11:52 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sun, 20 Mar 2022 00:11:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 00:11:59 GMT
EXPOSE 2368
# Sun, 20 Mar 2022 00:12:01 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:aec78dc45d7b3df12df0672d13e22005592b453f03ff2580efac2598dddd680b`  
		Last Modified: Thu, 17 Mar 2022 11:28:17 GMT  
		Size: 35.3 MB (35279758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca53b81b04fce4349fb7d53e6c96231409ea54bc6d07808c393a268d8fcd78c3`  
		Last Modified: Fri, 18 Mar 2022 08:33:21 GMT  
		Size: 4.2 KB (4190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307e188a803758441743ab6c2c16c58d32cd25920f05e601d9fa75c13f8ec1f4`  
		Last Modified: Sat, 19 Mar 2022 02:15:29 GMT  
		Size: 38.0 MB (37978420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6a74008e734f41eb1091af470bca5677108b1eb61729b017bd6e96944fc1c1`  
		Last Modified: Sat, 19 Mar 2022 02:15:22 GMT  
		Size: 2.8 MB (2782569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9e81db75711e347d46105e0daee9e64692433ad3141a1cf1a52bca316993e`  
		Last Modified: Sat, 19 Mar 2022 02:15:22 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d14ae585ca54d978c72b25f6580d1c2986a60f049aefed6a7146e58b8eb07da`  
		Last Modified: Sun, 20 Mar 2022 00:12:26 GMT  
		Size: 1.4 MB (1367834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4904132a0f018373255a9418743ef13604d402190eaf4737c0de15b28964951`  
		Last Modified: Sun, 20 Mar 2022 00:12:31 GMT  
		Size: 9.6 MB (9568608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12320605293f45afa67cc47adf173b0888368bb06886b3b219e3cd4a68fafac`  
		Last Modified: Sun, 20 Mar 2022 00:12:43 GMT  
		Size: 68.7 MB (68748529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270139457a810a99e7dd44848741575b541fe0de273a395f04a5c15fb54ccb23`  
		Last Modified: Sun, 20 Mar 2022 00:12:26 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; s390x

```console
$ docker pull ghost@sha256:45b1aa5e819038cf640e167b5a5a4ee3b7b1f8f534b9eef0696dbfe88a14e27c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.5 MB (147499556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a439d42fd5331e4df800fb4597e9eb5c12e1e4aa7a72b029fc59b3b884edd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 12:50:36 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 22:14:52 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 22:15:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Fri, 18 Mar 2022 22:15:12 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:15:21 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Fri, 18 Mar 2022 22:15:21 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:15:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:15:22 GMT
CMD ["node"]
# Sat, 19 Mar 2022 04:38:44 GMT
ENV GOSU_VERSION=1.12
# Sat, 19 Mar 2022 04:38:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 19 Mar 2022 04:38:53 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 04:38:53 GMT
ENV GHOST_CLI_VERSION=1.18.2
# Sat, 19 Mar 2022 04:39:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 19 Mar 2022 04:39:24 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 19 Mar 2022 04:39:24 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 19 Mar 2022 04:39:25 GMT
ENV GHOST_VERSION=4.39.1
# Sat, 19 Mar 2022 04:42:06 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python2; 		rm -rf /var/lib/apt/lists/*; 				npm_config_python='python2' gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source --ignore-optional; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 19 Mar 2022 04:42:15 GMT
WORKDIR /var/lib/ghost
# Sat, 19 Mar 2022 04:42:15 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 19 Mar 2022 04:42:16 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Sat, 19 Mar 2022 04:42:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 04:42:16 GMT
EXPOSE 2368
# Sat, 19 Mar 2022 04:42:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722821cfaf9b99e01207f42d38caa8d0eea9818925d58a5d590057ff6271525d`  
		Last Modified: Thu, 17 Mar 2022 14:21:32 GMT  
		Size: 4.2 KB (4189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924acd2003e404035ae30769a9ed0531c116ccfe4965f354999da4c593b38dc`  
		Last Modified: Fri, 18 Mar 2022 23:10:07 GMT  
		Size: 35.9 MB (35913738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1c92724e1dbac9baa9b4949197499bd94e7abda3f1392dd48cc6f78fb23589`  
		Last Modified: Fri, 18 Mar 2022 23:10:03 GMT  
		Size: 2.8 MB (2782997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f42e3d4bc22c450816fb2255b83b884ec091394d12aff4a84c65c1193e935a`  
		Last Modified: Fri, 18 Mar 2022 23:10:03 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a61fd10dbc4124b4be87498e57bca3e89cab9d50ed7acf9934d6103e2b32eb`  
		Last Modified: Sat, 19 Mar 2022 04:42:48 GMT  
		Size: 1.4 MB (1434956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d6f9332f2c9557e6d14acdf3a51fb916f10fa41d64027309df97ce26b51dbc`  
		Last Modified: Sat, 19 Mar 2022 04:42:49 GMT  
		Size: 9.6 MB (9567431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b22e8969248f953b6c6d82f75ca2021591edf483759ad1672850841c2b90299`  
		Last Modified: Sat, 19 Mar 2022 04:42:59 GMT  
		Size: 68.1 MB (68139455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09db7bc896fefc28b64d7f40ca85f1aed46b128fcde04b0748a3ddfe437daa11`  
		Last Modified: Sat, 19 Mar 2022 04:42:47 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
