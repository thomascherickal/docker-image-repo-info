<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ghost`

-	[`ghost:4`](#ghost4)
-	[`ghost:4-alpine`](#ghost4-alpine)
-	[`ghost:4.48`](#ghost448)
-	[`ghost:4.48-alpine`](#ghost448-alpine)
-	[`ghost:4.48.2`](#ghost4482)
-	[`ghost:4.48.2-alpine`](#ghost4482-alpine)
-	[`ghost:5`](#ghost5)
-	[`ghost:5-alpine`](#ghost5-alpine)
-	[`ghost:5.12`](#ghost512)
-	[`ghost:5.12-alpine`](#ghost512-alpine)
-	[`ghost:5.12.0`](#ghost5120)
-	[`ghost:5.12.0-alpine`](#ghost5120-alpine)
-	[`ghost:alpine`](#ghostalpine)
-	[`ghost:latest`](#ghostlatest)

## `ghost:4`

```console
$ docker pull ghost@sha256:d256880e794fb870c8e4d9c5b0b5f462f55fbca7f2d47fc78e9a37a04e6c6705
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
$ docker pull ghost@sha256:b79cc4dc90abfb31c3d96fe1066a0f89ea67e1f65a06d0fee65be33e6daf9012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153118922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae6b8d721a278fce74d2cad9d4f0c2545fdd21fdcd1fd931fff51d0f0f4b9f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:03:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:08:15 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 04:08:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:08:43 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:08:55 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:08:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:08:55 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:53:14 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:53:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:53:25 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:53:25 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:53:52 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:53:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:53:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 20:53:53 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 20:54:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 20:54:57 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 20:54:57 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 20:54:57 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 20:54:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 20:54:57 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 20:54:57 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065fda631bffac8aa07440d44064117eee8bbfb50d65e04dbd5b29021c0140bf`  
		Last Modified: Tue, 23 Aug 2022 04:12:47 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ec249bd481d6b9b90895320b0623267b937930af8289419142b25431b5e45`  
		Last Modified: Tue, 23 Aug 2022 04:16:45 GMT  
		Size: 36.1 MB (36066216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164bac049d8635f1f89f41277cc476550eee2aa272896939c2ce03ab6129b82a`  
		Last Modified: Tue, 23 Aug 2022 04:16:40 GMT  
		Size: 2.8 MB (2792038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d37c9bb493cc0b8f1b8f5f07a95cbedcf4849fb8b1182ad982a92ea24fc9fa`  
		Last Modified: Tue, 23 Aug 2022 04:16:39 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83180ff6457f93520a6f04d7f5b9ed6dcda59611cf83b3b2928c9227f1b834c9`  
		Last Modified: Tue, 23 Aug 2022 20:55:58 GMT  
		Size: 1.4 MB (1448257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb12a4e26b628f8cdeb898d50ccdc7e63bb54b7a7a34a6f7dce42d81189b867`  
		Last Modified: Tue, 23 Aug 2022 20:56:00 GMT  
		Size: 10.5 MB (10474883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7db60bd998f5af0df8ca87809d16c65c18c8d855e400c31d7a85c7fc19a0705`  
		Last Modified: Tue, 23 Aug 2022 20:56:10 GMT  
		Size: 71.0 MB (70950866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a717867f3e188de62caaf05bb6935ceb175bd1ce3050d8c9d3956f069da17c98`  
		Last Modified: Tue, 23 Aug 2022 20:55:57 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4` - linux; arm variant v7

```console
$ docker pull ghost@sha256:2074acdffff45db9702ec7563136addb6ec6379b5488b1f671362413b89df37c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166907887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe194b7bd13214424fa5a825c2ead033cdcebab4a50302520a05926f0cbf167`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:44:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 21:51:19 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 21:51:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 21:51:48 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 21:52:00 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 21:52:01 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 21:52:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:52:01 GMT
CMD ["node"]
# Thu, 25 Aug 2022 11:23:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 25 Aug 2022 11:24:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 25 Aug 2022 11:24:04 GMT
ENV NODE_ENV=production
# Thu, 25 Aug 2022 11:24:04 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Thu, 25 Aug 2022 11:24:42 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Thu, 25 Aug 2022 11:24:43 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Thu, 25 Aug 2022 11:24:43 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 25 Aug 2022 11:24:43 GMT
ENV GHOST_VERSION=4.48.2
# Thu, 25 Aug 2022 11:31:24 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 25 Aug 2022 11:31:25 GMT
WORKDIR /var/lib/ghost
# Thu, 25 Aug 2022 11:31:25 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 25 Aug 2022 11:31:26 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Thu, 25 Aug 2022 11:31:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Aug 2022 11:31:26 GMT
EXPOSE 2368
# Thu, 25 Aug 2022 11:31:26 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5221a7a14db5d9fbd6928fcb2921040bb5d801661c018df5b4922f1c0cd73b25`  
		Last Modified: Tue, 23 Aug 2022 22:00:09 GMT  
		Size: 4.2 KB (4168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd95c7a73ed249c57ba223090a89338e0134753b81abf3b6d9fd6f68c2790889`  
		Last Modified: Tue, 23 Aug 2022 22:05:54 GMT  
		Size: 34.2 MB (34226454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c689dd7090fcc73638299bd0b2dea6dace2555089c78c67b63f256766e5f2ed6`  
		Last Modified: Tue, 23 Aug 2022 22:05:45 GMT  
		Size: 2.8 MB (2782975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e14669509146e051ead49dc0000d61beeca1ca9920ce8fcbba53d7d40c3ed66`  
		Last Modified: Tue, 23 Aug 2022 22:05:44 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5033373e37fe063c2e876acd7419e6eab8a89b4c44975b196f26e9681da7693`  
		Last Modified: Thu, 25 Aug 2022 11:34:24 GMT  
		Size: 1.4 MB (1400168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c384dc693fdd0b610909915a4120209458ff6f198ba457a8f2d823c967db99`  
		Last Modified: Thu, 25 Aug 2022 11:34:36 GMT  
		Size: 10.5 MB (10475286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454d6df1620e4006a45000ab178d5fb09f4bd6c1ebe17836da2484c19c0c2a00`  
		Last Modified: Thu, 25 Aug 2022 11:34:56 GMT  
		Size: 91.4 MB (91446106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e880b36e82ebe3ced44fe60025b24d56d75d0dffeb88c7de829fecd61bee22fa`  
		Last Modified: Thu, 25 Aug 2022 11:34:23 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:46fb6c1bc0d8782564620dfc6a0ceca81750665722781f66d9d8e7e4abd09ca8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.5 MB (149546600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:168e1856d35603c78cf4f3479dd03a2d00367b176a1bcaabb72df02fe12e17b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:51:52 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:58:36 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 04:59:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:59:04 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:59:17 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:59:18 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:59:19 GMT
CMD ["node"]
# Tue, 23 Aug 2022 22:21:46 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 22:21:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 22:21:58 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 22:21:59 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 22:22:33 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 22:22:34 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 22:22:35 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 22:22:36 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 22:23:42 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 22:23:45 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 22:23:48 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 22:23:51 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 22:23:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 22:23:56 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 22:23:58 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f232a362cd9820adfd1443fbb1fe468c3175d65fa45259cc218f0b706a0ab11`  
		Last Modified: Tue, 23 Aug 2022 05:08:27 GMT  
		Size: 4.0 KB (4044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb15c1f69124e6198fa23e6d24f9835f6addc53026db7b2fb8a3251b397dc74`  
		Last Modified: Tue, 23 Aug 2022 05:13:16 GMT  
		Size: 36.2 MB (36161922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77315a20631c514f49b1df983a0c0f3037aebe4e83e6d3ce1b4ee73627b18cb`  
		Last Modified: Tue, 23 Aug 2022 05:13:10 GMT  
		Size: 2.8 MB (2791355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebd11967d647dd5cfc6cb25b9af5bbc4ed98395d3059ad661b3ae19057506dd`  
		Last Modified: Tue, 23 Aug 2022 05:13:10 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b22fca5731e39eadceb2d45458c67cadb51c629991c15d27a33c8ba008a0b2`  
		Last Modified: Tue, 23 Aug 2022 22:25:19 GMT  
		Size: 1.4 MB (1383753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e10c3358112d2bca2a7ea242b70718f6f4880ca6df7fe67966368acb90c9438`  
		Last Modified: Tue, 23 Aug 2022 22:25:22 GMT  
		Size: 10.5 MB (10476396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e66dd3c3638a5992c99646ab7e5fd0135fcc3871922907f568e29c9e47b8cac`  
		Last Modified: Tue, 23 Aug 2022 22:25:32 GMT  
		Size: 68.7 MB (68664343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6234a798ea401e9f16986f2b56edfc13398e8fa646ec762baff6826f0d58b5`  
		Last Modified: Tue, 23 Aug 2022 22:25:19 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4` - linux; ppc64le

```console
$ docker pull ghost@sha256:9dc5f7cb9b47635f0fe7fdd6665bc3f32ef2cd6021f1dd6cb804b30ffcf13d93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.4 MB (166360663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39a8581db5d39af705e561cb0f74962e65df69c9586b702d5a917c6b8e8bd13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:59:59 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 03:05:13 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 03:05:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 03:05:57 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 03:06:21 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 03:06:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 03:06:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 03:06:23 GMT
CMD ["node"]
# Tue, 23 Aug 2022 16:27:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 16:27:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 16:27:36 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 16:27:37 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 16:28:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 16:28:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 16:28:29 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 16:28:29 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 16:35:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 16:35:54 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 16:35:55 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 16:35:55 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 16:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 16:35:56 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 16:35:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f072867559a95ee18a2f9cafdd6d774dfd46aced3278c83d3652f9b47874402`  
		Last Modified: Tue, 23 Aug 2022 03:11:50 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2272bbef19d126f23a941cd5eb124198e71e91c2b00a9b5253db6205116aa8f4`  
		Last Modified: Tue, 23 Aug 2022 03:15:02 GMT  
		Size: 38.0 MB (37977525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275af2b69ff4c61fae0af3e7d3388f7ce306b3471900336ca0409c263924b61a`  
		Last Modified: Tue, 23 Aug 2022 03:14:53 GMT  
		Size: 2.8 MB (2791986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225c695b0d7dbc52f4dadf5f3a95aba9fbd79ec2bea71e35f6e10953ff86f672`  
		Last Modified: Tue, 23 Aug 2022 03:14:52 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f26aa6f118c17b691193f698e7250a563053aff623d824a63239df6b7d1633`  
		Last Modified: Tue, 23 Aug 2022 16:37:12 GMT  
		Size: 1.4 MB (1367216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bffb191defb74dc8a00ff4dd28c9a4b3e2df2b5a819f09867eb6e2a2e712fd7`  
		Last Modified: Tue, 23 Aug 2022 16:37:17 GMT  
		Size: 10.5 MB (10475288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a72d2148854d00ca569e91fda3d1ce4e5a2ea960321d9bd0fefa4b047235db`  
		Last Modified: Tue, 23 Aug 2022 16:37:37 GMT  
		Size: 78.5 MB (78459185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd6488acf65305851445c7c8aa80845c3637135ffdb92add998e1820dd23cf7`  
		Last Modified: Tue, 23 Aug 2022 16:37:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4` - linux; s390x

```console
$ docker pull ghost@sha256:bced498888e99920bb8c2076716e53eb9c4f9c9ed031cea14d9ffa8f31a3658a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158163729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0306fa03f5c798c60ccacd08800f4b3f55d9985b710853196a19440b2e7a68c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 10:34:41 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 10:38:19 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 10:38:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 10:38:50 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 10:39:00 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 10:39:00 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 10:39:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 10:39:01 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:54:46 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:55:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:55:12 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:55:13 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:56:23 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:56:28 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:56:29 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 20:56:30 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 21:04:56 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 21:05:13 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 21:05:14 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 21:05:14 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 21:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:05:15 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 21:05:15 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c379dfa30c39780b6036486f76caf47f9c913cafd9fc09843e09a18b85d8a95f`  
		Last Modified: Tue, 23 Aug 2022 10:43:30 GMT  
		Size: 4.2 KB (4186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b41927d92a044b983988ff3c801976df26b4312b547721aca871afa8c8abe04`  
		Last Modified: Tue, 23 Aug 2022 10:45:27 GMT  
		Size: 35.9 MB (35930762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcf971b762bf5d61364656e8c639b452d040ec92fc08ed70cafdecbe4170441`  
		Last Modified: Tue, 23 Aug 2022 10:45:23 GMT  
		Size: 2.8 MB (2795017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be8f7c1b99237a851cae0c77480d132d3acb78b76793184cd97898394522ec`  
		Last Modified: Tue, 23 Aug 2022 10:45:23 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3532d952257c36ce5843da7bf0fd846e190bbe93a8e24fb22812af737cdc0df0`  
		Last Modified: Tue, 23 Aug 2022 21:06:17 GMT  
		Size: 1.4 MB (1435207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464123c020b16d4662f8090d708ca6cf4f1bb2736bb4fd9e601b3b8bf21ae585`  
		Last Modified: Tue, 23 Aug 2022 21:06:19 GMT  
		Size: 10.5 MB (10475352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8478740f82a8ef2317bc10855a3c5a127f3904f2e9b2741f0a7df626b8c87816`  
		Last Modified: Tue, 23 Aug 2022 21:06:30 GMT  
		Size: 77.9 MB (77872109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19773b2df153882c27d1a9915352719c330150694f750ef378531a9841372cbf`  
		Last Modified: Tue, 23 Aug 2022 21:06:17 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4-alpine`

```console
$ docker pull ghost@sha256:e88d4940126ce72857bf756704d541bdca735a45f6c1c126c905dc99d3d260df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:4-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:a26cb9b01baf3790d010d6c99fe1fd295fd51536cd511567858610f8acce25cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125404157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3f1999067d36d71407d9fcd456e8a22c060db9d8b95aa75ebe5cebc97a5516b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 21:03:22 GMT
ENV NODE_VERSION=14.20.0
# Tue, 09 Aug 2022 21:03:30 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 09 Aug 2022 21:03:30 GMT
ENV YARN_VERSION=1.22.19
# Tue, 09 Aug 2022 21:03:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 09 Aug 2022 21:03:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 09 Aug 2022 21:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 21:03:34 GMT
CMD ["node"]
# Wed, 10 Aug 2022 03:16:48 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 10 Aug 2022 03:16:49 GMT
RUN apk add --no-cache 		bash
# Wed, 10 Aug 2022 03:16:49 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:30:13 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:30:41 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:30:42 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:30:42 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:30:42 GMT
ENV GHOST_VERSION=4.48.2
# Fri, 19 Aug 2022 00:27:04 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 19 Aug 2022 00:27:06 GMT
WORKDIR /var/lib/ghost
# Fri, 19 Aug 2022 00:27:06 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 00:27:06 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 00:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 00:27:07 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 00:27:07 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb06cd79147098226b90a44ed66cc7ec9f2f4175ee2d90557fd99500e9bd3da`  
		Last Modified: Tue, 09 Aug 2022 21:08:23 GMT  
		Size: 37.2 MB (37234122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765a58e5319058a1ec35459f25ffb310cd052522d9254b4ab11f7055517251bb`  
		Last Modified: Tue, 09 Aug 2022 21:08:18 GMT  
		Size: 2.4 MB (2368736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beee7f5da459e13aa9d48d8d1279ec75df8a68613a996f27e7c20a3246ab1432`  
		Last Modified: Tue, 09 Aug 2022 21:08:17 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516e40f07fa2e3168daff25293ed11e979722e20b781f0233da502442341891c`  
		Last Modified: Wed, 10 Aug 2022 03:19:28 GMT  
		Size: 11.3 KB (11275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66bf249fe1b89c2a761ff737252be2cf8d3c6523fcad38fc0bb6f704141f14c`  
		Last Modified: Wed, 10 Aug 2022 03:19:28 GMT  
		Size: 820.0 KB (820043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2688a29e863f75c4331bc984d1b16d8cf84fec0a151802044c277381ce3257`  
		Last Modified: Fri, 12 Aug 2022 00:33:46 GMT  
		Size: 10.5 MB (10475729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a56dc0c4d2daf7a26a3eb9ce9dfab64c71888cfbbdf37a9f3757b9025adf0b`  
		Last Modified: Fri, 19 Aug 2022 00:28:19 GMT  
		Size: 71.7 MB (71687200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb3827b8e84ea980ee2f03a8310e9128ae4d89eb0b5cfc59683ed2ea1226089`  
		Last Modified: Fri, 19 Aug 2022 00:28:07 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:21d46727d65227b34b48bd707881274b1909bd9c48caea910e00c116430fd258
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128705469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1063abd59d1a6b00e8450572875f8413009a6a22146842e9c5e0df767db4f324`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 09:19:32 GMT
ENV NODE_VERSION=14.20.0
# Wed, 10 Aug 2022 11:12:16 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 10 Aug 2022 11:12:16 GMT
ENV YARN_VERSION=1.22.19
# Wed, 10 Aug 2022 11:12:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 10 Aug 2022 11:12:23 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 10 Aug 2022 11:12:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 11:12:23 GMT
CMD ["node"]
# Thu, 11 Aug 2022 01:28:07 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 11 Aug 2022 01:28:08 GMT
RUN apk add --no-cache 		bash
# Thu, 11 Aug 2022 01:28:08 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:04:45 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:06:04 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:06:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:06:05 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:06:05 GMT
ENV GHOST_VERSION=4.48.2
# Fri, 19 Aug 2022 04:04:27 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 19 Aug 2022 04:04:28 GMT
WORKDIR /var/lib/ghost
# Fri, 19 Aug 2022 04:04:29 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 04:04:29 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 04:04:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 04:04:29 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 04:04:29 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3013f82179b5c8924f9d3de2ada926fb916bdf161bf2592ab46dfc11a0e70d87`  
		Last Modified: Wed, 10 Aug 2022 11:15:56 GMT  
		Size: 36.3 MB (36281861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a175c263694a52363e6903954aacce227330e9ae38f7dc663e7e12ffe1451`  
		Last Modified: Wed, 10 Aug 2022 11:15:49 GMT  
		Size: 2.4 MB (2447687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db221eecf612fb8d7475005c6de72bbaaa455cc937e081cce984ffd0faf58ab7`  
		Last Modified: Wed, 10 Aug 2022 11:15:48 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec39c3839dc8024d012fd6a66fa091cb930ff1f325941985e447902316fee6d2`  
		Last Modified: Fri, 19 Aug 2022 04:05:09 GMT  
		Size: 11.0 KB (10964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fc9db4af048ebdaafc3ac90e5472dcb7b7bb016efe8f434f4ff650e9d901e3`  
		Last Modified: Fri, 19 Aug 2022 04:05:10 GMT  
		Size: 772.0 KB (771994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4318f596df9a2394a8bd2730410d61827c5ba2b7b6995d6e15ad35c5771238f`  
		Last Modified: Fri, 19 Aug 2022 04:05:23 GMT  
		Size: 10.5 MB (10474611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6847c838a915d01366d3ebf51d7840f194c6c6b09bca86a5b4a5420cc651f4b3`  
		Last Modified: Fri, 19 Aug 2022 04:05:33 GMT  
		Size: 76.1 MB (76103388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7a415c5d8fae58acfc30f9e2151c1f95b2c0bb493bbdc1e6c52d0216315de9`  
		Last Modified: Fri, 19 Aug 2022 04:05:09 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:16a74cdfeefc8374978d6195378b18bfedf5b915968670977aeedfc8b8c21891
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127477594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680a135de23810d1d7fc4adb102927520f99cc4764a6a06758599b9c426dd7a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 12:12:46 GMT
ENV NODE_VERSION=14.20.0
# Wed, 10 Aug 2022 14:02:22 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 10 Aug 2022 14:02:23 GMT
ENV YARN_VERSION=1.22.19
# Wed, 10 Aug 2022 14:02:29 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 10 Aug 2022 14:02:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 10 Aug 2022 14:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 14:02:29 GMT
CMD ["node"]
# Thu, 11 Aug 2022 04:47:58 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 11 Aug 2022 04:47:59 GMT
RUN apk add --no-cache 		bash
# Thu, 11 Aug 2022 04:47:59 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:32:38 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:33:29 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:33:30 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:33:30 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:33:30 GMT
ENV GHOST_VERSION=4.48.2
# Thu, 18 Aug 2022 22:33:02 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 18 Aug 2022 22:33:04 GMT
WORKDIR /var/lib/ghost
# Thu, 18 Aug 2022 22:33:04 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 06:09:36 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 06:09:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 06:09:36 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 06:09:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a5d5e3efc39633586d718ed087aa8c94ed97eb000bf3912b4ad58c8841a8df`  
		Last Modified: Wed, 10 Aug 2022 14:10:40 GMT  
		Size: 35.9 MB (35850710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e084b1c42c28230d701f5adf4c69cb86c4412c9e2831028d7a2084c9220a48`  
		Last Modified: Wed, 10 Aug 2022 14:10:33 GMT  
		Size: 2.4 MB (2447708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2375b3b7af35638f4a31108f06f9ff2c9c44ab48e889fc4b603424c0fe13a4bf`  
		Last Modified: Wed, 10 Aug 2022 14:10:32 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd28fec1bea3a7e87491fcbcfccc258fb18db7a477011fd1583abcedba497e`  
		Last Modified: Fri, 19 Aug 2022 06:11:11 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471192fd32321605cdea263d3d59d836c85fcdb6430a3617f767e8061cd9bcdc`  
		Last Modified: Fri, 19 Aug 2022 06:11:12 GMT  
		Size: 704.7 KB (704663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a075f4cdadc577f64fb02a1cebab124392c77e400811511d662f87d5d55847d4`  
		Last Modified: Fri, 19 Aug 2022 06:11:21 GMT  
		Size: 10.5 MB (10474493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0a965c7f189e120dc5a2d3451d798ddbdf117457f4efeb372ad301ff523cff`  
		Last Modified: Fri, 19 Aug 2022 06:11:43 GMT  
		Size: 75.6 MB (75571220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fcd21dfbc607aecc812bec89fe508a2f1a8eae91ea4aeb1d5c689a813426f9`  
		Last Modified: Fri, 19 Aug 2022 06:11:11 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:bb2e47be4baecfdc88b9d698e26fa6e3c913e6a06939f9854709031730c20012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122396337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cbc40902b1f3d2a7cd53b5289b76cf0037487d410a68af848b5c6f803555275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 23:33:51 GMT
ENV NODE_VERSION=14.20.0
# Tue, 09 Aug 2022 23:54:07 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 09 Aug 2022 23:54:07 GMT
ENV YARN_VERSION=1.22.19
# Tue, 09 Aug 2022 23:54:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 09 Aug 2022 23:54:14 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 09 Aug 2022 23:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 23:54:15 GMT
CMD ["node"]
# Wed, 10 Aug 2022 06:59:14 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 10 Aug 2022 06:59:16 GMT
RUN apk add --no-cache 		bash
# Wed, 10 Aug 2022 06:59:16 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:58:45 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:59:14 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:59:15 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:59:16 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:59:17 GMT
ENV GHOST_VERSION=4.48.2
# Fri, 19 Aug 2022 02:55:40 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 19 Aug 2022 02:55:44 GMT
WORKDIR /var/lib/ghost
# Fri, 19 Aug 2022 02:55:46 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 02:55:49 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 02:55:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 02:55:54 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 02:55:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4242f05bf8f81383ae5f83a145e56c06bd56cbbaf842d62336ae61ad5623d7c`  
		Last Modified: Wed, 10 Aug 2022 00:01:53 GMT  
		Size: 37.1 MB (37093903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32b5555b1313bb81b1adaf7d6b227602c820f6d8979c75c8ce0d56badf7393b`  
		Last Modified: Wed, 10 Aug 2022 00:01:47 GMT  
		Size: 2.5 MB (2456916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8b559c1581e3927b80bddba4943c340d93f53c1125df349532aac2d5bfdc22`  
		Last Modified: Wed, 10 Aug 2022 00:01:46 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0efd58105672cf062fb8f45d542eefd8c9f2878d890cc5e96f6932bfe23fb2`  
		Last Modified: Wed, 10 Aug 2022 07:02:30 GMT  
		Size: 11.0 KB (10988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab058ad29d156af9a9eff1d9c7e350c1216fb7497af1a6ab5590c4d6d6d80bc2`  
		Last Modified: Wed, 10 Aug 2022 07:02:31 GMT  
		Size: 826.1 KB (826083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e173c551124981202b7ceaff30a6da436121b2c3ff5ea7bfbbfbfe23e02ff91c`  
		Last Modified: Fri, 12 Aug 2022 01:03:11 GMT  
		Size: 10.5 MB (10475774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a42838339bf48103ea6e3bae7e0ad2d10c42c45ff051ffbfefd897397a6b1e`  
		Last Modified: Fri, 19 Aug 2022 02:57:23 GMT  
		Size: 68.8 MB (68824017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6e519d8dfabf0b5cc1a2a4a8dac016683e37dac1f0daffcc0b00e0b1fb97af`  
		Last Modified: Fri, 19 Aug 2022 02:57:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4.48`

```console
$ docker pull ghost@sha256:d256880e794fb870c8e4d9c5b0b5f462f55fbca7f2d47fc78e9a37a04e6c6705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:4.48` - linux; amd64

```console
$ docker pull ghost@sha256:b79cc4dc90abfb31c3d96fe1066a0f89ea67e1f65a06d0fee65be33e6daf9012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153118922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae6b8d721a278fce74d2cad9d4f0c2545fdd21fdcd1fd931fff51d0f0f4b9f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:03:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:08:15 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 04:08:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:08:43 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:08:55 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:08:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:08:55 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:53:14 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:53:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:53:25 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:53:25 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:53:52 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:53:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:53:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 20:53:53 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 20:54:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 20:54:57 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 20:54:57 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 20:54:57 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 20:54:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 20:54:57 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 20:54:57 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065fda631bffac8aa07440d44064117eee8bbfb50d65e04dbd5b29021c0140bf`  
		Last Modified: Tue, 23 Aug 2022 04:12:47 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ec249bd481d6b9b90895320b0623267b937930af8289419142b25431b5e45`  
		Last Modified: Tue, 23 Aug 2022 04:16:45 GMT  
		Size: 36.1 MB (36066216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164bac049d8635f1f89f41277cc476550eee2aa272896939c2ce03ab6129b82a`  
		Last Modified: Tue, 23 Aug 2022 04:16:40 GMT  
		Size: 2.8 MB (2792038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d37c9bb493cc0b8f1b8f5f07a95cbedcf4849fb8b1182ad982a92ea24fc9fa`  
		Last Modified: Tue, 23 Aug 2022 04:16:39 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83180ff6457f93520a6f04d7f5b9ed6dcda59611cf83b3b2928c9227f1b834c9`  
		Last Modified: Tue, 23 Aug 2022 20:55:58 GMT  
		Size: 1.4 MB (1448257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb12a4e26b628f8cdeb898d50ccdc7e63bb54b7a7a34a6f7dce42d81189b867`  
		Last Modified: Tue, 23 Aug 2022 20:56:00 GMT  
		Size: 10.5 MB (10474883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7db60bd998f5af0df8ca87809d16c65c18c8d855e400c31d7a85c7fc19a0705`  
		Last Modified: Tue, 23 Aug 2022 20:56:10 GMT  
		Size: 71.0 MB (70950866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a717867f3e188de62caaf05bb6935ceb175bd1ce3050d8c9d3956f069da17c98`  
		Last Modified: Tue, 23 Aug 2022 20:55:57 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48` - linux; arm variant v7

```console
$ docker pull ghost@sha256:2074acdffff45db9702ec7563136addb6ec6379b5488b1f671362413b89df37c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166907887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe194b7bd13214424fa5a825c2ead033cdcebab4a50302520a05926f0cbf167`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:44:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 21:51:19 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 21:51:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 21:51:48 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 21:52:00 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 21:52:01 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 21:52:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:52:01 GMT
CMD ["node"]
# Thu, 25 Aug 2022 11:23:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 25 Aug 2022 11:24:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 25 Aug 2022 11:24:04 GMT
ENV NODE_ENV=production
# Thu, 25 Aug 2022 11:24:04 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Thu, 25 Aug 2022 11:24:42 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Thu, 25 Aug 2022 11:24:43 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Thu, 25 Aug 2022 11:24:43 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 25 Aug 2022 11:24:43 GMT
ENV GHOST_VERSION=4.48.2
# Thu, 25 Aug 2022 11:31:24 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 25 Aug 2022 11:31:25 GMT
WORKDIR /var/lib/ghost
# Thu, 25 Aug 2022 11:31:25 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 25 Aug 2022 11:31:26 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Thu, 25 Aug 2022 11:31:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Aug 2022 11:31:26 GMT
EXPOSE 2368
# Thu, 25 Aug 2022 11:31:26 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5221a7a14db5d9fbd6928fcb2921040bb5d801661c018df5b4922f1c0cd73b25`  
		Last Modified: Tue, 23 Aug 2022 22:00:09 GMT  
		Size: 4.2 KB (4168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd95c7a73ed249c57ba223090a89338e0134753b81abf3b6d9fd6f68c2790889`  
		Last Modified: Tue, 23 Aug 2022 22:05:54 GMT  
		Size: 34.2 MB (34226454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c689dd7090fcc73638299bd0b2dea6dace2555089c78c67b63f256766e5f2ed6`  
		Last Modified: Tue, 23 Aug 2022 22:05:45 GMT  
		Size: 2.8 MB (2782975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e14669509146e051ead49dc0000d61beeca1ca9920ce8fcbba53d7d40c3ed66`  
		Last Modified: Tue, 23 Aug 2022 22:05:44 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5033373e37fe063c2e876acd7419e6eab8a89b4c44975b196f26e9681da7693`  
		Last Modified: Thu, 25 Aug 2022 11:34:24 GMT  
		Size: 1.4 MB (1400168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c384dc693fdd0b610909915a4120209458ff6f198ba457a8f2d823c967db99`  
		Last Modified: Thu, 25 Aug 2022 11:34:36 GMT  
		Size: 10.5 MB (10475286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454d6df1620e4006a45000ab178d5fb09f4bd6c1ebe17836da2484c19c0c2a00`  
		Last Modified: Thu, 25 Aug 2022 11:34:56 GMT  
		Size: 91.4 MB (91446106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e880b36e82ebe3ced44fe60025b24d56d75d0dffeb88c7de829fecd61bee22fa`  
		Last Modified: Thu, 25 Aug 2022 11:34:23 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:46fb6c1bc0d8782564620dfc6a0ceca81750665722781f66d9d8e7e4abd09ca8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.5 MB (149546600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:168e1856d35603c78cf4f3479dd03a2d00367b176a1bcaabb72df02fe12e17b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:51:52 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:58:36 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 04:59:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:59:04 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:59:17 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:59:18 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:59:19 GMT
CMD ["node"]
# Tue, 23 Aug 2022 22:21:46 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 22:21:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 22:21:58 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 22:21:59 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 22:22:33 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 22:22:34 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 22:22:35 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 22:22:36 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 22:23:42 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 22:23:45 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 22:23:48 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 22:23:51 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 22:23:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 22:23:56 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 22:23:58 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f232a362cd9820adfd1443fbb1fe468c3175d65fa45259cc218f0b706a0ab11`  
		Last Modified: Tue, 23 Aug 2022 05:08:27 GMT  
		Size: 4.0 KB (4044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb15c1f69124e6198fa23e6d24f9835f6addc53026db7b2fb8a3251b397dc74`  
		Last Modified: Tue, 23 Aug 2022 05:13:16 GMT  
		Size: 36.2 MB (36161922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77315a20631c514f49b1df983a0c0f3037aebe4e83e6d3ce1b4ee73627b18cb`  
		Last Modified: Tue, 23 Aug 2022 05:13:10 GMT  
		Size: 2.8 MB (2791355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebd11967d647dd5cfc6cb25b9af5bbc4ed98395d3059ad661b3ae19057506dd`  
		Last Modified: Tue, 23 Aug 2022 05:13:10 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b22fca5731e39eadceb2d45458c67cadb51c629991c15d27a33c8ba008a0b2`  
		Last Modified: Tue, 23 Aug 2022 22:25:19 GMT  
		Size: 1.4 MB (1383753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e10c3358112d2bca2a7ea242b70718f6f4880ca6df7fe67966368acb90c9438`  
		Last Modified: Tue, 23 Aug 2022 22:25:22 GMT  
		Size: 10.5 MB (10476396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e66dd3c3638a5992c99646ab7e5fd0135fcc3871922907f568e29c9e47b8cac`  
		Last Modified: Tue, 23 Aug 2022 22:25:32 GMT  
		Size: 68.7 MB (68664343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6234a798ea401e9f16986f2b56edfc13398e8fa646ec762baff6826f0d58b5`  
		Last Modified: Tue, 23 Aug 2022 22:25:19 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48` - linux; ppc64le

```console
$ docker pull ghost@sha256:9dc5f7cb9b47635f0fe7fdd6665bc3f32ef2cd6021f1dd6cb804b30ffcf13d93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.4 MB (166360663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39a8581db5d39af705e561cb0f74962e65df69c9586b702d5a917c6b8e8bd13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:59:59 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 03:05:13 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 03:05:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 03:05:57 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 03:06:21 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 03:06:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 03:06:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 03:06:23 GMT
CMD ["node"]
# Tue, 23 Aug 2022 16:27:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 16:27:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 16:27:36 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 16:27:37 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 16:28:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 16:28:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 16:28:29 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 16:28:29 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 16:35:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 16:35:54 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 16:35:55 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 16:35:55 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 16:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 16:35:56 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 16:35:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f072867559a95ee18a2f9cafdd6d774dfd46aced3278c83d3652f9b47874402`  
		Last Modified: Tue, 23 Aug 2022 03:11:50 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2272bbef19d126f23a941cd5eb124198e71e91c2b00a9b5253db6205116aa8f4`  
		Last Modified: Tue, 23 Aug 2022 03:15:02 GMT  
		Size: 38.0 MB (37977525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275af2b69ff4c61fae0af3e7d3388f7ce306b3471900336ca0409c263924b61a`  
		Last Modified: Tue, 23 Aug 2022 03:14:53 GMT  
		Size: 2.8 MB (2791986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225c695b0d7dbc52f4dadf5f3a95aba9fbd79ec2bea71e35f6e10953ff86f672`  
		Last Modified: Tue, 23 Aug 2022 03:14:52 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f26aa6f118c17b691193f698e7250a563053aff623d824a63239df6b7d1633`  
		Last Modified: Tue, 23 Aug 2022 16:37:12 GMT  
		Size: 1.4 MB (1367216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bffb191defb74dc8a00ff4dd28c9a4b3e2df2b5a819f09867eb6e2a2e712fd7`  
		Last Modified: Tue, 23 Aug 2022 16:37:17 GMT  
		Size: 10.5 MB (10475288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a72d2148854d00ca569e91fda3d1ce4e5a2ea960321d9bd0fefa4b047235db`  
		Last Modified: Tue, 23 Aug 2022 16:37:37 GMT  
		Size: 78.5 MB (78459185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd6488acf65305851445c7c8aa80845c3637135ffdb92add998e1820dd23cf7`  
		Last Modified: Tue, 23 Aug 2022 16:37:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48` - linux; s390x

```console
$ docker pull ghost@sha256:bced498888e99920bb8c2076716e53eb9c4f9c9ed031cea14d9ffa8f31a3658a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158163729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0306fa03f5c798c60ccacd08800f4b3f55d9985b710853196a19440b2e7a68c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 10:34:41 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 10:38:19 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 10:38:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 10:38:50 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 10:39:00 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 10:39:00 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 10:39:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 10:39:01 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:54:46 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:55:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:55:12 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:55:13 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:56:23 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:56:28 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:56:29 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 20:56:30 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 21:04:56 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 21:05:13 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 21:05:14 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 21:05:14 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 21:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:05:15 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 21:05:15 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c379dfa30c39780b6036486f76caf47f9c913cafd9fc09843e09a18b85d8a95f`  
		Last Modified: Tue, 23 Aug 2022 10:43:30 GMT  
		Size: 4.2 KB (4186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b41927d92a044b983988ff3c801976df26b4312b547721aca871afa8c8abe04`  
		Last Modified: Tue, 23 Aug 2022 10:45:27 GMT  
		Size: 35.9 MB (35930762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcf971b762bf5d61364656e8c639b452d040ec92fc08ed70cafdecbe4170441`  
		Last Modified: Tue, 23 Aug 2022 10:45:23 GMT  
		Size: 2.8 MB (2795017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be8f7c1b99237a851cae0c77480d132d3acb78b76793184cd97898394522ec`  
		Last Modified: Tue, 23 Aug 2022 10:45:23 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3532d952257c36ce5843da7bf0fd846e190bbe93a8e24fb22812af737cdc0df0`  
		Last Modified: Tue, 23 Aug 2022 21:06:17 GMT  
		Size: 1.4 MB (1435207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464123c020b16d4662f8090d708ca6cf4f1bb2736bb4fd9e601b3b8bf21ae585`  
		Last Modified: Tue, 23 Aug 2022 21:06:19 GMT  
		Size: 10.5 MB (10475352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8478740f82a8ef2317bc10855a3c5a127f3904f2e9b2741f0a7df626b8c87816`  
		Last Modified: Tue, 23 Aug 2022 21:06:30 GMT  
		Size: 77.9 MB (77872109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19773b2df153882c27d1a9915352719c330150694f750ef378531a9841372cbf`  
		Last Modified: Tue, 23 Aug 2022 21:06:17 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4.48-alpine`

```console
$ docker pull ghost@sha256:e88d4940126ce72857bf756704d541bdca735a45f6c1c126c905dc99d3d260df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:4.48-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:a26cb9b01baf3790d010d6c99fe1fd295fd51536cd511567858610f8acce25cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125404157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3f1999067d36d71407d9fcd456e8a22c060db9d8b95aa75ebe5cebc97a5516b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 21:03:22 GMT
ENV NODE_VERSION=14.20.0
# Tue, 09 Aug 2022 21:03:30 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 09 Aug 2022 21:03:30 GMT
ENV YARN_VERSION=1.22.19
# Tue, 09 Aug 2022 21:03:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 09 Aug 2022 21:03:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 09 Aug 2022 21:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 21:03:34 GMT
CMD ["node"]
# Wed, 10 Aug 2022 03:16:48 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 10 Aug 2022 03:16:49 GMT
RUN apk add --no-cache 		bash
# Wed, 10 Aug 2022 03:16:49 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:30:13 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:30:41 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:30:42 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:30:42 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:30:42 GMT
ENV GHOST_VERSION=4.48.2
# Fri, 19 Aug 2022 00:27:04 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 19 Aug 2022 00:27:06 GMT
WORKDIR /var/lib/ghost
# Fri, 19 Aug 2022 00:27:06 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 00:27:06 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 00:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 00:27:07 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 00:27:07 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb06cd79147098226b90a44ed66cc7ec9f2f4175ee2d90557fd99500e9bd3da`  
		Last Modified: Tue, 09 Aug 2022 21:08:23 GMT  
		Size: 37.2 MB (37234122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765a58e5319058a1ec35459f25ffb310cd052522d9254b4ab11f7055517251bb`  
		Last Modified: Tue, 09 Aug 2022 21:08:18 GMT  
		Size: 2.4 MB (2368736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beee7f5da459e13aa9d48d8d1279ec75df8a68613a996f27e7c20a3246ab1432`  
		Last Modified: Tue, 09 Aug 2022 21:08:17 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516e40f07fa2e3168daff25293ed11e979722e20b781f0233da502442341891c`  
		Last Modified: Wed, 10 Aug 2022 03:19:28 GMT  
		Size: 11.3 KB (11275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66bf249fe1b89c2a761ff737252be2cf8d3c6523fcad38fc0bb6f704141f14c`  
		Last Modified: Wed, 10 Aug 2022 03:19:28 GMT  
		Size: 820.0 KB (820043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2688a29e863f75c4331bc984d1b16d8cf84fec0a151802044c277381ce3257`  
		Last Modified: Fri, 12 Aug 2022 00:33:46 GMT  
		Size: 10.5 MB (10475729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a56dc0c4d2daf7a26a3eb9ce9dfab64c71888cfbbdf37a9f3757b9025adf0b`  
		Last Modified: Fri, 19 Aug 2022 00:28:19 GMT  
		Size: 71.7 MB (71687200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb3827b8e84ea980ee2f03a8310e9128ae4d89eb0b5cfc59683ed2ea1226089`  
		Last Modified: Fri, 19 Aug 2022 00:28:07 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:21d46727d65227b34b48bd707881274b1909bd9c48caea910e00c116430fd258
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128705469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1063abd59d1a6b00e8450572875f8413009a6a22146842e9c5e0df767db4f324`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 09:19:32 GMT
ENV NODE_VERSION=14.20.0
# Wed, 10 Aug 2022 11:12:16 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 10 Aug 2022 11:12:16 GMT
ENV YARN_VERSION=1.22.19
# Wed, 10 Aug 2022 11:12:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 10 Aug 2022 11:12:23 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 10 Aug 2022 11:12:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 11:12:23 GMT
CMD ["node"]
# Thu, 11 Aug 2022 01:28:07 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 11 Aug 2022 01:28:08 GMT
RUN apk add --no-cache 		bash
# Thu, 11 Aug 2022 01:28:08 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:04:45 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:06:04 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:06:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:06:05 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:06:05 GMT
ENV GHOST_VERSION=4.48.2
# Fri, 19 Aug 2022 04:04:27 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 19 Aug 2022 04:04:28 GMT
WORKDIR /var/lib/ghost
# Fri, 19 Aug 2022 04:04:29 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 04:04:29 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 04:04:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 04:04:29 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 04:04:29 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3013f82179b5c8924f9d3de2ada926fb916bdf161bf2592ab46dfc11a0e70d87`  
		Last Modified: Wed, 10 Aug 2022 11:15:56 GMT  
		Size: 36.3 MB (36281861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a175c263694a52363e6903954aacce227330e9ae38f7dc663e7e12ffe1451`  
		Last Modified: Wed, 10 Aug 2022 11:15:49 GMT  
		Size: 2.4 MB (2447687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db221eecf612fb8d7475005c6de72bbaaa455cc937e081cce984ffd0faf58ab7`  
		Last Modified: Wed, 10 Aug 2022 11:15:48 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec39c3839dc8024d012fd6a66fa091cb930ff1f325941985e447902316fee6d2`  
		Last Modified: Fri, 19 Aug 2022 04:05:09 GMT  
		Size: 11.0 KB (10964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fc9db4af048ebdaafc3ac90e5472dcb7b7bb016efe8f434f4ff650e9d901e3`  
		Last Modified: Fri, 19 Aug 2022 04:05:10 GMT  
		Size: 772.0 KB (771994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4318f596df9a2394a8bd2730410d61827c5ba2b7b6995d6e15ad35c5771238f`  
		Last Modified: Fri, 19 Aug 2022 04:05:23 GMT  
		Size: 10.5 MB (10474611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6847c838a915d01366d3ebf51d7840f194c6c6b09bca86a5b4a5420cc651f4b3`  
		Last Modified: Fri, 19 Aug 2022 04:05:33 GMT  
		Size: 76.1 MB (76103388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7a415c5d8fae58acfc30f9e2151c1f95b2c0bb493bbdc1e6c52d0216315de9`  
		Last Modified: Fri, 19 Aug 2022 04:05:09 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:16a74cdfeefc8374978d6195378b18bfedf5b915968670977aeedfc8b8c21891
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127477594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680a135de23810d1d7fc4adb102927520f99cc4764a6a06758599b9c426dd7a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 12:12:46 GMT
ENV NODE_VERSION=14.20.0
# Wed, 10 Aug 2022 14:02:22 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 10 Aug 2022 14:02:23 GMT
ENV YARN_VERSION=1.22.19
# Wed, 10 Aug 2022 14:02:29 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 10 Aug 2022 14:02:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 10 Aug 2022 14:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 14:02:29 GMT
CMD ["node"]
# Thu, 11 Aug 2022 04:47:58 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 11 Aug 2022 04:47:59 GMT
RUN apk add --no-cache 		bash
# Thu, 11 Aug 2022 04:47:59 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:32:38 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:33:29 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:33:30 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:33:30 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:33:30 GMT
ENV GHOST_VERSION=4.48.2
# Thu, 18 Aug 2022 22:33:02 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 18 Aug 2022 22:33:04 GMT
WORKDIR /var/lib/ghost
# Thu, 18 Aug 2022 22:33:04 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 06:09:36 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 06:09:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 06:09:36 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 06:09:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a5d5e3efc39633586d718ed087aa8c94ed97eb000bf3912b4ad58c8841a8df`  
		Last Modified: Wed, 10 Aug 2022 14:10:40 GMT  
		Size: 35.9 MB (35850710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e084b1c42c28230d701f5adf4c69cb86c4412c9e2831028d7a2084c9220a48`  
		Last Modified: Wed, 10 Aug 2022 14:10:33 GMT  
		Size: 2.4 MB (2447708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2375b3b7af35638f4a31108f06f9ff2c9c44ab48e889fc4b603424c0fe13a4bf`  
		Last Modified: Wed, 10 Aug 2022 14:10:32 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd28fec1bea3a7e87491fcbcfccc258fb18db7a477011fd1583abcedba497e`  
		Last Modified: Fri, 19 Aug 2022 06:11:11 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471192fd32321605cdea263d3d59d836c85fcdb6430a3617f767e8061cd9bcdc`  
		Last Modified: Fri, 19 Aug 2022 06:11:12 GMT  
		Size: 704.7 KB (704663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a075f4cdadc577f64fb02a1cebab124392c77e400811511d662f87d5d55847d4`  
		Last Modified: Fri, 19 Aug 2022 06:11:21 GMT  
		Size: 10.5 MB (10474493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0a965c7f189e120dc5a2d3451d798ddbdf117457f4efeb372ad301ff523cff`  
		Last Modified: Fri, 19 Aug 2022 06:11:43 GMT  
		Size: 75.6 MB (75571220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fcd21dfbc607aecc812bec89fe508a2f1a8eae91ea4aeb1d5c689a813426f9`  
		Last Modified: Fri, 19 Aug 2022 06:11:11 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:bb2e47be4baecfdc88b9d698e26fa6e3c913e6a06939f9854709031730c20012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122396337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cbc40902b1f3d2a7cd53b5289b76cf0037487d410a68af848b5c6f803555275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 23:33:51 GMT
ENV NODE_VERSION=14.20.0
# Tue, 09 Aug 2022 23:54:07 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 09 Aug 2022 23:54:07 GMT
ENV YARN_VERSION=1.22.19
# Tue, 09 Aug 2022 23:54:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 09 Aug 2022 23:54:14 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 09 Aug 2022 23:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 23:54:15 GMT
CMD ["node"]
# Wed, 10 Aug 2022 06:59:14 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 10 Aug 2022 06:59:16 GMT
RUN apk add --no-cache 		bash
# Wed, 10 Aug 2022 06:59:16 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:58:45 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:59:14 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:59:15 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:59:16 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:59:17 GMT
ENV GHOST_VERSION=4.48.2
# Fri, 19 Aug 2022 02:55:40 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 19 Aug 2022 02:55:44 GMT
WORKDIR /var/lib/ghost
# Fri, 19 Aug 2022 02:55:46 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 02:55:49 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 02:55:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 02:55:54 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 02:55:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4242f05bf8f81383ae5f83a145e56c06bd56cbbaf842d62336ae61ad5623d7c`  
		Last Modified: Wed, 10 Aug 2022 00:01:53 GMT  
		Size: 37.1 MB (37093903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32b5555b1313bb81b1adaf7d6b227602c820f6d8979c75c8ce0d56badf7393b`  
		Last Modified: Wed, 10 Aug 2022 00:01:47 GMT  
		Size: 2.5 MB (2456916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8b559c1581e3927b80bddba4943c340d93f53c1125df349532aac2d5bfdc22`  
		Last Modified: Wed, 10 Aug 2022 00:01:46 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0efd58105672cf062fb8f45d542eefd8c9f2878d890cc5e96f6932bfe23fb2`  
		Last Modified: Wed, 10 Aug 2022 07:02:30 GMT  
		Size: 11.0 KB (10988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab058ad29d156af9a9eff1d9c7e350c1216fb7497af1a6ab5590c4d6d6d80bc2`  
		Last Modified: Wed, 10 Aug 2022 07:02:31 GMT  
		Size: 826.1 KB (826083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e173c551124981202b7ceaff30a6da436121b2c3ff5ea7bfbbfbfe23e02ff91c`  
		Last Modified: Fri, 12 Aug 2022 01:03:11 GMT  
		Size: 10.5 MB (10475774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a42838339bf48103ea6e3bae7e0ad2d10c42c45ff051ffbfefd897397a6b1e`  
		Last Modified: Fri, 19 Aug 2022 02:57:23 GMT  
		Size: 68.8 MB (68824017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6e519d8dfabf0b5cc1a2a4a8dac016683e37dac1f0daffcc0b00e0b1fb97af`  
		Last Modified: Fri, 19 Aug 2022 02:57:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4.48.2`

```console
$ docker pull ghost@sha256:d256880e794fb870c8e4d9c5b0b5f462f55fbca7f2d47fc78e9a37a04e6c6705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:4.48.2` - linux; amd64

```console
$ docker pull ghost@sha256:b79cc4dc90abfb31c3d96fe1066a0f89ea67e1f65a06d0fee65be33e6daf9012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153118922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ae6b8d721a278fce74d2cad9d4f0c2545fdd21fdcd1fd931fff51d0f0f4b9f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:03:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:08:15 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 04:08:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:08:43 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:08:55 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:08:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:08:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:08:55 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:53:14 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:53:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:53:25 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:53:25 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:53:52 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:53:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:53:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 20:53:53 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 20:54:55 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 20:54:57 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 20:54:57 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 20:54:57 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 20:54:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 20:54:57 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 20:54:57 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065fda631bffac8aa07440d44064117eee8bbfb50d65e04dbd5b29021c0140bf`  
		Last Modified: Tue, 23 Aug 2022 04:12:47 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627ec249bd481d6b9b90895320b0623267b937930af8289419142b25431b5e45`  
		Last Modified: Tue, 23 Aug 2022 04:16:45 GMT  
		Size: 36.1 MB (36066216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:164bac049d8635f1f89f41277cc476550eee2aa272896939c2ce03ab6129b82a`  
		Last Modified: Tue, 23 Aug 2022 04:16:40 GMT  
		Size: 2.8 MB (2792038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d37c9bb493cc0b8f1b8f5f07a95cbedcf4849fb8b1182ad982a92ea24fc9fa`  
		Last Modified: Tue, 23 Aug 2022 04:16:39 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83180ff6457f93520a6f04d7f5b9ed6dcda59611cf83b3b2928c9227f1b834c9`  
		Last Modified: Tue, 23 Aug 2022 20:55:58 GMT  
		Size: 1.4 MB (1448257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb12a4e26b628f8cdeb898d50ccdc7e63bb54b7a7a34a6f7dce42d81189b867`  
		Last Modified: Tue, 23 Aug 2022 20:56:00 GMT  
		Size: 10.5 MB (10474883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7db60bd998f5af0df8ca87809d16c65c18c8d855e400c31d7a85c7fc19a0705`  
		Last Modified: Tue, 23 Aug 2022 20:56:10 GMT  
		Size: 71.0 MB (70950866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a717867f3e188de62caaf05bb6935ceb175bd1ce3050d8c9d3956f069da17c98`  
		Last Modified: Tue, 23 Aug 2022 20:55:57 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48.2` - linux; arm variant v7

```console
$ docker pull ghost@sha256:2074acdffff45db9702ec7563136addb6ec6379b5488b1f671362413b89df37c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166907887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe194b7bd13214424fa5a825c2ead033cdcebab4a50302520a05926f0cbf167`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:44:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 21:51:19 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 21:51:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 21:51:48 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 21:52:00 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 21:52:01 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 21:52:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:52:01 GMT
CMD ["node"]
# Thu, 25 Aug 2022 11:23:48 GMT
ENV GOSU_VERSION=1.12
# Thu, 25 Aug 2022 11:24:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 25 Aug 2022 11:24:04 GMT
ENV NODE_ENV=production
# Thu, 25 Aug 2022 11:24:04 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Thu, 25 Aug 2022 11:24:42 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Thu, 25 Aug 2022 11:24:43 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Thu, 25 Aug 2022 11:24:43 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 25 Aug 2022 11:24:43 GMT
ENV GHOST_VERSION=4.48.2
# Thu, 25 Aug 2022 11:31:24 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 25 Aug 2022 11:31:25 GMT
WORKDIR /var/lib/ghost
# Thu, 25 Aug 2022 11:31:25 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 25 Aug 2022 11:31:26 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Thu, 25 Aug 2022 11:31:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Aug 2022 11:31:26 GMT
EXPOSE 2368
# Thu, 25 Aug 2022 11:31:26 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5221a7a14db5d9fbd6928fcb2921040bb5d801661c018df5b4922f1c0cd73b25`  
		Last Modified: Tue, 23 Aug 2022 22:00:09 GMT  
		Size: 4.2 KB (4168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd95c7a73ed249c57ba223090a89338e0134753b81abf3b6d9fd6f68c2790889`  
		Last Modified: Tue, 23 Aug 2022 22:05:54 GMT  
		Size: 34.2 MB (34226454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c689dd7090fcc73638299bd0b2dea6dace2555089c78c67b63f256766e5f2ed6`  
		Last Modified: Tue, 23 Aug 2022 22:05:45 GMT  
		Size: 2.8 MB (2782975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e14669509146e051ead49dc0000d61beeca1ca9920ce8fcbba53d7d40c3ed66`  
		Last Modified: Tue, 23 Aug 2022 22:05:44 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5033373e37fe063c2e876acd7419e6eab8a89b4c44975b196f26e9681da7693`  
		Last Modified: Thu, 25 Aug 2022 11:34:24 GMT  
		Size: 1.4 MB (1400168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c384dc693fdd0b610909915a4120209458ff6f198ba457a8f2d823c967db99`  
		Last Modified: Thu, 25 Aug 2022 11:34:36 GMT  
		Size: 10.5 MB (10475286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454d6df1620e4006a45000ab178d5fb09f4bd6c1ebe17836da2484c19c0c2a00`  
		Last Modified: Thu, 25 Aug 2022 11:34:56 GMT  
		Size: 91.4 MB (91446106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e880b36e82ebe3ced44fe60025b24d56d75d0dffeb88c7de829fecd61bee22fa`  
		Last Modified: Thu, 25 Aug 2022 11:34:23 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48.2` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:46fb6c1bc0d8782564620dfc6a0ceca81750665722781f66d9d8e7e4abd09ca8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.5 MB (149546600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:168e1856d35603c78cf4f3479dd03a2d00367b176a1bcaabb72df02fe12e17b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:51:52 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:58:36 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 04:59:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:59:04 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:59:17 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:59:18 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:59:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:59:19 GMT
CMD ["node"]
# Tue, 23 Aug 2022 22:21:46 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 22:21:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 22:21:58 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 22:21:59 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 22:22:33 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 22:22:34 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 22:22:35 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 22:22:36 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 22:23:42 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 22:23:45 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 22:23:48 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 22:23:51 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 22:23:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 22:23:56 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 22:23:58 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f232a362cd9820adfd1443fbb1fe468c3175d65fa45259cc218f0b706a0ab11`  
		Last Modified: Tue, 23 Aug 2022 05:08:27 GMT  
		Size: 4.0 KB (4044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb15c1f69124e6198fa23e6d24f9835f6addc53026db7b2fb8a3251b397dc74`  
		Last Modified: Tue, 23 Aug 2022 05:13:16 GMT  
		Size: 36.2 MB (36161922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77315a20631c514f49b1df983a0c0f3037aebe4e83e6d3ce1b4ee73627b18cb`  
		Last Modified: Tue, 23 Aug 2022 05:13:10 GMT  
		Size: 2.8 MB (2791355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebd11967d647dd5cfc6cb25b9af5bbc4ed98395d3059ad661b3ae19057506dd`  
		Last Modified: Tue, 23 Aug 2022 05:13:10 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b22fca5731e39eadceb2d45458c67cadb51c629991c15d27a33c8ba008a0b2`  
		Last Modified: Tue, 23 Aug 2022 22:25:19 GMT  
		Size: 1.4 MB (1383753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e10c3358112d2bca2a7ea242b70718f6f4880ca6df7fe67966368acb90c9438`  
		Last Modified: Tue, 23 Aug 2022 22:25:22 GMT  
		Size: 10.5 MB (10476396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e66dd3c3638a5992c99646ab7e5fd0135fcc3871922907f568e29c9e47b8cac`  
		Last Modified: Tue, 23 Aug 2022 22:25:32 GMT  
		Size: 68.7 MB (68664343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6234a798ea401e9f16986f2b56edfc13398e8fa646ec762baff6826f0d58b5`  
		Last Modified: Tue, 23 Aug 2022 22:25:19 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48.2` - linux; ppc64le

```console
$ docker pull ghost@sha256:9dc5f7cb9b47635f0fe7fdd6665bc3f32ef2cd6021f1dd6cb804b30ffcf13d93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.4 MB (166360663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39a8581db5d39af705e561cb0f74962e65df69c9586b702d5a917c6b8e8bd13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:59:59 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 03:05:13 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 03:05:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 03:05:57 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 03:06:21 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 03:06:22 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 03:06:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 03:06:23 GMT
CMD ["node"]
# Tue, 23 Aug 2022 16:27:11 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 16:27:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 16:27:36 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 16:27:37 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 16:28:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 16:28:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 16:28:29 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 16:28:29 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 16:35:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 16:35:54 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 16:35:55 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 16:35:55 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 16:35:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 16:35:56 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 16:35:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f072867559a95ee18a2f9cafdd6d774dfd46aced3278c83d3652f9b47874402`  
		Last Modified: Tue, 23 Aug 2022 03:11:50 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2272bbef19d126f23a941cd5eb124198e71e91c2b00a9b5253db6205116aa8f4`  
		Last Modified: Tue, 23 Aug 2022 03:15:02 GMT  
		Size: 38.0 MB (37977525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275af2b69ff4c61fae0af3e7d3388f7ce306b3471900336ca0409c263924b61a`  
		Last Modified: Tue, 23 Aug 2022 03:14:53 GMT  
		Size: 2.8 MB (2791986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225c695b0d7dbc52f4dadf5f3a95aba9fbd79ec2bea71e35f6e10953ff86f672`  
		Last Modified: Tue, 23 Aug 2022 03:14:52 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f26aa6f118c17b691193f698e7250a563053aff623d824a63239df6b7d1633`  
		Last Modified: Tue, 23 Aug 2022 16:37:12 GMT  
		Size: 1.4 MB (1367216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bffb191defb74dc8a00ff4dd28c9a4b3e2df2b5a819f09867eb6e2a2e712fd7`  
		Last Modified: Tue, 23 Aug 2022 16:37:17 GMT  
		Size: 10.5 MB (10475288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a72d2148854d00ca569e91fda3d1ce4e5a2ea960321d9bd0fefa4b047235db`  
		Last Modified: Tue, 23 Aug 2022 16:37:37 GMT  
		Size: 78.5 MB (78459185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd6488acf65305851445c7c8aa80845c3637135ffdb92add998e1820dd23cf7`  
		Last Modified: Tue, 23 Aug 2022 16:37:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48.2` - linux; s390x

```console
$ docker pull ghost@sha256:bced498888e99920bb8c2076716e53eb9c4f9c9ed031cea14d9ffa8f31a3658a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.2 MB (158163729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0306fa03f5c798c60ccacd08800f4b3f55d9985b710853196a19440b2e7a68c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 10:34:41 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 10:38:19 GMT
ENV NODE_VERSION=14.20.0
# Tue, 23 Aug 2022 10:38:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 10:38:50 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 10:39:00 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 10:39:00 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 10:39:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 10:39:01 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:54:46 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:55:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:55:12 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:55:13 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:56:23 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:56:28 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:56:29 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 23 Aug 2022 20:56:30 GMT
ENV GHOST_VERSION=4.48.2
# Tue, 23 Aug 2022 21:04:56 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		gosu node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! gosu node yarn add "sqlite3@$sqlite3Version" --force; then 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 		apt-get install -y --no-install-recommends g++ gcc libc-dev libvips-dev make python3; 		rm -rf /var/lib/apt/lists/*; 				gosu node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 23 Aug 2022 21:05:13 GMT
WORKDIR /var/lib/ghost
# Tue, 23 Aug 2022 21:05:14 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 23 Aug 2022 21:05:14 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Tue, 23 Aug 2022 21:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:05:15 GMT
EXPOSE 2368
# Tue, 23 Aug 2022 21:05:15 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c379dfa30c39780b6036486f76caf47f9c913cafd9fc09843e09a18b85d8a95f`  
		Last Modified: Tue, 23 Aug 2022 10:43:30 GMT  
		Size: 4.2 KB (4186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b41927d92a044b983988ff3c801976df26b4312b547721aca871afa8c8abe04`  
		Last Modified: Tue, 23 Aug 2022 10:45:27 GMT  
		Size: 35.9 MB (35930762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcf971b762bf5d61364656e8c639b452d040ec92fc08ed70cafdecbe4170441`  
		Last Modified: Tue, 23 Aug 2022 10:45:23 GMT  
		Size: 2.8 MB (2795017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91be8f7c1b99237a851cae0c77480d132d3acb78b76793184cd97898394522ec`  
		Last Modified: Tue, 23 Aug 2022 10:45:23 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3532d952257c36ce5843da7bf0fd846e190bbe93a8e24fb22812af737cdc0df0`  
		Last Modified: Tue, 23 Aug 2022 21:06:17 GMT  
		Size: 1.4 MB (1435207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464123c020b16d4662f8090d708ca6cf4f1bb2736bb4fd9e601b3b8bf21ae585`  
		Last Modified: Tue, 23 Aug 2022 21:06:19 GMT  
		Size: 10.5 MB (10475352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8478740f82a8ef2317bc10855a3c5a127f3904f2e9b2741f0a7df626b8c87816`  
		Last Modified: Tue, 23 Aug 2022 21:06:30 GMT  
		Size: 77.9 MB (77872109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19773b2df153882c27d1a9915352719c330150694f750ef378531a9841372cbf`  
		Last Modified: Tue, 23 Aug 2022 21:06:17 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:4.48.2-alpine`

```console
$ docker pull ghost@sha256:e88d4940126ce72857bf756704d541bdca735a45f6c1c126c905dc99d3d260df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:4.48.2-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:a26cb9b01baf3790d010d6c99fe1fd295fd51536cd511567858610f8acce25cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125404157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3f1999067d36d71407d9fcd456e8a22c060db9d8b95aa75ebe5cebc97a5516b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 21:03:22 GMT
ENV NODE_VERSION=14.20.0
# Tue, 09 Aug 2022 21:03:30 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 09 Aug 2022 21:03:30 GMT
ENV YARN_VERSION=1.22.19
# Tue, 09 Aug 2022 21:03:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 09 Aug 2022 21:03:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 09 Aug 2022 21:03:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 21:03:34 GMT
CMD ["node"]
# Wed, 10 Aug 2022 03:16:48 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 10 Aug 2022 03:16:49 GMT
RUN apk add --no-cache 		bash
# Wed, 10 Aug 2022 03:16:49 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:30:13 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:30:41 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:30:42 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:30:42 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:30:42 GMT
ENV GHOST_VERSION=4.48.2
# Fri, 19 Aug 2022 00:27:04 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 19 Aug 2022 00:27:06 GMT
WORKDIR /var/lib/ghost
# Fri, 19 Aug 2022 00:27:06 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 00:27:06 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 00:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 00:27:07 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 00:27:07 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb06cd79147098226b90a44ed66cc7ec9f2f4175ee2d90557fd99500e9bd3da`  
		Last Modified: Tue, 09 Aug 2022 21:08:23 GMT  
		Size: 37.2 MB (37234122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765a58e5319058a1ec35459f25ffb310cd052522d9254b4ab11f7055517251bb`  
		Last Modified: Tue, 09 Aug 2022 21:08:18 GMT  
		Size: 2.4 MB (2368736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beee7f5da459e13aa9d48d8d1279ec75df8a68613a996f27e7c20a3246ab1432`  
		Last Modified: Tue, 09 Aug 2022 21:08:17 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516e40f07fa2e3168daff25293ed11e979722e20b781f0233da502442341891c`  
		Last Modified: Wed, 10 Aug 2022 03:19:28 GMT  
		Size: 11.3 KB (11275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66bf249fe1b89c2a761ff737252be2cf8d3c6523fcad38fc0bb6f704141f14c`  
		Last Modified: Wed, 10 Aug 2022 03:19:28 GMT  
		Size: 820.0 KB (820043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2688a29e863f75c4331bc984d1b16d8cf84fec0a151802044c277381ce3257`  
		Last Modified: Fri, 12 Aug 2022 00:33:46 GMT  
		Size: 10.5 MB (10475729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a56dc0c4d2daf7a26a3eb9ce9dfab64c71888cfbbdf37a9f3757b9025adf0b`  
		Last Modified: Fri, 19 Aug 2022 00:28:19 GMT  
		Size: 71.7 MB (71687200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb3827b8e84ea980ee2f03a8310e9128ae4d89eb0b5cfc59683ed2ea1226089`  
		Last Modified: Fri, 19 Aug 2022 00:28:07 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48.2-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:21d46727d65227b34b48bd707881274b1909bd9c48caea910e00c116430fd258
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128705469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1063abd59d1a6b00e8450572875f8413009a6a22146842e9c5e0df767db4f324`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 09:19:32 GMT
ENV NODE_VERSION=14.20.0
# Wed, 10 Aug 2022 11:12:16 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 10 Aug 2022 11:12:16 GMT
ENV YARN_VERSION=1.22.19
# Wed, 10 Aug 2022 11:12:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 10 Aug 2022 11:12:23 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 10 Aug 2022 11:12:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 11:12:23 GMT
CMD ["node"]
# Thu, 11 Aug 2022 01:28:07 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 11 Aug 2022 01:28:08 GMT
RUN apk add --no-cache 		bash
# Thu, 11 Aug 2022 01:28:08 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:04:45 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:06:04 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:06:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:06:05 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:06:05 GMT
ENV GHOST_VERSION=4.48.2
# Fri, 19 Aug 2022 04:04:27 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 19 Aug 2022 04:04:28 GMT
WORKDIR /var/lib/ghost
# Fri, 19 Aug 2022 04:04:29 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 04:04:29 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 04:04:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 04:04:29 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 04:04:29 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3013f82179b5c8924f9d3de2ada926fb916bdf161bf2592ab46dfc11a0e70d87`  
		Last Modified: Wed, 10 Aug 2022 11:15:56 GMT  
		Size: 36.3 MB (36281861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950a175c263694a52363e6903954aacce227330e9ae38f7dc663e7e12ffe1451`  
		Last Modified: Wed, 10 Aug 2022 11:15:49 GMT  
		Size: 2.4 MB (2447687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db221eecf612fb8d7475005c6de72bbaaa455cc937e081cce984ffd0faf58ab7`  
		Last Modified: Wed, 10 Aug 2022 11:15:48 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec39c3839dc8024d012fd6a66fa091cb930ff1f325941985e447902316fee6d2`  
		Last Modified: Fri, 19 Aug 2022 04:05:09 GMT  
		Size: 11.0 KB (10964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fc9db4af048ebdaafc3ac90e5472dcb7b7bb016efe8f434f4ff650e9d901e3`  
		Last Modified: Fri, 19 Aug 2022 04:05:10 GMT  
		Size: 772.0 KB (771994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4318f596df9a2394a8bd2730410d61827c5ba2b7b6995d6e15ad35c5771238f`  
		Last Modified: Fri, 19 Aug 2022 04:05:23 GMT  
		Size: 10.5 MB (10474611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6847c838a915d01366d3ebf51d7840f194c6c6b09bca86a5b4a5420cc651f4b3`  
		Last Modified: Fri, 19 Aug 2022 04:05:33 GMT  
		Size: 76.1 MB (76103388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7a415c5d8fae58acfc30f9e2151c1f95b2c0bb493bbdc1e6c52d0216315de9`  
		Last Modified: Fri, 19 Aug 2022 04:05:09 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48.2-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:16a74cdfeefc8374978d6195378b18bfedf5b915968670977aeedfc8b8c21891
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127477594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:680a135de23810d1d7fc4adb102927520f99cc4764a6a06758599b9c426dd7a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 12:12:46 GMT
ENV NODE_VERSION=14.20.0
# Wed, 10 Aug 2022 14:02:22 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 10 Aug 2022 14:02:23 GMT
ENV YARN_VERSION=1.22.19
# Wed, 10 Aug 2022 14:02:29 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 10 Aug 2022 14:02:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 10 Aug 2022 14:02:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 14:02:29 GMT
CMD ["node"]
# Thu, 11 Aug 2022 04:47:58 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 11 Aug 2022 04:47:59 GMT
RUN apk add --no-cache 		bash
# Thu, 11 Aug 2022 04:47:59 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:32:38 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:33:29 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:33:30 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:33:30 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:33:30 GMT
ENV GHOST_VERSION=4.48.2
# Thu, 18 Aug 2022 22:33:02 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 18 Aug 2022 22:33:04 GMT
WORKDIR /var/lib/ghost
# Thu, 18 Aug 2022 22:33:04 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 06:09:36 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 06:09:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 06:09:36 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 06:09:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a5d5e3efc39633586d718ed087aa8c94ed97eb000bf3912b4ad58c8841a8df`  
		Last Modified: Wed, 10 Aug 2022 14:10:40 GMT  
		Size: 35.9 MB (35850710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e084b1c42c28230d701f5adf4c69cb86c4412c9e2831028d7a2084c9220a48`  
		Last Modified: Wed, 10 Aug 2022 14:10:33 GMT  
		Size: 2.4 MB (2447708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2375b3b7af35638f4a31108f06f9ff2c9c44ab48e889fc4b603424c0fe13a4bf`  
		Last Modified: Wed, 10 Aug 2022 14:10:32 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd28fec1bea3a7e87491fcbcfccc258fb18db7a477011fd1583abcedba497e`  
		Last Modified: Fri, 19 Aug 2022 06:11:11 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471192fd32321605cdea263d3d59d836c85fcdb6430a3617f767e8061cd9bcdc`  
		Last Modified: Fri, 19 Aug 2022 06:11:12 GMT  
		Size: 704.7 KB (704663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a075f4cdadc577f64fb02a1cebab124392c77e400811511d662f87d5d55847d4`  
		Last Modified: Fri, 19 Aug 2022 06:11:21 GMT  
		Size: 10.5 MB (10474493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0a965c7f189e120dc5a2d3451d798ddbdf117457f4efeb372ad301ff523cff`  
		Last Modified: Fri, 19 Aug 2022 06:11:43 GMT  
		Size: 75.6 MB (75571220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fcd21dfbc607aecc812bec89fe508a2f1a8eae91ea4aeb1d5c689a813426f9`  
		Last Modified: Fri, 19 Aug 2022 06:11:11 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4.48.2-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:bb2e47be4baecfdc88b9d698e26fa6e3c913e6a06939f9854709031730c20012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122396337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cbc40902b1f3d2a7cd53b5289b76cf0037487d410a68af848b5c6f803555275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 23:33:51 GMT
ENV NODE_VERSION=14.20.0
# Tue, 09 Aug 2022 23:54:07 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c96fdd6438cb919f4861419b632165697aabb1233d8da6cf3f7886b221416bf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 09 Aug 2022 23:54:07 GMT
ENV YARN_VERSION=1.22.19
# Tue, 09 Aug 2022 23:54:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 09 Aug 2022 23:54:14 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 09 Aug 2022 23:54:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 23:54:15 GMT
CMD ["node"]
# Wed, 10 Aug 2022 06:59:14 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 10 Aug 2022 06:59:16 GMT
RUN apk add --no-cache 		bash
# Wed, 10 Aug 2022 06:59:16 GMT
ENV NODE_ENV=production
# Fri, 12 Aug 2022 00:58:45 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Fri, 12 Aug 2022 00:59:14 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 12 Aug 2022 00:59:15 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 12 Aug 2022 00:59:16 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 12 Aug 2022 00:59:17 GMT
ENV GHOST_VERSION=4.48.2
# Fri, 19 Aug 2022 02:55:40 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 19 Aug 2022 02:55:44 GMT
WORKDIR /var/lib/ghost
# Fri, 19 Aug 2022 02:55:46 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 19 Aug 2022 02:55:49 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 19 Aug 2022 02:55:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 02:55:54 GMT
EXPOSE 2368
# Fri, 19 Aug 2022 02:55:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4242f05bf8f81383ae5f83a145e56c06bd56cbbaf842d62336ae61ad5623d7c`  
		Last Modified: Wed, 10 Aug 2022 00:01:53 GMT  
		Size: 37.1 MB (37093903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32b5555b1313bb81b1adaf7d6b227602c820f6d8979c75c8ce0d56badf7393b`  
		Last Modified: Wed, 10 Aug 2022 00:01:47 GMT  
		Size: 2.5 MB (2456916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8b559c1581e3927b80bddba4943c340d93f53c1125df349532aac2d5bfdc22`  
		Last Modified: Wed, 10 Aug 2022 00:01:46 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0efd58105672cf062fb8f45d542eefd8c9f2878d890cc5e96f6932bfe23fb2`  
		Last Modified: Wed, 10 Aug 2022 07:02:30 GMT  
		Size: 11.0 KB (10988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab058ad29d156af9a9eff1d9c7e350c1216fb7497af1a6ab5590c4d6d6d80bc2`  
		Last Modified: Wed, 10 Aug 2022 07:02:31 GMT  
		Size: 826.1 KB (826083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e173c551124981202b7ceaff30a6da436121b2c3ff5ea7bfbbfbfe23e02ff91c`  
		Last Modified: Fri, 12 Aug 2022 01:03:11 GMT  
		Size: 10.5 MB (10475774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a42838339bf48103ea6e3bae7e0ad2d10c42c45ff051ffbfefd897397a6b1e`  
		Last Modified: Fri, 19 Aug 2022 02:57:23 GMT  
		Size: 68.8 MB (68824017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6e519d8dfabf0b5cc1a2a4a8dac016683e37dac1f0daffcc0b00e0b1fb97af`  
		Last Modified: Fri, 19 Aug 2022 02:57:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:5`

```console
$ docker pull ghost@sha256:073d56e59a5ca2b9cc97ba14ecee8cb27820e0dd99d1064794ef1a5ff67b1600
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ghost:5` - linux; amd64

```console
$ docker pull ghost@sha256:bde8307b90069d5c19f25705d3f9dd2f2f9cb296838649b8820c4a7461c2c950
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148881875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed89eced794e9bf97e4af237e2eb9712deae6419d023306f68e42d87c6bc319a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:03:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:05:45 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 04:06:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:06:12 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:06:24 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:06:24 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:06:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:06:24 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:51:34 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:51:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:51:46 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:51:46 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:52:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:52:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:52:05 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 24 Aug 2022 23:25:08 GMT
ENV GHOST_VERSION=5.11.0
# Wed, 24 Aug 2022 23:26:08 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 24 Aug 2022 23:26:10 GMT
WORKDIR /var/lib/ghost
# Wed, 24 Aug 2022 23:26:10 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 24 Aug 2022 23:26:10 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 24 Aug 2022 23:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 23:26:10 GMT
EXPOSE 2368
# Wed, 24 Aug 2022 23:26:10 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065fda631bffac8aa07440d44064117eee8bbfb50d65e04dbd5b29021c0140bf`  
		Last Modified: Tue, 23 Aug 2022 04:12:47 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8870f8b81b668639dc33301e8197b549f9d7a8fb85598376cc3cccdc8e0282ec`  
		Last Modified: Tue, 23 Aug 2022 04:14:46 GMT  
		Size: 35.3 MB (35348605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1aeb08c8d655334863d3f8cbada8f83783bcbf4daa4c04868a404169c9e97a`  
		Last Modified: Tue, 23 Aug 2022 04:14:41 GMT  
		Size: 2.8 MB (2773386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41346f34487d2de1801efdbb3cc550aa6ba3ac1b5778c7fdb8ed411b7ac1db5`  
		Last Modified: Tue, 23 Aug 2022 04:14:41 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f035609a702017b50a93d64dc01042501c221794129de701d96eb06cd71260`  
		Last Modified: Tue, 23 Aug 2022 20:55:26 GMT  
		Size: 1.4 MB (1448263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c6c0e9e735e43683b9e73b95657123dcb17dcf74ddc911097e695705fcfe09`  
		Last Modified: Tue, 23 Aug 2022 20:55:29 GMT  
		Size: 10.5 MB (10453707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada2c2e4ff48ce35a513530614ff27307d87bace55295c283c2c87fe4302ae5d`  
		Last Modified: Wed, 24 Aug 2022 23:28:11 GMT  
		Size: 67.5 MB (67471253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecfc8400a05eea0ac1181de2080e243f3879d8a309fa4624bedcdf8cebb9006`  
		Last Modified: Wed, 24 Aug 2022 23:28:00 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5` - linux; arm variant v7

```console
$ docker pull ghost@sha256:4a54abec917354a2433b00b8fcd001f45bf05d4bf6c449937f1dd99a414deecd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153136501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448273a23b2dd5ed0daf6fa2fb3a17a801b3d2f1c1c4c425ef6373eddc3bbd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:44:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 21:47:37 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 21:48:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 21:48:11 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 21:48:26 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 21:48:26 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 21:48:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:48:26 GMT
CMD ["node"]
# Thu, 25 Aug 2022 11:06:28 GMT
ENV GOSU_VERSION=1.12
# Thu, 25 Aug 2022 11:06:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 25 Aug 2022 11:06:44 GMT
ENV NODE_ENV=production
# Thu, 25 Aug 2022 11:06:44 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Thu, 25 Aug 2022 11:07:11 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Thu, 25 Aug 2022 11:07:11 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Thu, 25 Aug 2022 11:07:11 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 25 Aug 2022 11:07:11 GMT
ENV GHOST_VERSION=5.11.0
# Thu, 25 Aug 2022 11:13:52 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 25 Aug 2022 11:13:53 GMT
WORKDIR /var/lib/ghost
# Thu, 25 Aug 2022 11:13:53 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 25 Aug 2022 11:13:53 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Thu, 25 Aug 2022 11:13:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Aug 2022 11:13:54 GMT
EXPOSE 2368
# Thu, 25 Aug 2022 11:13:54 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5221a7a14db5d9fbd6928fcb2921040bb5d801661c018df5b4922f1c0cd73b25`  
		Last Modified: Tue, 23 Aug 2022 22:00:09 GMT  
		Size: 4.2 KB (4168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620dcb50c9c7f1bbeb5e2b5a12e7fa08bf27a468bfc8ed3fbf439d1bc082c1b8`  
		Last Modified: Tue, 23 Aug 2022 22:03:06 GMT  
		Size: 32.6 MB (32573345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca57e71c998e1a076aed800c650e8758b6b6917356581b7b29d4aef537581df`  
		Last Modified: Tue, 23 Aug 2022 22:02:59 GMT  
		Size: 2.8 MB (2767232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59650dc6a524a79de3b9d5c0d5589cdb9003948e9d9e55cec41b494e6c060ed`  
		Last Modified: Tue, 23 Aug 2022 22:02:58 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865fed7c0dce56885134704e18d70ae963d20bf39dc80adb1fc43df2259f2f66`  
		Last Modified: Thu, 25 Aug 2022 11:32:29 GMT  
		Size: 1.4 MB (1400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d24704e6b17ee2bb7332099b285f0d2f47157d7aa6ece29c99174dcd59ba765`  
		Last Modified: Thu, 25 Aug 2022 11:32:43 GMT  
		Size: 10.5 MB (10458318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0157d1c1f9ddbddbe2547095e20a9fc215bde7581c6092e70f81f5096e48aa79`  
		Last Modified: Thu, 25 Aug 2022 11:33:10 GMT  
		Size: 79.4 MB (79360512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6255ec21dad79c58ec4d433176949dcecff5be2631f540b954d461b9ed2a5eb5`  
		Last Modified: Thu, 25 Aug 2022 11:32:28 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:6ef301ab3555fb1636b918d719174614be61b661da5fda1b6bcf8d8dcbbee4d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156157808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b43780b59a0b8d89594337ce2aae1e92435588df8050c36281a62464b69b5975`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:51:52 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:55:16 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 04:55:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:55:43 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:55:55 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:55:57 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:55:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:55:58 GMT
CMD ["node"]
# Tue, 23 Aug 2022 22:17:12 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 22:17:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 22:17:24 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 22:17:25 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 22:17:44 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 22:17:45 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 22:17:46 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:52:35 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 21:56:20 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 21:56:24 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 21:56:26 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 21:56:29 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 26 Aug 2022 21:56:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 21:56:34 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 21:56:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f232a362cd9820adfd1443fbb1fe468c3175d65fa45259cc218f0b706a0ab11`  
		Last Modified: Tue, 23 Aug 2022 05:08:27 GMT  
		Size: 4.0 KB (4044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa653d801310584a170e38c681b10894b2a77ef836273f9d199c0c6a47904094`  
		Last Modified: Tue, 23 Aug 2022 05:10:51 GMT  
		Size: 35.5 MB (35495106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25750f98abe8642e2ad2e8b0311e2f33bf18a485553993e1d2a92b7f16e71a74`  
		Last Modified: Tue, 23 Aug 2022 05:10:46 GMT  
		Size: 2.8 MB (2772303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476cb0003ed3a2e40214ba9063e0bb0f5542ef59f6c33588c076664260ba176d`  
		Last Modified: Tue, 23 Aug 2022 05:10:45 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24b540e3d30c4849b45592e96ea7f677993457b4c161935ec2d8b536aa49a72`  
		Last Modified: Tue, 23 Aug 2022 22:24:44 GMT  
		Size: 1.4 MB (1383735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba84c7d5d4ca00a02d329912660d788c3509eb8325a6064d97b0058b45a5474`  
		Last Modified: Tue, 23 Aug 2022 22:24:47 GMT  
		Size: 10.5 MB (10454579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af36c284258f664c6fe8c7eb63689c98d1595fcc65079657bf8eb84891c11db`  
		Last Modified: Fri, 26 Aug 2022 22:02:51 GMT  
		Size: 76.0 MB (75983259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a71325e5f20be54324fbc5ff1dc747e0b03cc691d7472e3b19fc277d9cd6714`  
		Last Modified: Fri, 26 Aug 2022 22:02:36 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5` - linux; ppc64le

```console
$ docker pull ghost@sha256:4c08885ac69ee4aedf606dceb6b9be3c977cdc5ac80a9ff37e31219c08e686d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152708772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ebce572687b5e88fa7ccca994f0934d575d4569b0d9ff808b6753598e5d9614`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:59:59 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 03:02:23 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 03:03:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 03:03:06 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 03:03:31 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 03:03:32 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 03:03:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 03:03:32 GMT
CMD ["node"]
# Tue, 23 Aug 2022 16:17:13 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 16:17:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 16:17:39 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 16:17:39 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 16:18:10 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 16:18:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 16:18:13 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 24 Aug 2022 22:32:20 GMT
ENV GHOST_VERSION=5.11.0
# Wed, 24 Aug 2022 22:41:03 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 24 Aug 2022 22:41:11 GMT
WORKDIR /var/lib/ghost
# Wed, 24 Aug 2022 22:41:11 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 24 Aug 2022 22:41:12 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 24 Aug 2022 22:41:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 22:41:13 GMT
EXPOSE 2368
# Wed, 24 Aug 2022 22:41:13 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f072867559a95ee18a2f9cafdd6d774dfd46aced3278c83d3652f9b47874402`  
		Last Modified: Tue, 23 Aug 2022 03:11:50 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d672ed322507d9fe8d9cc50c2c0322dec911843f285809f396eb5a24276fb39`  
		Last Modified: Tue, 23 Aug 2022 03:13:44 GMT  
		Size: 37.4 MB (37413541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc6f3d892c304e25ca4018d68093a08ef0abf6a685d03b687052a6aedd78ff5`  
		Last Modified: Tue, 23 Aug 2022 03:13:35 GMT  
		Size: 2.8 MB (2773489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d242eaa1a1d467ce825da0390583291c07bafbdbbd6068577e58f6ef6a946ecb`  
		Last Modified: Tue, 23 Aug 2022 03:13:34 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c0c8ea85d5ad4979cd20a465ac7f6b1a2521dc080589bda90263b276ba273`  
		Last Modified: Tue, 23 Aug 2022 16:36:28 GMT  
		Size: 1.4 MB (1367219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e03d4bcc0b171c0ee68bbb4704f0cea8c2ab9bcc309eef80488699529c12336`  
		Last Modified: Tue, 23 Aug 2022 16:36:33 GMT  
		Size: 10.5 MB (10459153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee6f3f210367839f64ed97b02829a92708d8c76b3961744ffc05e115470da36`  
		Last Modified: Wed, 24 Aug 2022 22:42:17 GMT  
		Size: 65.4 MB (65405908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35d75685c112e934f6d660e7b6467cb9859a59876d5cc7d4e78e40507e7eb66`  
		Last Modified: Wed, 24 Aug 2022 22:41:54 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5` - linux; s390x

```console
$ docker pull ghost@sha256:e3a777ad6e2680d2fdd419c185def4d44e81821f6a9500da89fa36ee9b783058
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144902229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7213ae4b9752d1be299eb0fd729e03ed2719f8c381fd5c19b0661eec496cec53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 10:34:41 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 10:36:25 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 10:36:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 10:36:46 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 10:36:54 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 10:36:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 10:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 10:36:55 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:43:29 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:43:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:43:57 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:43:57 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:44:40 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:44:48 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:44:48 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:46:48 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 21:50:32 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 21:50:40 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 21:50:40 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 21:50:40 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 26 Aug 2022 21:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 21:50:40 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 21:50:40 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c379dfa30c39780b6036486f76caf47f9c913cafd9fc09843e09a18b85d8a95f`  
		Last Modified: Tue, 23 Aug 2022 10:43:30 GMT  
		Size: 4.2 KB (4186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5f681357b689bb7539d1e20b4cadedd292b61a3c69b5708498366d6fd7d79c`  
		Last Modified: Tue, 23 Aug 2022 10:44:37 GMT  
		Size: 35.2 MB (35242738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924401253b9a620a330a5140a4a4f698349610df8872c46039c6aeb87a94a351`  
		Last Modified: Tue, 23 Aug 2022 10:44:33 GMT  
		Size: 2.8 MB (2775220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60f8644f086e6d183d4c2ec8835e42eb82d5f98dd837d727bbeaa76de2d1a3`  
		Last Modified: Tue, 23 Aug 2022 10:44:32 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0967c4f7d945eda8be25366902a136d8a8813486bce0cc4037762d23efbe3442`  
		Last Modified: Tue, 23 Aug 2022 21:05:53 GMT  
		Size: 1.4 MB (1435147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd66868ffb16cd3f9211d5304900f8dcabe3f55da8d322f1d801e5eba0691e1`  
		Last Modified: Tue, 23 Aug 2022 21:05:55 GMT  
		Size: 10.5 MB (10460473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0240bf01c75304f3cb51b17bfc8f37926c97384d908ce268a2d48ef2938f892`  
		Last Modified: Fri, 26 Aug 2022 21:51:27 GMT  
		Size: 65.3 MB (65333373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cf4c8cf40a063c9ce1736e080b0287408cb5d9554a49c75c05431393c38c48`  
		Last Modified: Fri, 26 Aug 2022 21:51:16 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:5-alpine`

```console
$ docker pull ghost@sha256:05702fcd8b36c375e67d802dc509b1cd3fca75a5120c351b345438833a4022a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:5-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:5cbea95e17628ed41c89b036080b704dc5de4ac1931657304da3909f17909c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (121048344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0216d33e59a2c6040a2ce8da935038b3f5a824666393fdb86ada484e83383e38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 16 Aug 2022 23:35:38 GMT
ENV NODE_VERSION=16.17.0
# Tue, 16 Aug 2022 23:35:45 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 16 Aug 2022 23:35:46 GMT
ENV YARN_VERSION=1.22.19
# Tue, 16 Aug 2022 23:35:50 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 16 Aug 2022 23:35:50 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 16 Aug 2022 23:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 Aug 2022 23:35:50 GMT
CMD ["node"]
# Wed, 17 Aug 2022 00:25:36 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 00:25:37 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 00:25:37 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 00:25:38 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 00:25:55 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 00:25:55 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 00:25:56 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 24 Aug 2022 23:26:17 GMT
ENV GHOST_VERSION=5.11.0
# Wed, 24 Aug 2022 23:27:24 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 24 Aug 2022 23:27:26 GMT
WORKDIR /var/lib/ghost
# Wed, 24 Aug 2022 23:27:26 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 24 Aug 2022 23:27:26 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 24 Aug 2022 23:27:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 23:27:27 GMT
EXPOSE 2368
# Wed, 24 Aug 2022 23:27:27 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864b973d1bf1f32e9e7938e6f158ecf7b2503fbbe7799aacbf1fe853f506f398`  
		Last Modified: Tue, 16 Aug 2022 23:41:04 GMT  
		Size: 36.4 MB (36447059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fe61ad56f50607679112c84f9b17b0dc5f9f2c130e875aa8d2d49d43a8fbbd`  
		Last Modified: Tue, 16 Aug 2022 23:40:59 GMT  
		Size: 2.4 MB (2350967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3887ab559e662a183c826648d3d51ba916a9be9119c1349b63ad6ca2c1c6c32`  
		Last Modified: Tue, 16 Aug 2022 23:40:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0934c2dd904c5efc297df956ff406bc4612835aef251c5fdefb18325930d42a6`  
		Last Modified: Wed, 17 Aug 2022 00:28:02 GMT  
		Size: 11.3 KB (11279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2212eaaa6ff840552d707d93915cb7ab73b7ab30b5dd8bee5791ef6e7f77b4e0`  
		Last Modified: Wed, 17 Aug 2022 00:28:02 GMT  
		Size: 820.0 KB (820039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f91237b7e346ccbacb16136605b73c0ef6bb3c24801d331990385ef5614205`  
		Last Modified: Wed, 17 Aug 2022 00:28:05 GMT  
		Size: 10.5 MB (10453252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed9260d182f293ca9db9b7d44631fcd0b720db204f1b338f83ed8bc5330f66`  
		Last Modified: Wed, 24 Aug 2022 23:28:39 GMT  
		Size: 68.2 MB (68158694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af63d868d813e102a89546302d93bfef19deb775d4c3a36fa9ae19dad1a46f5`  
		Last Modified: Wed, 24 Aug 2022 23:28:26 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:b7cdd7a7ae670cf833f839b3cf3c5e15b5f9c1ae0d1b220d32dd4b701e21d562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115171904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36c4534571a9c97ad0dd3111039423ef7c7486ae058e5e46330ad179ec82023`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 05:42:56 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 08:33:31 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 08:33:31 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 08:33:38 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 08:33:38 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 08:33:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 08:33:38 GMT
CMD ["node"]
# Wed, 17 Aug 2022 08:37:49 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 08:37:51 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 08:37:51 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 08:37:51 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 08:38:52 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 08:38:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 08:38:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:55:05 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 22:05:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 22:05:08 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 22:05:08 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 22:05:09 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 26 Aug 2022 22:05:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 22:05:09 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 22:05:09 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0242dcb01a33bec13ceb8fea51cdfbdac1677423e322b07dc334b0cb67aec642`  
		Last Modified: Wed, 17 Aug 2022 08:36:51 GMT  
		Size: 35.4 MB (35430982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612fd2e24f9da53aeff556efe5d18ef95264e831be9eba4c8bced3c9aabf4b22`  
		Last Modified: Wed, 17 Aug 2022 08:36:44 GMT  
		Size: 2.4 MB (2431032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89adb15822bd2887be78a2b8b70777482a8a6b84490d1210c54d93c6fd7177a5`  
		Last Modified: Wed, 17 Aug 2022 08:36:42 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350c39d4194c2030fff551020327a74cd025a79ce950690a6548f7341b197e5c`  
		Last Modified: Wed, 17 Aug 2022 08:59:08 GMT  
		Size: 11.0 KB (10961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e0405fab6a93ba6b0ce37c0803e29b5500f43fd8aac23f9f998281015d0cd6`  
		Last Modified: Wed, 17 Aug 2022 08:59:09 GMT  
		Size: 772.0 KB (771989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd866b6c9473c76325836db455955454bf064ebde704c9909583fec3e8f7f13`  
		Last Modified: Wed, 17 Aug 2022 08:59:22 GMT  
		Size: 10.5 MB (10459688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c7e973f13d211e59855a80a94364e31c6e6a1a3a2dfec7b989c58c58fafefe`  
		Last Modified: Fri, 26 Aug 2022 22:06:08 GMT  
		Size: 63.5 MB (63452287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b124ba258bf3feadd20db14b3ba2afa43271af465b2bb4c283b80b3551a3b80`  
		Last Modified: Fri, 26 Aug 2022 22:05:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:e81be4dbd26ed1bfecb149da0248ca35082bd837550c566e79e401d7afc4ff7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.2 MB (114154756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3aa4cadae8a2cece6c5078f11127c57f3999e33595e7a7c54fcd0d85f9d92b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 08:51:37 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 11:44:06 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 11:44:06 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 11:44:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 11:44:12 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 11:44:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 11:44:12 GMT
CMD ["node"]
# Wed, 17 Aug 2022 12:07:15 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 12:07:16 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 12:07:16 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 12:07:16 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 12:07:40 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 12:07:41 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 12:07:41 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 25 Aug 2022 11:14:07 GMT
ENV GHOST_VERSION=5.11.0
# Thu, 25 Aug 2022 11:23:38 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 25 Aug 2022 11:23:39 GMT
WORKDIR /var/lib/ghost
# Thu, 25 Aug 2022 11:23:40 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 25 Aug 2022 11:23:40 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 25 Aug 2022 11:23:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Aug 2022 11:23:40 GMT
EXPOSE 2368
# Thu, 25 Aug 2022 11:23:40 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af62c2a8a93c8d8d84c4b7f3ea2d40da7355f049477c23dad411d59b2687619`  
		Last Modified: Wed, 17 Aug 2022 11:54:27 GMT  
		Size: 35.0 MB (34960433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecbe39d3f57b92a197c93a31ce4457cc2042c1e806fe36620e43e5170583fd4`  
		Last Modified: Wed, 17 Aug 2022 11:54:19 GMT  
		Size: 2.4 MB (2430938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b335659237c4596ce2b2c2a58cd9122a83e828f0433d10ed23121fe84900076`  
		Last Modified: Wed, 17 Aug 2022 11:54:18 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac45770c5da644dce686ca3b1f3f229f2606c92601a302ad6bfba78e7eb80136`  
		Last Modified: Wed, 17 Aug 2022 12:20:08 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986eb734888fa41d4980b8f4ed215b85de0db92a44dec53d2de8542e51d8936f`  
		Last Modified: Wed, 17 Aug 2022 12:20:09 GMT  
		Size: 704.7 KB (704656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9dbc2371a118885185eed934e1de1597c58263dee5ff2ffbb2704f69899eef`  
		Last Modified: Wed, 17 Aug 2022 12:20:18 GMT  
		Size: 10.5 MB (10457009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cd01b20c32d3a9cf594fabc2fb4e8be18d02616504092fed3b8f0d92877eac`  
		Last Modified: Thu, 25 Aug 2022 11:34:03 GMT  
		Size: 63.2 MB (63172927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d75ea7e56b3dc33396e3df3fd241d73dd69d989c4d2009101a016142833276`  
		Last Modified: Thu, 25 Aug 2022 11:33:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:101aeb094f23c3ad06cac7bff69199738ec7f2cb406b7b1df1a19440d1a55fd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128143191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7827ca61839c38a612c5adb293035b079b78741745a8b6809cc820cb18e63f42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 00:49:14 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 01:19:27 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 01:19:28 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 01:19:32 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 01:19:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 01:19:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 01:19:35 GMT
CMD ["node"]
# Wed, 17 Aug 2022 02:27:45 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 02:27:47 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 02:27:47 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 02:27:48 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 02:28:07 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 02:28:08 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 02:28:09 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:56:47 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 22:01:30 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 22:01:33 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 22:01:35 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 22:01:37 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 26 Aug 2022 22:01:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 22:01:42 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 22:01:44 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bbdc18f3e0d876c6dd22cb80843cd39643602e791488600c523655514f1f31`  
		Last Modified: Wed, 17 Aug 2022 01:28:14 GMT  
		Size: 36.3 MB (36344502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb54f68a6fc352431a291f292597a7445894ab233ad63742943345a8adfe34b8`  
		Last Modified: Wed, 17 Aug 2022 01:28:09 GMT  
		Size: 2.4 MB (2440157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6c5903b8c0ef8e2e35ecf2ba7b484d0732333f44224b7bbd07cab3fc8980d0`  
		Last Modified: Wed, 17 Aug 2022 01:28:09 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822d0cbaa1675e44af4152ee9e2678b3e94940c75977aedf8a2161c4bdcb0ae8`  
		Last Modified: Wed, 17 Aug 2022 02:34:20 GMT  
		Size: 11.0 KB (10988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f5ed121dd729b06bf5c0fa31d95f6a2269739d68eb5bf2dc884c57c02b9e39`  
		Last Modified: Wed, 17 Aug 2022 02:34:21 GMT  
		Size: 826.1 KB (826078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b760c5860186be667d6be0e7933199cc6bf74bc0c997ddb4d5eac6232b882`  
		Last Modified: Wed, 17 Aug 2022 02:34:24 GMT  
		Size: 10.5 MB (10454441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4140a1d88f4c96f6ce1ab4d5322427a93b95ed9bacce56133c9860a2f658f7`  
		Last Modified: Fri, 26 Aug 2022 22:03:23 GMT  
		Size: 75.4 MB (75358365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094f4a7e5552544716eccb4169a4d80f632487a9f4b5f0aca504be92343d11e6`  
		Last Modified: Fri, 26 Aug 2022 22:03:09 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:5.12`

```console
$ docker pull ghost@sha256:f3b389d8bf036ab72f08e133e061b06ac5f8227f42c128ba65f08c8c595ce9e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm64 variant v8
	-	linux; s390x

### `ghost:5.12` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:6ef301ab3555fb1636b918d719174614be61b661da5fda1b6bcf8d8dcbbee4d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156157808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b43780b59a0b8d89594337ce2aae1e92435588df8050c36281a62464b69b5975`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:51:52 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:55:16 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 04:55:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:55:43 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:55:55 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:55:57 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:55:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:55:58 GMT
CMD ["node"]
# Tue, 23 Aug 2022 22:17:12 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 22:17:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 22:17:24 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 22:17:25 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 22:17:44 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 22:17:45 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 22:17:46 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:52:35 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 21:56:20 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 21:56:24 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 21:56:26 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 21:56:29 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 26 Aug 2022 21:56:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 21:56:34 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 21:56:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f232a362cd9820adfd1443fbb1fe468c3175d65fa45259cc218f0b706a0ab11`  
		Last Modified: Tue, 23 Aug 2022 05:08:27 GMT  
		Size: 4.0 KB (4044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa653d801310584a170e38c681b10894b2a77ef836273f9d199c0c6a47904094`  
		Last Modified: Tue, 23 Aug 2022 05:10:51 GMT  
		Size: 35.5 MB (35495106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25750f98abe8642e2ad2e8b0311e2f33bf18a485553993e1d2a92b7f16e71a74`  
		Last Modified: Tue, 23 Aug 2022 05:10:46 GMT  
		Size: 2.8 MB (2772303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476cb0003ed3a2e40214ba9063e0bb0f5542ef59f6c33588c076664260ba176d`  
		Last Modified: Tue, 23 Aug 2022 05:10:45 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24b540e3d30c4849b45592e96ea7f677993457b4c161935ec2d8b536aa49a72`  
		Last Modified: Tue, 23 Aug 2022 22:24:44 GMT  
		Size: 1.4 MB (1383735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba84c7d5d4ca00a02d329912660d788c3509eb8325a6064d97b0058b45a5474`  
		Last Modified: Tue, 23 Aug 2022 22:24:47 GMT  
		Size: 10.5 MB (10454579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af36c284258f664c6fe8c7eb63689c98d1595fcc65079657bf8eb84891c11db`  
		Last Modified: Fri, 26 Aug 2022 22:02:51 GMT  
		Size: 76.0 MB (75983259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a71325e5f20be54324fbc5ff1dc747e0b03cc691d7472e3b19fc277d9cd6714`  
		Last Modified: Fri, 26 Aug 2022 22:02:36 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5.12` - linux; s390x

```console
$ docker pull ghost@sha256:e3a777ad6e2680d2fdd419c185def4d44e81821f6a9500da89fa36ee9b783058
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144902229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7213ae4b9752d1be299eb0fd729e03ed2719f8c381fd5c19b0661eec496cec53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 10:34:41 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 10:36:25 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 10:36:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 10:36:46 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 10:36:54 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 10:36:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 10:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 10:36:55 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:43:29 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:43:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:43:57 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:43:57 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:44:40 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:44:48 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:44:48 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:46:48 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 21:50:32 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 21:50:40 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 21:50:40 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 21:50:40 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 26 Aug 2022 21:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 21:50:40 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 21:50:40 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c379dfa30c39780b6036486f76caf47f9c913cafd9fc09843e09a18b85d8a95f`  
		Last Modified: Tue, 23 Aug 2022 10:43:30 GMT  
		Size: 4.2 KB (4186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5f681357b689bb7539d1e20b4cadedd292b61a3c69b5708498366d6fd7d79c`  
		Last Modified: Tue, 23 Aug 2022 10:44:37 GMT  
		Size: 35.2 MB (35242738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924401253b9a620a330a5140a4a4f698349610df8872c46039c6aeb87a94a351`  
		Last Modified: Tue, 23 Aug 2022 10:44:33 GMT  
		Size: 2.8 MB (2775220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60f8644f086e6d183d4c2ec8835e42eb82d5f98dd837d727bbeaa76de2d1a3`  
		Last Modified: Tue, 23 Aug 2022 10:44:32 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0967c4f7d945eda8be25366902a136d8a8813486bce0cc4037762d23efbe3442`  
		Last Modified: Tue, 23 Aug 2022 21:05:53 GMT  
		Size: 1.4 MB (1435147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd66868ffb16cd3f9211d5304900f8dcabe3f55da8d322f1d801e5eba0691e1`  
		Last Modified: Tue, 23 Aug 2022 21:05:55 GMT  
		Size: 10.5 MB (10460473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0240bf01c75304f3cb51b17bfc8f37926c97384d908ce268a2d48ef2938f892`  
		Last Modified: Fri, 26 Aug 2022 21:51:27 GMT  
		Size: 65.3 MB (65333373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cf4c8cf40a063c9ce1736e080b0287408cb5d9554a49c75c05431393c38c48`  
		Last Modified: Fri, 26 Aug 2022 21:51:16 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:5.12-alpine`

```console
$ docker pull ghost@sha256:4e9dc911a54f89224bf4552e72a155d9c2b9ff29ce5f034e8c5055e24d861f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `ghost:5.12-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:b7cdd7a7ae670cf833f839b3cf3c5e15b5f9c1ae0d1b220d32dd4b701e21d562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115171904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36c4534571a9c97ad0dd3111039423ef7c7486ae058e5e46330ad179ec82023`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 05:42:56 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 08:33:31 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 08:33:31 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 08:33:38 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 08:33:38 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 08:33:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 08:33:38 GMT
CMD ["node"]
# Wed, 17 Aug 2022 08:37:49 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 08:37:51 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 08:37:51 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 08:37:51 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 08:38:52 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 08:38:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 08:38:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:55:05 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 22:05:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 22:05:08 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 22:05:08 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 22:05:09 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 26 Aug 2022 22:05:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 22:05:09 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 22:05:09 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0242dcb01a33bec13ceb8fea51cdfbdac1677423e322b07dc334b0cb67aec642`  
		Last Modified: Wed, 17 Aug 2022 08:36:51 GMT  
		Size: 35.4 MB (35430982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612fd2e24f9da53aeff556efe5d18ef95264e831be9eba4c8bced3c9aabf4b22`  
		Last Modified: Wed, 17 Aug 2022 08:36:44 GMT  
		Size: 2.4 MB (2431032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89adb15822bd2887be78a2b8b70777482a8a6b84490d1210c54d93c6fd7177a5`  
		Last Modified: Wed, 17 Aug 2022 08:36:42 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350c39d4194c2030fff551020327a74cd025a79ce950690a6548f7341b197e5c`  
		Last Modified: Wed, 17 Aug 2022 08:59:08 GMT  
		Size: 11.0 KB (10961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e0405fab6a93ba6b0ce37c0803e29b5500f43fd8aac23f9f998281015d0cd6`  
		Last Modified: Wed, 17 Aug 2022 08:59:09 GMT  
		Size: 772.0 KB (771989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd866b6c9473c76325836db455955454bf064ebde704c9909583fec3e8f7f13`  
		Last Modified: Wed, 17 Aug 2022 08:59:22 GMT  
		Size: 10.5 MB (10459688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c7e973f13d211e59855a80a94364e31c6e6a1a3a2dfec7b989c58c58fafefe`  
		Last Modified: Fri, 26 Aug 2022 22:06:08 GMT  
		Size: 63.5 MB (63452287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b124ba258bf3feadd20db14b3ba2afa43271af465b2bb4c283b80b3551a3b80`  
		Last Modified: Fri, 26 Aug 2022 22:05:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5.12-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:101aeb094f23c3ad06cac7bff69199738ec7f2cb406b7b1df1a19440d1a55fd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128143191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7827ca61839c38a612c5adb293035b079b78741745a8b6809cc820cb18e63f42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 00:49:14 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 01:19:27 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 01:19:28 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 01:19:32 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 01:19:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 01:19:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 01:19:35 GMT
CMD ["node"]
# Wed, 17 Aug 2022 02:27:45 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 02:27:47 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 02:27:47 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 02:27:48 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 02:28:07 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 02:28:08 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 02:28:09 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:56:47 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 22:01:30 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 22:01:33 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 22:01:35 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 22:01:37 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 26 Aug 2022 22:01:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 22:01:42 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 22:01:44 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bbdc18f3e0d876c6dd22cb80843cd39643602e791488600c523655514f1f31`  
		Last Modified: Wed, 17 Aug 2022 01:28:14 GMT  
		Size: 36.3 MB (36344502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb54f68a6fc352431a291f292597a7445894ab233ad63742943345a8adfe34b8`  
		Last Modified: Wed, 17 Aug 2022 01:28:09 GMT  
		Size: 2.4 MB (2440157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6c5903b8c0ef8e2e35ecf2ba7b484d0732333f44224b7bbd07cab3fc8980d0`  
		Last Modified: Wed, 17 Aug 2022 01:28:09 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822d0cbaa1675e44af4152ee9e2678b3e94940c75977aedf8a2161c4bdcb0ae8`  
		Last Modified: Wed, 17 Aug 2022 02:34:20 GMT  
		Size: 11.0 KB (10988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f5ed121dd729b06bf5c0fa31d95f6a2269739d68eb5bf2dc884c57c02b9e39`  
		Last Modified: Wed, 17 Aug 2022 02:34:21 GMT  
		Size: 826.1 KB (826078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b760c5860186be667d6be0e7933199cc6bf74bc0c997ddb4d5eac6232b882`  
		Last Modified: Wed, 17 Aug 2022 02:34:24 GMT  
		Size: 10.5 MB (10454441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4140a1d88f4c96f6ce1ab4d5322427a93b95ed9bacce56133c9860a2f658f7`  
		Last Modified: Fri, 26 Aug 2022 22:03:23 GMT  
		Size: 75.4 MB (75358365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094f4a7e5552544716eccb4169a4d80f632487a9f4b5f0aca504be92343d11e6`  
		Last Modified: Fri, 26 Aug 2022 22:03:09 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:5.12.0`

```console
$ docker pull ghost@sha256:f3b389d8bf036ab72f08e133e061b06ac5f8227f42c128ba65f08c8c595ce9e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm64 variant v8
	-	linux; s390x

### `ghost:5.12.0` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:6ef301ab3555fb1636b918d719174614be61b661da5fda1b6bcf8d8dcbbee4d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156157808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b43780b59a0b8d89594337ce2aae1e92435588df8050c36281a62464b69b5975`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:51:52 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:55:16 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 04:55:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:55:43 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:55:55 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:55:57 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:55:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:55:58 GMT
CMD ["node"]
# Tue, 23 Aug 2022 22:17:12 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 22:17:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 22:17:24 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 22:17:25 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 22:17:44 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 22:17:45 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 22:17:46 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:52:35 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 21:56:20 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 21:56:24 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 21:56:26 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 21:56:29 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 26 Aug 2022 21:56:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 21:56:34 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 21:56:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f232a362cd9820adfd1443fbb1fe468c3175d65fa45259cc218f0b706a0ab11`  
		Last Modified: Tue, 23 Aug 2022 05:08:27 GMT  
		Size: 4.0 KB (4044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa653d801310584a170e38c681b10894b2a77ef836273f9d199c0c6a47904094`  
		Last Modified: Tue, 23 Aug 2022 05:10:51 GMT  
		Size: 35.5 MB (35495106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25750f98abe8642e2ad2e8b0311e2f33bf18a485553993e1d2a92b7f16e71a74`  
		Last Modified: Tue, 23 Aug 2022 05:10:46 GMT  
		Size: 2.8 MB (2772303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476cb0003ed3a2e40214ba9063e0bb0f5542ef59f6c33588c076664260ba176d`  
		Last Modified: Tue, 23 Aug 2022 05:10:45 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24b540e3d30c4849b45592e96ea7f677993457b4c161935ec2d8b536aa49a72`  
		Last Modified: Tue, 23 Aug 2022 22:24:44 GMT  
		Size: 1.4 MB (1383735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba84c7d5d4ca00a02d329912660d788c3509eb8325a6064d97b0058b45a5474`  
		Last Modified: Tue, 23 Aug 2022 22:24:47 GMT  
		Size: 10.5 MB (10454579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af36c284258f664c6fe8c7eb63689c98d1595fcc65079657bf8eb84891c11db`  
		Last Modified: Fri, 26 Aug 2022 22:02:51 GMT  
		Size: 76.0 MB (75983259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a71325e5f20be54324fbc5ff1dc747e0b03cc691d7472e3b19fc277d9cd6714`  
		Last Modified: Fri, 26 Aug 2022 22:02:36 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5.12.0` - linux; s390x

```console
$ docker pull ghost@sha256:e3a777ad6e2680d2fdd419c185def4d44e81821f6a9500da89fa36ee9b783058
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144902229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7213ae4b9752d1be299eb0fd729e03ed2719f8c381fd5c19b0661eec496cec53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 10:34:41 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 10:36:25 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 10:36:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 10:36:46 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 10:36:54 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 10:36:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 10:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 10:36:55 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:43:29 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:43:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:43:57 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:43:57 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:44:40 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:44:48 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:44:48 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:46:48 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 21:50:32 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 21:50:40 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 21:50:40 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 21:50:40 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 26 Aug 2022 21:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 21:50:40 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 21:50:40 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c379dfa30c39780b6036486f76caf47f9c913cafd9fc09843e09a18b85d8a95f`  
		Last Modified: Tue, 23 Aug 2022 10:43:30 GMT  
		Size: 4.2 KB (4186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5f681357b689bb7539d1e20b4cadedd292b61a3c69b5708498366d6fd7d79c`  
		Last Modified: Tue, 23 Aug 2022 10:44:37 GMT  
		Size: 35.2 MB (35242738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924401253b9a620a330a5140a4a4f698349610df8872c46039c6aeb87a94a351`  
		Last Modified: Tue, 23 Aug 2022 10:44:33 GMT  
		Size: 2.8 MB (2775220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60f8644f086e6d183d4c2ec8835e42eb82d5f98dd837d727bbeaa76de2d1a3`  
		Last Modified: Tue, 23 Aug 2022 10:44:32 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0967c4f7d945eda8be25366902a136d8a8813486bce0cc4037762d23efbe3442`  
		Last Modified: Tue, 23 Aug 2022 21:05:53 GMT  
		Size: 1.4 MB (1435147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd66868ffb16cd3f9211d5304900f8dcabe3f55da8d322f1d801e5eba0691e1`  
		Last Modified: Tue, 23 Aug 2022 21:05:55 GMT  
		Size: 10.5 MB (10460473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0240bf01c75304f3cb51b17bfc8f37926c97384d908ce268a2d48ef2938f892`  
		Last Modified: Fri, 26 Aug 2022 21:51:27 GMT  
		Size: 65.3 MB (65333373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cf4c8cf40a063c9ce1736e080b0287408cb5d9554a49c75c05431393c38c48`  
		Last Modified: Fri, 26 Aug 2022 21:51:16 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:5.12.0-alpine`

```console
$ docker pull ghost@sha256:4e9dc911a54f89224bf4552e72a155d9c2b9ff29ce5f034e8c5055e24d861f15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `ghost:5.12.0-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:b7cdd7a7ae670cf833f839b3cf3c5e15b5f9c1ae0d1b220d32dd4b701e21d562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115171904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36c4534571a9c97ad0dd3111039423ef7c7486ae058e5e46330ad179ec82023`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 05:42:56 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 08:33:31 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 08:33:31 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 08:33:38 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 08:33:38 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 08:33:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 08:33:38 GMT
CMD ["node"]
# Wed, 17 Aug 2022 08:37:49 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 08:37:51 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 08:37:51 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 08:37:51 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 08:38:52 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 08:38:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 08:38:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:55:05 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 22:05:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 22:05:08 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 22:05:08 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 22:05:09 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 26 Aug 2022 22:05:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 22:05:09 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 22:05:09 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0242dcb01a33bec13ceb8fea51cdfbdac1677423e322b07dc334b0cb67aec642`  
		Last Modified: Wed, 17 Aug 2022 08:36:51 GMT  
		Size: 35.4 MB (35430982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612fd2e24f9da53aeff556efe5d18ef95264e831be9eba4c8bced3c9aabf4b22`  
		Last Modified: Wed, 17 Aug 2022 08:36:44 GMT  
		Size: 2.4 MB (2431032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89adb15822bd2887be78a2b8b70777482a8a6b84490d1210c54d93c6fd7177a5`  
		Last Modified: Wed, 17 Aug 2022 08:36:42 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350c39d4194c2030fff551020327a74cd025a79ce950690a6548f7341b197e5c`  
		Last Modified: Wed, 17 Aug 2022 08:59:08 GMT  
		Size: 11.0 KB (10961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e0405fab6a93ba6b0ce37c0803e29b5500f43fd8aac23f9f998281015d0cd6`  
		Last Modified: Wed, 17 Aug 2022 08:59:09 GMT  
		Size: 772.0 KB (771989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd866b6c9473c76325836db455955454bf064ebde704c9909583fec3e8f7f13`  
		Last Modified: Wed, 17 Aug 2022 08:59:22 GMT  
		Size: 10.5 MB (10459688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c7e973f13d211e59855a80a94364e31c6e6a1a3a2dfec7b989c58c58fafefe`  
		Last Modified: Fri, 26 Aug 2022 22:06:08 GMT  
		Size: 63.5 MB (63452287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b124ba258bf3feadd20db14b3ba2afa43271af465b2bb4c283b80b3551a3b80`  
		Last Modified: Fri, 26 Aug 2022 22:05:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5.12.0-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:101aeb094f23c3ad06cac7bff69199738ec7f2cb406b7b1df1a19440d1a55fd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128143191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7827ca61839c38a612c5adb293035b079b78741745a8b6809cc820cb18e63f42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 00:49:14 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 01:19:27 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 01:19:28 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 01:19:32 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 01:19:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 01:19:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 01:19:35 GMT
CMD ["node"]
# Wed, 17 Aug 2022 02:27:45 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 02:27:47 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 02:27:47 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 02:27:48 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 02:28:07 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 02:28:08 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 02:28:09 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:56:47 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 22:01:30 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 22:01:33 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 22:01:35 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 22:01:37 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 26 Aug 2022 22:01:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 22:01:42 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 22:01:44 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bbdc18f3e0d876c6dd22cb80843cd39643602e791488600c523655514f1f31`  
		Last Modified: Wed, 17 Aug 2022 01:28:14 GMT  
		Size: 36.3 MB (36344502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb54f68a6fc352431a291f292597a7445894ab233ad63742943345a8adfe34b8`  
		Last Modified: Wed, 17 Aug 2022 01:28:09 GMT  
		Size: 2.4 MB (2440157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6c5903b8c0ef8e2e35ecf2ba7b484d0732333f44224b7bbd07cab3fc8980d0`  
		Last Modified: Wed, 17 Aug 2022 01:28:09 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822d0cbaa1675e44af4152ee9e2678b3e94940c75977aedf8a2161c4bdcb0ae8`  
		Last Modified: Wed, 17 Aug 2022 02:34:20 GMT  
		Size: 11.0 KB (10988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f5ed121dd729b06bf5c0fa31d95f6a2269739d68eb5bf2dc884c57c02b9e39`  
		Last Modified: Wed, 17 Aug 2022 02:34:21 GMT  
		Size: 826.1 KB (826078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b760c5860186be667d6be0e7933199cc6bf74bc0c997ddb4d5eac6232b882`  
		Last Modified: Wed, 17 Aug 2022 02:34:24 GMT  
		Size: 10.5 MB (10454441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4140a1d88f4c96f6ce1ab4d5322427a93b95ed9bacce56133c9860a2f658f7`  
		Last Modified: Fri, 26 Aug 2022 22:03:23 GMT  
		Size: 75.4 MB (75358365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094f4a7e5552544716eccb4169a4d80f632487a9f4b5f0aca504be92343d11e6`  
		Last Modified: Fri, 26 Aug 2022 22:03:09 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:alpine`

```console
$ docker pull ghost@sha256:05702fcd8b36c375e67d802dc509b1cd3fca75a5120c351b345438833a4022a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:alpine` - linux; amd64

```console
$ docker pull ghost@sha256:5cbea95e17628ed41c89b036080b704dc5de4ac1931657304da3909f17909c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (121048344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0216d33e59a2c6040a2ce8da935038b3f5a824666393fdb86ada484e83383e38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 16 Aug 2022 23:35:38 GMT
ENV NODE_VERSION=16.17.0
# Tue, 16 Aug 2022 23:35:45 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 16 Aug 2022 23:35:46 GMT
ENV YARN_VERSION=1.22.19
# Tue, 16 Aug 2022 23:35:50 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 16 Aug 2022 23:35:50 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 16 Aug 2022 23:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 Aug 2022 23:35:50 GMT
CMD ["node"]
# Wed, 17 Aug 2022 00:25:36 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 00:25:37 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 00:25:37 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 00:25:38 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 00:25:55 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 00:25:55 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 00:25:56 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 24 Aug 2022 23:26:17 GMT
ENV GHOST_VERSION=5.11.0
# Wed, 24 Aug 2022 23:27:24 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 24 Aug 2022 23:27:26 GMT
WORKDIR /var/lib/ghost
# Wed, 24 Aug 2022 23:27:26 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 24 Aug 2022 23:27:26 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 24 Aug 2022 23:27:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 23:27:27 GMT
EXPOSE 2368
# Wed, 24 Aug 2022 23:27:27 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864b973d1bf1f32e9e7938e6f158ecf7b2503fbbe7799aacbf1fe853f506f398`  
		Last Modified: Tue, 16 Aug 2022 23:41:04 GMT  
		Size: 36.4 MB (36447059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fe61ad56f50607679112c84f9b17b0dc5f9f2c130e875aa8d2d49d43a8fbbd`  
		Last Modified: Tue, 16 Aug 2022 23:40:59 GMT  
		Size: 2.4 MB (2350967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3887ab559e662a183c826648d3d51ba916a9be9119c1349b63ad6ca2c1c6c32`  
		Last Modified: Tue, 16 Aug 2022 23:40:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0934c2dd904c5efc297df956ff406bc4612835aef251c5fdefb18325930d42a6`  
		Last Modified: Wed, 17 Aug 2022 00:28:02 GMT  
		Size: 11.3 KB (11279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2212eaaa6ff840552d707d93915cb7ab73b7ab30b5dd8bee5791ef6e7f77b4e0`  
		Last Modified: Wed, 17 Aug 2022 00:28:02 GMT  
		Size: 820.0 KB (820039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f91237b7e346ccbacb16136605b73c0ef6bb3c24801d331990385ef5614205`  
		Last Modified: Wed, 17 Aug 2022 00:28:05 GMT  
		Size: 10.5 MB (10453252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ed9260d182f293ca9db9b7d44631fcd0b720db204f1b338f83ed8bc5330f66`  
		Last Modified: Wed, 24 Aug 2022 23:28:39 GMT  
		Size: 68.2 MB (68158694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af63d868d813e102a89546302d93bfef19deb775d4c3a36fa9ae19dad1a46f5`  
		Last Modified: Wed, 24 Aug 2022 23:28:26 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:b7cdd7a7ae670cf833f839b3cf3c5e15b5f9c1ae0d1b220d32dd4b701e21d562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115171904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36c4534571a9c97ad0dd3111039423ef7c7486ae058e5e46330ad179ec82023`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 05:42:56 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 08:33:31 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 08:33:31 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 08:33:38 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 08:33:38 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 08:33:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 08:33:38 GMT
CMD ["node"]
# Wed, 17 Aug 2022 08:37:49 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 08:37:51 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 08:37:51 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 08:37:51 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 08:38:52 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 08:38:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 08:38:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:55:05 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 22:05:07 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 22:05:08 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 22:05:08 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 22:05:09 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 26 Aug 2022 22:05:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 22:05:09 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 22:05:09 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0242dcb01a33bec13ceb8fea51cdfbdac1677423e322b07dc334b0cb67aec642`  
		Last Modified: Wed, 17 Aug 2022 08:36:51 GMT  
		Size: 35.4 MB (35430982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612fd2e24f9da53aeff556efe5d18ef95264e831be9eba4c8bced3c9aabf4b22`  
		Last Modified: Wed, 17 Aug 2022 08:36:44 GMT  
		Size: 2.4 MB (2431032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89adb15822bd2887be78a2b8b70777482a8a6b84490d1210c54d93c6fd7177a5`  
		Last Modified: Wed, 17 Aug 2022 08:36:42 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350c39d4194c2030fff551020327a74cd025a79ce950690a6548f7341b197e5c`  
		Last Modified: Wed, 17 Aug 2022 08:59:08 GMT  
		Size: 11.0 KB (10961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e0405fab6a93ba6b0ce37c0803e29b5500f43fd8aac23f9f998281015d0cd6`  
		Last Modified: Wed, 17 Aug 2022 08:59:09 GMT  
		Size: 772.0 KB (771989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd866b6c9473c76325836db455955454bf064ebde704c9909583fec3e8f7f13`  
		Last Modified: Wed, 17 Aug 2022 08:59:22 GMT  
		Size: 10.5 MB (10459688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c7e973f13d211e59855a80a94364e31c6e6a1a3a2dfec7b989c58c58fafefe`  
		Last Modified: Fri, 26 Aug 2022 22:06:08 GMT  
		Size: 63.5 MB (63452287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b124ba258bf3feadd20db14b3ba2afa43271af465b2bb4c283b80b3551a3b80`  
		Last Modified: Fri, 26 Aug 2022 22:05:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:e81be4dbd26ed1bfecb149da0248ca35082bd837550c566e79e401d7afc4ff7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.2 MB (114154756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3aa4cadae8a2cece6c5078f11127c57f3999e33595e7a7c54fcd0d85f9d92b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 08:51:37 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 11:44:06 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 11:44:06 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 11:44:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 11:44:12 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 11:44:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 11:44:12 GMT
CMD ["node"]
# Wed, 17 Aug 2022 12:07:15 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 12:07:16 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 12:07:16 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 12:07:16 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 12:07:40 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 12:07:41 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 12:07:41 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 25 Aug 2022 11:14:07 GMT
ENV GHOST_VERSION=5.11.0
# Thu, 25 Aug 2022 11:23:38 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 25 Aug 2022 11:23:39 GMT
WORKDIR /var/lib/ghost
# Thu, 25 Aug 2022 11:23:40 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 25 Aug 2022 11:23:40 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 25 Aug 2022 11:23:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Aug 2022 11:23:40 GMT
EXPOSE 2368
# Thu, 25 Aug 2022 11:23:40 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af62c2a8a93c8d8d84c4b7f3ea2d40da7355f049477c23dad411d59b2687619`  
		Last Modified: Wed, 17 Aug 2022 11:54:27 GMT  
		Size: 35.0 MB (34960433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecbe39d3f57b92a197c93a31ce4457cc2042c1e806fe36620e43e5170583fd4`  
		Last Modified: Wed, 17 Aug 2022 11:54:19 GMT  
		Size: 2.4 MB (2430938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b335659237c4596ce2b2c2a58cd9122a83e828f0433d10ed23121fe84900076`  
		Last Modified: Wed, 17 Aug 2022 11:54:18 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac45770c5da644dce686ca3b1f3f229f2606c92601a302ad6bfba78e7eb80136`  
		Last Modified: Wed, 17 Aug 2022 12:20:08 GMT  
		Size: 10.7 KB (10734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986eb734888fa41d4980b8f4ed215b85de0db92a44dec53d2de8542e51d8936f`  
		Last Modified: Wed, 17 Aug 2022 12:20:09 GMT  
		Size: 704.7 KB (704656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9dbc2371a118885185eed934e1de1597c58263dee5ff2ffbb2704f69899eef`  
		Last Modified: Wed, 17 Aug 2022 12:20:18 GMT  
		Size: 10.5 MB (10457009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cd01b20c32d3a9cf594fabc2fb4e8be18d02616504092fed3b8f0d92877eac`  
		Last Modified: Thu, 25 Aug 2022 11:34:03 GMT  
		Size: 63.2 MB (63172927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d75ea7e56b3dc33396e3df3fd241d73dd69d989c4d2009101a016142833276`  
		Last Modified: Thu, 25 Aug 2022 11:33:29 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:101aeb094f23c3ad06cac7bff69199738ec7f2cb406b7b1df1a19440d1a55fd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128143191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7827ca61839c38a612c5adb293035b079b78741745a8b6809cc820cb18e63f42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 17 Aug 2022 00:49:14 GMT
ENV NODE_VERSION=16.17.0
# Wed, 17 Aug 2022 01:19:27 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6c94de8608fcd5b992f5f804c2d03bc3a7f422426760b1b80ea4ced486a694fe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 17 Aug 2022 01:19:28 GMT
ENV YARN_VERSION=1.22.19
# Wed, 17 Aug 2022 01:19:32 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 17 Aug 2022 01:19:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Aug 2022 01:19:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Aug 2022 01:19:35 GMT
CMD ["node"]
# Wed, 17 Aug 2022 02:27:45 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 17 Aug 2022 02:27:47 GMT
RUN apk add --no-cache 		bash
# Wed, 17 Aug 2022 02:27:47 GMT
ENV NODE_ENV=production
# Wed, 17 Aug 2022 02:27:48 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Wed, 17 Aug 2022 02:28:07 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 17 Aug 2022 02:28:08 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 17 Aug 2022 02:28:09 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:56:47 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 22:01:30 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 22:01:33 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 22:01:35 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 22:01:37 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 26 Aug 2022 22:01:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 22:01:42 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 22:01:44 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bbdc18f3e0d876c6dd22cb80843cd39643602e791488600c523655514f1f31`  
		Last Modified: Wed, 17 Aug 2022 01:28:14 GMT  
		Size: 36.3 MB (36344502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb54f68a6fc352431a291f292597a7445894ab233ad63742943345a8adfe34b8`  
		Last Modified: Wed, 17 Aug 2022 01:28:09 GMT  
		Size: 2.4 MB (2440157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6c5903b8c0ef8e2e35ecf2ba7b484d0732333f44224b7bbd07cab3fc8980d0`  
		Last Modified: Wed, 17 Aug 2022 01:28:09 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822d0cbaa1675e44af4152ee9e2678b3e94940c75977aedf8a2161c4bdcb0ae8`  
		Last Modified: Wed, 17 Aug 2022 02:34:20 GMT  
		Size: 11.0 KB (10988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f5ed121dd729b06bf5c0fa31d95f6a2269739d68eb5bf2dc884c57c02b9e39`  
		Last Modified: Wed, 17 Aug 2022 02:34:21 GMT  
		Size: 826.1 KB (826078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b760c5860186be667d6be0e7933199cc6bf74bc0c997ddb4d5eac6232b882`  
		Last Modified: Wed, 17 Aug 2022 02:34:24 GMT  
		Size: 10.5 MB (10454441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e4140a1d88f4c96f6ce1ab4d5322427a93b95ed9bacce56133c9860a2f658f7`  
		Last Modified: Fri, 26 Aug 2022 22:03:23 GMT  
		Size: 75.4 MB (75358365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094f4a7e5552544716eccb4169a4d80f632487a9f4b5f0aca504be92343d11e6`  
		Last Modified: Fri, 26 Aug 2022 22:03:09 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ghost:latest`

```console
$ docker pull ghost@sha256:073d56e59a5ca2b9cc97ba14ecee8cb27820e0dd99d1064794ef1a5ff67b1600
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
$ docker pull ghost@sha256:bde8307b90069d5c19f25705d3f9dd2f2f9cb296838649b8820c4a7461c2c950
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148881875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed89eced794e9bf97e4af237e2eb9712deae6419d023306f68e42d87c6bc319a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:03:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:05:45 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 04:06:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:06:12 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:06:24 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:06:24 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:06:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:06:24 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:51:34 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:51:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:51:46 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:51:46 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:52:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:52:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:52:05 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 24 Aug 2022 23:25:08 GMT
ENV GHOST_VERSION=5.11.0
# Wed, 24 Aug 2022 23:26:08 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 24 Aug 2022 23:26:10 GMT
WORKDIR /var/lib/ghost
# Wed, 24 Aug 2022 23:26:10 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 24 Aug 2022 23:26:10 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 24 Aug 2022 23:26:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 23:26:10 GMT
EXPOSE 2368
# Wed, 24 Aug 2022 23:26:10 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065fda631bffac8aa07440d44064117eee8bbfb50d65e04dbd5b29021c0140bf`  
		Last Modified: Tue, 23 Aug 2022 04:12:47 GMT  
		Size: 4.2 KB (4180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8870f8b81b668639dc33301e8197b549f9d7a8fb85598376cc3cccdc8e0282ec`  
		Last Modified: Tue, 23 Aug 2022 04:14:46 GMT  
		Size: 35.3 MB (35348605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1aeb08c8d655334863d3f8cbada8f83783bcbf4daa4c04868a404169c9e97a`  
		Last Modified: Tue, 23 Aug 2022 04:14:41 GMT  
		Size: 2.8 MB (2773386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41346f34487d2de1801efdbb3cc550aa6ba3ac1b5778c7fdb8ed411b7ac1db5`  
		Last Modified: Tue, 23 Aug 2022 04:14:41 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f035609a702017b50a93d64dc01042501c221794129de701d96eb06cd71260`  
		Last Modified: Tue, 23 Aug 2022 20:55:26 GMT  
		Size: 1.4 MB (1448263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c6c0e9e735e43683b9e73b95657123dcb17dcf74ddc911097e695705fcfe09`  
		Last Modified: Tue, 23 Aug 2022 20:55:29 GMT  
		Size: 10.5 MB (10453707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada2c2e4ff48ce35a513530614ff27307d87bace55295c283c2c87fe4302ae5d`  
		Last Modified: Wed, 24 Aug 2022 23:28:11 GMT  
		Size: 67.5 MB (67471253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecfc8400a05eea0ac1181de2080e243f3879d8a309fa4624bedcdf8cebb9006`  
		Last Modified: Wed, 24 Aug 2022 23:28:00 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; arm variant v7

```console
$ docker pull ghost@sha256:4a54abec917354a2433b00b8fcd001f45bf05d4bf6c449937f1dd99a414deecd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153136501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:448273a23b2dd5ed0daf6fa2fb3a17a801b3d2f1c1c4c425ef6373eddc3bbd32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 21:44:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 21:47:37 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 21:48:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 21:48:11 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 21:48:26 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 21:48:26 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 21:48:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:48:26 GMT
CMD ["node"]
# Thu, 25 Aug 2022 11:06:28 GMT
ENV GOSU_VERSION=1.12
# Thu, 25 Aug 2022 11:06:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 25 Aug 2022 11:06:44 GMT
ENV NODE_ENV=production
# Thu, 25 Aug 2022 11:06:44 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Thu, 25 Aug 2022 11:07:11 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Thu, 25 Aug 2022 11:07:11 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Thu, 25 Aug 2022 11:07:11 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 25 Aug 2022 11:07:11 GMT
ENV GHOST_VERSION=5.11.0
# Thu, 25 Aug 2022 11:13:52 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 25 Aug 2022 11:13:53 GMT
WORKDIR /var/lib/ghost
# Thu, 25 Aug 2022 11:13:53 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 25 Aug 2022 11:13:53 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Thu, 25 Aug 2022 11:13:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Aug 2022 11:13:54 GMT
EXPOSE 2368
# Thu, 25 Aug 2022 11:13:54 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5221a7a14db5d9fbd6928fcb2921040bb5d801661c018df5b4922f1c0cd73b25`  
		Last Modified: Tue, 23 Aug 2022 22:00:09 GMT  
		Size: 4.2 KB (4168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620dcb50c9c7f1bbeb5e2b5a12e7fa08bf27a468bfc8ed3fbf439d1bc082c1b8`  
		Last Modified: Tue, 23 Aug 2022 22:03:06 GMT  
		Size: 32.6 MB (32573345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca57e71c998e1a076aed800c650e8758b6b6917356581b7b29d4aef537581df`  
		Last Modified: Tue, 23 Aug 2022 22:02:59 GMT  
		Size: 2.8 MB (2767232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59650dc6a524a79de3b9d5c0d5589cdb9003948e9d9e55cec41b494e6c060ed`  
		Last Modified: Tue, 23 Aug 2022 22:02:58 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865fed7c0dce56885134704e18d70ae963d20bf39dc80adb1fc43df2259f2f66`  
		Last Modified: Thu, 25 Aug 2022 11:32:29 GMT  
		Size: 1.4 MB (1400198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d24704e6b17ee2bb7332099b285f0d2f47157d7aa6ece29c99174dcd59ba765`  
		Last Modified: Thu, 25 Aug 2022 11:32:43 GMT  
		Size: 10.5 MB (10458318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0157d1c1f9ddbddbe2547095e20a9fc215bde7581c6092e70f81f5096e48aa79`  
		Last Modified: Thu, 25 Aug 2022 11:33:10 GMT  
		Size: 79.4 MB (79360512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6255ec21dad79c58ec4d433176949dcecff5be2631f540b954d461b9ed2a5eb5`  
		Last Modified: Thu, 25 Aug 2022 11:32:28 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:6ef301ab3555fb1636b918d719174614be61b661da5fda1b6bcf8d8dcbbee4d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156157808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b43780b59a0b8d89594337ce2aae1e92435588df8050c36281a62464b69b5975`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 04:51:52 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 04:55:16 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 04:55:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 04:55:43 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 04:55:55 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 04:55:57 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 04:55:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 04:55:58 GMT
CMD ["node"]
# Tue, 23 Aug 2022 22:17:12 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 22:17:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 22:17:24 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 22:17:25 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 22:17:44 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 22:17:45 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 22:17:46 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:52:35 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 21:56:20 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 21:56:24 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 21:56:26 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 21:56:29 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 26 Aug 2022 21:56:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 21:56:34 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 21:56:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f232a362cd9820adfd1443fbb1fe468c3175d65fa45259cc218f0b706a0ab11`  
		Last Modified: Tue, 23 Aug 2022 05:08:27 GMT  
		Size: 4.0 KB (4044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa653d801310584a170e38c681b10894b2a77ef836273f9d199c0c6a47904094`  
		Last Modified: Tue, 23 Aug 2022 05:10:51 GMT  
		Size: 35.5 MB (35495106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25750f98abe8642e2ad2e8b0311e2f33bf18a485553993e1d2a92b7f16e71a74`  
		Last Modified: Tue, 23 Aug 2022 05:10:46 GMT  
		Size: 2.8 MB (2772303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476cb0003ed3a2e40214ba9063e0bb0f5542ef59f6c33588c076664260ba176d`  
		Last Modified: Tue, 23 Aug 2022 05:10:45 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24b540e3d30c4849b45592e96ea7f677993457b4c161935ec2d8b536aa49a72`  
		Last Modified: Tue, 23 Aug 2022 22:24:44 GMT  
		Size: 1.4 MB (1383735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba84c7d5d4ca00a02d329912660d788c3509eb8325a6064d97b0058b45a5474`  
		Last Modified: Tue, 23 Aug 2022 22:24:47 GMT  
		Size: 10.5 MB (10454579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af36c284258f664c6fe8c7eb63689c98d1595fcc65079657bf8eb84891c11db`  
		Last Modified: Fri, 26 Aug 2022 22:02:51 GMT  
		Size: 76.0 MB (75983259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a71325e5f20be54324fbc5ff1dc747e0b03cc691d7472e3b19fc277d9cd6714`  
		Last Modified: Fri, 26 Aug 2022 22:02:36 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; ppc64le

```console
$ docker pull ghost@sha256:4c08885ac69ee4aedf606dceb6b9be3c977cdc5ac80a9ff37e31219c08e686d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152708772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ebce572687b5e88fa7ccca994f0934d575d4569b0d9ff808b6753598e5d9614`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:59:59 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 03:02:23 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 03:03:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 03:03:06 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 03:03:31 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 03:03:32 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 03:03:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 03:03:32 GMT
CMD ["node"]
# Tue, 23 Aug 2022 16:17:13 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 16:17:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 16:17:39 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 16:17:39 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 16:18:10 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 16:18:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 16:18:13 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 24 Aug 2022 22:32:20 GMT
ENV GHOST_VERSION=5.11.0
# Wed, 24 Aug 2022 22:41:03 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 24 Aug 2022 22:41:11 GMT
WORKDIR /var/lib/ghost
# Wed, 24 Aug 2022 22:41:11 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 24 Aug 2022 22:41:12 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Wed, 24 Aug 2022 22:41:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 22:41:13 GMT
EXPOSE 2368
# Wed, 24 Aug 2022 22:41:13 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f072867559a95ee18a2f9cafdd6d774dfd46aced3278c83d3652f9b47874402`  
		Last Modified: Tue, 23 Aug 2022 03:11:50 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d672ed322507d9fe8d9cc50c2c0322dec911843f285809f396eb5a24276fb39`  
		Last Modified: Tue, 23 Aug 2022 03:13:44 GMT  
		Size: 37.4 MB (37413541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc6f3d892c304e25ca4018d68093a08ef0abf6a685d03b687052a6aedd78ff5`  
		Last Modified: Tue, 23 Aug 2022 03:13:35 GMT  
		Size: 2.8 MB (2773489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d242eaa1a1d467ce825da0390583291c07bafbdbbd6068577e58f6ef6a946ecb`  
		Last Modified: Tue, 23 Aug 2022 03:13:34 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c0c8ea85d5ad4979cd20a465ac7f6b1a2521dc080589bda90263b276ba273`  
		Last Modified: Tue, 23 Aug 2022 16:36:28 GMT  
		Size: 1.4 MB (1367219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e03d4bcc0b171c0ee68bbb4704f0cea8c2ab9bcc309eef80488699529c12336`  
		Last Modified: Tue, 23 Aug 2022 16:36:33 GMT  
		Size: 10.5 MB (10459153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee6f3f210367839f64ed97b02829a92708d8c76b3961744ffc05e115470da36`  
		Last Modified: Wed, 24 Aug 2022 22:42:17 GMT  
		Size: 65.4 MB (65405908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35d75685c112e934f6d660e7b6467cb9859a59876d5cc7d4e78e40507e7eb66`  
		Last Modified: Wed, 24 Aug 2022 22:41:54 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:latest` - linux; s390x

```console
$ docker pull ghost@sha256:e3a777ad6e2680d2fdd419c185def4d44e81821f6a9500da89fa36ee9b783058
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144902229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7213ae4b9752d1be299eb0fd729e03ed2719f8c381fd5c19b0661eec496cec53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 10:34:41 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 23 Aug 2022 10:36:25 GMT
ENV NODE_VERSION=16.17.0
# Tue, 23 Aug 2022 10:36:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch##*-}" in       amd64) ARCH='x64';;       ppc64el) ARCH='ppc64le';;       s390x) ARCH='s390x';;       arm64) ARCH='arm64';;       armhf) ARCH='armv7l';;       i386) ARCH='x86';;       *) echo "unsupported architecture"; exit 1 ;;     esac     && set -ex     && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr xz-utils libatomic1 --no-install-recommends     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false     && ln -s /usr/local/bin/node /usr/local/bin/nodejs     && node --version     && npm --version
# Tue, 23 Aug 2022 10:36:46 GMT
ENV YARN_VERSION=1.22.19
# Tue, 23 Aug 2022 10:36:54 GMT
RUN set -ex   && savedAptMark="$(apt-mark showmanual)"   && apt-get update && apt-get install -y ca-certificates curl wget gnupg dirmngr --no-install-recommends   && rm -rf /var/lib/apt/lists/*   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apt-mark auto '.*' > /dev/null   && { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; }   && find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && yarn --version
# Tue, 23 Aug 2022 10:36:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 23 Aug 2022 10:36:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 10:36:55 GMT
CMD ["node"]
# Tue, 23 Aug 2022 20:43:29 GMT
ENV GOSU_VERSION=1.12
# Tue, 23 Aug 2022 20:43:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 Aug 2022 20:43:57 GMT
ENV NODE_ENV=production
# Tue, 23 Aug 2022 20:43:57 GMT
ENV GHOST_CLI_VERSION=1.22.0
# Tue, 23 Aug 2022 20:44:40 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 23 Aug 2022 20:44:48 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 23 Aug 2022 20:44:48 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 26 Aug 2022 21:46:48 GMT
ENV GHOST_VERSION=5.12.0
# Fri, 26 Aug 2022 21:50:32 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		savedAptMark="$(apt-mark showmanual)"; 	aptPurge=; 		installCmd='gosu node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		aptPurge=1; 		apt-get update; 		apt-get install -y --no-install-recommends g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	gosu node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	gosu node ghost config paths.contentPath "$GHOST_CONTENT"; 		gosu node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='gosu node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			aptPurge=1; 			apt-get update; 			apt-get install -y --no-install-recommends g++ make python3; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.10 in Debian bullseye is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$aptPurge" ]; then 		apt-mark showmanual | xargs apt-mark auto > /dev/null; 		[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 		apt-get purge -y --auto-remove; 		rm -rf /var/lib/apt/lists/*; 	fi; 		gosu node yarn cache clean; 	gosu node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 26 Aug 2022 21:50:40 GMT
WORKDIR /var/lib/ghost
# Fri, 26 Aug 2022 21:50:40 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 26 Aug 2022 21:50:40 GMT
COPY file:303989b132b5193e832753e2c7236a4050fdc0fe60a54dc1f0c4a44422a2d1ca in /usr/local/bin 
# Fri, 26 Aug 2022 21:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Aug 2022 21:50:40 GMT
EXPOSE 2368
# Fri, 26 Aug 2022 21:50:40 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c379dfa30c39780b6036486f76caf47f9c913cafd9fc09843e09a18b85d8a95f`  
		Last Modified: Tue, 23 Aug 2022 10:43:30 GMT  
		Size: 4.2 KB (4186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5f681357b689bb7539d1e20b4cadedd292b61a3c69b5708498366d6fd7d79c`  
		Last Modified: Tue, 23 Aug 2022 10:44:37 GMT  
		Size: 35.2 MB (35242738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924401253b9a620a330a5140a4a4f698349610df8872c46039c6aeb87a94a351`  
		Last Modified: Tue, 23 Aug 2022 10:44:33 GMT  
		Size: 2.8 MB (2775220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60f8644f086e6d183d4c2ec8835e42eb82d5f98dd837d727bbeaa76de2d1a3`  
		Last Modified: Tue, 23 Aug 2022 10:44:32 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0967c4f7d945eda8be25366902a136d8a8813486bce0cc4037762d23efbe3442`  
		Last Modified: Tue, 23 Aug 2022 21:05:53 GMT  
		Size: 1.4 MB (1435147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd66868ffb16cd3f9211d5304900f8dcabe3f55da8d322f1d801e5eba0691e1`  
		Last Modified: Tue, 23 Aug 2022 21:05:55 GMT  
		Size: 10.5 MB (10460473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0240bf01c75304f3cb51b17bfc8f37926c97384d908ce268a2d48ef2938f892`  
		Last Modified: Fri, 26 Aug 2022 21:51:27 GMT  
		Size: 65.3 MB (65333373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cf4c8cf40a063c9ce1736e080b0287408cb5d9554a49c75c05431393c38c48`  
		Last Modified: Fri, 26 Aug 2022 21:51:16 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
