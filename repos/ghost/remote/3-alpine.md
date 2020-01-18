## `ghost:3-alpine`

```console
$ docker pull ghost@sha256:7e329a0cdec5e926f2d49bf8054280416911f21d471f50ca017ef79b1672ff84
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
$ docker pull ghost@sha256:6e8c037e40260b8de3e5dfaa55f2ff973795df9c376a92bb81205f7dd6cb3040
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115870745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f49a701ea32b3e2de67ec8d21f4945515b1486f029a7d8b0748b6e09b0d5579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 24 Dec 2019 19:20:12 GMT
ADD file:36fdc8cb08228a87093fb227736f4ce1d4d6c15366326dea541fbbd863976ee5 in / 
# Tue, 24 Dec 2019 19:20:12 GMT
CMD ["/bin/sh"]
# Wed, 08 Jan 2020 22:24:28 GMT
ENV NODE_VERSION=12.14.1
# Wed, 08 Jan 2020 22:24:33 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6906577d7b15cc940f47fc88436ac45f73e5abecd15f09d8f2a9ea337fc2fe5e"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 08 Jan 2020 22:24:33 GMT
ENV YARN_VERSION=1.21.1
# Wed, 08 Jan 2020 22:24:36 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 08 Jan 2020 22:24:36 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 08 Jan 2020 22:24:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jan 2020 22:24:36 GMT
CMD ["node"]
# Fri, 17 Jan 2020 23:21:33 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 17 Jan 2020 23:21:34 GMT
RUN apk add --no-cache 		bash
# Fri, 17 Jan 2020 23:21:34 GMT
ENV NODE_ENV=production
# Fri, 17 Jan 2020 23:21:35 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Fri, 17 Jan 2020 23:21:50 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 17 Jan 2020 23:21:50 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 17 Jan 2020 23:21:50 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 17 Jan 2020 23:21:50 GMT
ENV GHOST_VERSION=3.3.0
# Fri, 17 Jan 2020 23:22:42 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 17 Jan 2020 23:22:43 GMT
WORKDIR /var/lib/ghost
# Fri, 17 Jan 2020 23:22:43 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 17 Jan 2020 23:22:44 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 17 Jan 2020 23:22:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Jan 2020 23:22:44 GMT
EXPOSE 2368
# Fri, 17 Jan 2020 23:22:44 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:e6b0cf9c0882fb079c9d35361d12ff4691f916b6d825061247d1bd0b26d7cf3f`  
		Last Modified: Tue, 24 Dec 2019 19:20:40 GMT  
		Size: 2.8 MB (2801778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c42fbec1fbad37f47954fc628a1fdc34831e7f0c56dde8f310c05ba47c4fb4`  
		Last Modified: Wed, 08 Jan 2020 22:34:50 GMT  
		Size: 24.3 MB (24270485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f549f993396784dff3779ba5d24adbbdf9a3b3c3c2e00412b713fc4b6bf4bed`  
		Last Modified: Wed, 08 Jan 2020 22:34:46 GMT  
		Size: 1.3 MB (1264625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882dbe8a558734699d46465fc8ab0ce489a0dffaac61132130cd372caeca4bf5`  
		Last Modified: Wed, 08 Jan 2020 22:34:45 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3126eb850f8c0ad9ffb8cfb57daffa7770bc89131eda4f6d59e5b9fe388fdd`  
		Last Modified: Fri, 17 Jan 2020 23:27:24 GMT  
		Size: 9.9 KB (9905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1721b77a4ad65c664b669e4d830f675ca92c5e29d5fa17222365603b5ba46c50`  
		Last Modified: Fri, 17 Jan 2020 23:27:25 GMT  
		Size: 1.2 MB (1211028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4b7a275decabdb38f3cd2e3d8f3fd016cbda3e44a37f3dc3675b008824cf33`  
		Last Modified: Fri, 17 Jan 2020 23:27:27 GMT  
		Size: 6.8 MB (6791368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06023564ce428ab4063cc3e2f84ffd13b2998eb6b0729f201507f43a823a6268`  
		Last Modified: Fri, 17 Jan 2020 23:27:50 GMT  
		Size: 79.5 MB (79520722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe58b1fc028b89b6f7af06c1b6239c3a00180fa40b313cbd3ca5679e6c66b8de`  
		Last Modified: Fri, 17 Jan 2020 23:27:24 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:43e323f5abe0330ddd1e990f8ea7f5ebff3cb9c30c2cdb9f3032fe1eeb880e33
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107286341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806d29f60195224aba2c86bf2ce516666326dfc986ee996d9fc2f4842abeeeb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Wed, 08 Jan 2020 23:17:56 GMT
ENV NODE_VERSION=12.14.1
# Wed, 08 Jan 2020 23:28:00 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6906577d7b15cc940f47fc88436ac45f73e5abecd15f09d8f2a9ea337fc2fe5e"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 08 Jan 2020 23:28:02 GMT
ENV YARN_VERSION=1.21.1
# Wed, 08 Jan 2020 23:28:10 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 08 Jan 2020 23:28:11 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 08 Jan 2020 23:28:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jan 2020 23:28:13 GMT
CMD ["node"]
# Fri, 17 Jan 2020 23:49:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 17 Jan 2020 23:49:42 GMT
RUN apk add --no-cache 		bash
# Fri, 17 Jan 2020 23:49:43 GMT
ENV NODE_ENV=production
# Fri, 17 Jan 2020 23:49:44 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Fri, 17 Jan 2020 23:50:35 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 17 Jan 2020 23:50:47 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 17 Jan 2020 23:50:50 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 17 Jan 2020 23:50:56 GMT
ENV GHOST_VERSION=3.3.0
# Fri, 17 Jan 2020 23:57:28 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 17 Jan 2020 23:57:33 GMT
WORKDIR /var/lib/ghost
# Fri, 17 Jan 2020 23:57:34 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 17 Jan 2020 23:57:34 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 17 Jan 2020 23:57:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Jan 2020 23:57:35 GMT
EXPOSE 2368
# Fri, 17 Jan 2020 23:57:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b37da9996cf84c0b930ca24b9703edb23ef4ab2523d6bf0e3a016726863a0650`  
		Last Modified: Wed, 08 Jan 2020 23:29:49 GMT  
		Size: 23.7 MB (23721045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c444ae2117f3eec85b91b75e17fdec95d712f34baf12455e337db27e2210dc2e`  
		Last Modified: Wed, 08 Jan 2020 23:29:40 GMT  
		Size: 1.3 MB (1327781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25330ae59fbf5bbc63924cf7cbdb88a5b622ece9c34c7ca1a9768f6fc3d1a4a6`  
		Last Modified: Wed, 08 Jan 2020 23:29:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2377831e7f76ae94722d0b8c947f1a62456c98089259cd737ab53c83c8a667`  
		Last Modified: Sat, 18 Jan 2020 00:10:47 GMT  
		Size: 9.7 KB (9731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6eb1625b822ee4f41d539c0c74357534f5c434d9cb44b81e23729eaef1b610`  
		Last Modified: Sat, 18 Jan 2020 00:10:48 GMT  
		Size: 1.2 MB (1162966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7444b68a1f22dc82be909fc815e303029561dc502ebfbb353ceea38fe2f73f`  
		Last Modified: Sat, 18 Jan 2020 00:10:52 GMT  
		Size: 6.8 MB (6791594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085f15c034d24c377d661ab6fed5b3f434a2d14cc7a794cbb99ffe627e7ca17b`  
		Last Modified: Sat, 18 Jan 2020 00:11:15 GMT  
		Size: 71.7 MB (71660374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b8016d4f2e0462c07bf1106aa2a6643ab660a76acb641f3d5a4f24200072dc`  
		Last Modified: Sat, 18 Jan 2020 00:10:48 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:e3689600b0ea05476613f7cccb9e1a5e855b105d08da24eb9f4c6ac075cfe585
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105666154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5090e6937a30cc565078d8c7f0b908dbee04c077196128d8a57a2e347745e9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 24 Dec 2019 18:59:09 GMT
ADD file:caf7ca25875eddd2bfa2d1e56663bb52d278a85f6ee1314f9ccf01dc4da8070a in / 
# Tue, 24 Dec 2019 18:59:10 GMT
CMD ["/bin/sh"]
# Wed, 08 Jan 2020 23:45:26 GMT
ENV NODE_VERSION=12.14.1
# Wed, 08 Jan 2020 23:52:35 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6906577d7b15cc940f47fc88436ac45f73e5abecd15f09d8f2a9ea337fc2fe5e"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 08 Jan 2020 23:52:39 GMT
ENV YARN_VERSION=1.21.1
# Wed, 08 Jan 2020 23:52:48 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 08 Jan 2020 23:52:50 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 08 Jan 2020 23:52:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jan 2020 23:52:52 GMT
CMD ["node"]
# Sat, 18 Jan 2020 00:07:18 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 18 Jan 2020 00:07:21 GMT
RUN apk add --no-cache 		bash
# Sat, 18 Jan 2020 00:07:22 GMT
ENV NODE_ENV=production
# Sat, 18 Jan 2020 00:07:23 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Sat, 18 Jan 2020 00:07:53 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 18 Jan 2020 00:07:58 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 18 Jan 2020 00:07:59 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 18 Jan 2020 00:07:59 GMT
ENV GHOST_VERSION=3.3.0
# Sat, 18 Jan 2020 00:12:36 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 18 Jan 2020 00:12:41 GMT
WORKDIR /var/lib/ghost
# Sat, 18 Jan 2020 00:12:42 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 18 Jan 2020 00:12:43 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 18 Jan 2020 00:12:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 00:12:51 GMT
EXPOSE 2368
# Sat, 18 Jan 2020 00:12:55 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3922e475e500b2739b5e74787fc80622853325822f71f8bd3de7e5b09654d60f`  
		Last Modified: Tue, 24 Dec 2019 18:59:33 GMT  
		Size: 2.4 MB (2416691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939825db7aab98c2c55dfaf3ba06a5d2643b1757962077511e487afb42091857`  
		Last Modified: Thu, 09 Jan 2020 00:07:54 GMT  
		Size: 23.3 MB (23293000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8cc5cf222854ae3b8a06a343a8e8040fb3445d1401d711a4f22119704615d8`  
		Last Modified: Thu, 09 Jan 2020 00:07:47 GMT  
		Size: 1.3 MB (1327771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75da0a40e8cf9bbd6d4ea778962bcfd0f114d5865287de14e91a3ddab7b1e38`  
		Last Modified: Thu, 09 Jan 2020 00:07:47 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584f306f1d2adc7b602b5ad4a4de2ddbfeae7b24d5177768cf604f94da5bfaff`  
		Last Modified: Sat, 18 Jan 2020 00:31:47 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f501d11a051583b1dc57f23fe425d2c05b648e9b77af1c695c6d57e13f1efb7d`  
		Last Modified: Sat, 18 Jan 2020 00:31:48 GMT  
		Size: 1.1 MB (1101480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3ddd50cd15145452d288720322c2d9d7bb667d4bd6f8b931980678ea550ef1`  
		Last Modified: Sat, 18 Jan 2020 00:31:52 GMT  
		Size: 6.8 MB (6791443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c820efbc094f2339250bc591d26ac09a54ced1d730f06fbb4bd0bbf96eb47`  
		Last Modified: Sat, 18 Jan 2020 00:32:14 GMT  
		Size: 70.7 MB (70725418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85da355e5ac50b657850eb588e420515b82d93af3d6ccb63a2153ac936c0fe7d`  
		Last Modified: Sat, 18 Jan 2020 00:31:46 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:45f4abbc4306747c6fdbc1219d8171ca5157e537408a06131e14574005ba1298
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108462518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:159d0e8cfd32f6591688e10dccd4d1b5c5c7748898c8275cfb1282a65d235336`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 24 Dec 2019 20:26:15 GMT
ADD file:d6c3db0313ab0c6201770c7248d1bac964011a1c08f1a9b434442b7c21efef87 in / 
# Tue, 24 Dec 2019 20:26:24 GMT
CMD ["/bin/sh"]
# Wed, 08 Jan 2020 23:57:09 GMT
ENV NODE_VERSION=12.14.1
# Thu, 09 Jan 2020 00:05:17 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6906577d7b15cc940f47fc88436ac45f73e5abecd15f09d8f2a9ea337fc2fe5e"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Thu, 09 Jan 2020 00:05:17 GMT
ENV YARN_VERSION=1.21.1
# Thu, 09 Jan 2020 00:05:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Thu, 09 Jan 2020 00:05:23 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 09 Jan 2020 00:05:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Jan 2020 00:05:24 GMT
CMD ["node"]
# Fri, 17 Jan 2020 23:45:30 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 17 Jan 2020 23:45:34 GMT
RUN apk add --no-cache 		bash
# Fri, 17 Jan 2020 23:45:35 GMT
ENV NODE_ENV=production
# Fri, 17 Jan 2020 23:45:35 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Fri, 17 Jan 2020 23:46:16 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 17 Jan 2020 23:46:18 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 17 Jan 2020 23:46:18 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 17 Jan 2020 23:46:19 GMT
ENV GHOST_VERSION=3.3.0
# Fri, 17 Jan 2020 23:51:03 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 17 Jan 2020 23:51:09 GMT
WORKDIR /var/lib/ghost
# Fri, 17 Jan 2020 23:51:12 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 17 Jan 2020 23:51:13 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 17 Jan 2020 23:51:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Jan 2020 23:51:19 GMT
EXPOSE 2368
# Fri, 17 Jan 2020 23:51:23 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cde5963f3b93eec667cad527c99d80402a5a91a7a1381f7ffe562f215aec0c50`  
		Last Modified: Tue, 24 Dec 2019 20:26:52 GMT  
		Size: 2.7 MB (2719182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94304e940ba97276174f68320e4a5554a8000b4d2715ff3cbeb2371ba14b4d69`  
		Last Modified: Thu, 09 Jan 2020 00:15:38 GMT  
		Size: 24.4 MB (24430956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edd28c9a15a5cd2113b99446752b360cd952e0f48f739e1a89c408eaa292988`  
		Last Modified: Thu, 09 Jan 2020 00:15:26 GMT  
		Size: 1.3 MB (1327727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0535005041ff327e280cb332f8a78d861c3bc7b997b38272ba7074e8e84a0806`  
		Last Modified: Thu, 09 Jan 2020 00:15:26 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bf9d5a9aafcb740da79cb71da83f4d162b2153a4663d9c4289f23e0f40eca1`  
		Last Modified: Sat, 18 Jan 2020 00:18:33 GMT  
		Size: 9.8 KB (9850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd63ba224bb0740dd07dcc6a69ba48df1582d5ae2d1f7be352329aa61d212b9`  
		Last Modified: Sat, 18 Jan 2020 00:18:33 GMT  
		Size: 1.2 MB (1223208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8a6ea0061700d796ca5be074e647b44881d3ff558b6f557df4d4a915c28ef5`  
		Last Modified: Sat, 18 Jan 2020 00:18:36 GMT  
		Size: 6.8 MB (6791430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab722617ab91e2d3d558b6cee2e3b98d139bdff07c99421382c92e4cda70b65`  
		Last Modified: Sat, 18 Jan 2020 00:18:56 GMT  
		Size: 72.0 MB (71959335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84604822fb2d2d90eef2bd9580ba42a8b8fe5fc3278e44be093f79a447a7144`  
		Last Modified: Sat, 18 Jan 2020 00:18:34 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; 386

```console
$ docker pull ghost@sha256:cddd1fc9876f1b3fa17ece90b4e62e4d71aa913dc293880db6b0d8b772dce289
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.9 MB (108919985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d208fa4821927336715893879a4ed574420270eb8fa805261c9cadb2828788e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Thu, 09 Jan 2020 01:25:32 GMT
ENV NODE_VERSION=12.14.1
# Thu, 09 Jan 2020 02:03:47 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6906577d7b15cc940f47fc88436ac45f73e5abecd15f09d8f2a9ea337fc2fe5e"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Thu, 09 Jan 2020 02:03:47 GMT
ENV YARN_VERSION=1.21.1
# Thu, 09 Jan 2020 02:03:50 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Thu, 09 Jan 2020 02:03:50 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 09 Jan 2020 02:03:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Jan 2020 02:03:50 GMT
CMD ["node"]
# Fri, 17 Jan 2020 23:39:02 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 17 Jan 2020 23:39:03 GMT
RUN apk add --no-cache 		bash
# Fri, 17 Jan 2020 23:39:04 GMT
ENV NODE_ENV=production
# Fri, 17 Jan 2020 23:39:04 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Fri, 17 Jan 2020 23:39:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 17 Jan 2020 23:39:23 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 17 Jan 2020 23:39:23 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 17 Jan 2020 23:39:23 GMT
ENV GHOST_VERSION=3.3.0
# Fri, 17 Jan 2020 23:42:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 17 Jan 2020 23:42:47 GMT
WORKDIR /var/lib/ghost
# Fri, 17 Jan 2020 23:42:47 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 17 Jan 2020 23:42:47 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 17 Jan 2020 23:42:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Jan 2020 23:42:47 GMT
EXPOSE 2368
# Fri, 17 Jan 2020 23:42:48 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135f2bad84c03e1dfe9830d802376d6efb70dfa7fac368f227eebd27203756a`  
		Last Modified: Thu, 09 Jan 2020 02:05:33 GMT  
		Size: 24.6 MB (24597567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde544997c198d97ab0ff4744c16fb1ec3079651a4e77d35e0df0b8e5d487e32`  
		Last Modified: Thu, 09 Jan 2020 02:05:27 GMT  
		Size: 1.3 MB (1327778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e45c22ffa985e4f115c9dadb6901af67fbcf7b8356ccc493f0534f35ca00b0`  
		Last Modified: Thu, 09 Jan 2020 02:05:27 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6234be622d234985aea10600f2df4b206ce0bb06137cef3c6eff34f27ec07c`  
		Last Modified: Fri, 17 Jan 2020 23:50:40 GMT  
		Size: 10.0 KB (9987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789666365be60206147dd7c9b09adee7489179f291d949921ae301a44097a4bc`  
		Last Modified: Fri, 17 Jan 2020 23:50:41 GMT  
		Size: 1.3 MB (1261278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aedbc73be4e4319fb2164628d0a57f9dc4ca5dc26c8cea35d687dd112700ac`  
		Last Modified: Fri, 17 Jan 2020 23:50:43 GMT  
		Size: 6.8 MB (6791311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c94683c438704c4e83c28fb481c0c115bb64113707009a2efb623e428b1e56`  
		Last Modified: Fri, 17 Jan 2020 23:50:59 GMT  
		Size: 72.1 MB (72126089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05266f7957705b80edae2c9dea7c87da771171d7f06d9668c053cc76efafcb59`  
		Last Modified: Fri, 17 Jan 2020 23:50:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:42c3b4a01a90c36a43b6a2d64789ade9115bc8209e0b50db3786cb3053f15551
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112523034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2755a45ce223c00d76f53741edf6081b7201fdeec53b4fbeb800a1a15efc2c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 24 Dec 2019 19:28:37 GMT
ADD file:4d85451a651e236d899cd849617594eb6babf24079f9b2269134ad06d89bdecc in / 
# Tue, 24 Dec 2019 19:28:38 GMT
CMD ["/bin/sh"]
# Thu, 09 Jan 2020 00:49:48 GMT
ENV NODE_VERSION=12.14.1
# Thu, 09 Jan 2020 01:06:32 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6906577d7b15cc940f47fc88436ac45f73e5abecd15f09d8f2a9ea337fc2fe5e"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Thu, 09 Jan 2020 01:06:35 GMT
ENV YARN_VERSION=1.21.1
# Thu, 09 Jan 2020 01:06:44 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Thu, 09 Jan 2020 01:06:46 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 09 Jan 2020 01:06:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Jan 2020 01:06:50 GMT
CMD ["node"]
# Sat, 18 Jan 2020 00:30:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 18 Jan 2020 00:31:02 GMT
RUN apk add --no-cache 		bash
# Sat, 18 Jan 2020 00:31:04 GMT
ENV NODE_ENV=production
# Sat, 18 Jan 2020 00:31:05 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Sat, 18 Jan 2020 00:31:32 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 18 Jan 2020 00:31:35 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 18 Jan 2020 00:31:37 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 18 Jan 2020 00:31:39 GMT
ENV GHOST_VERSION=3.3.0
# Sat, 18 Jan 2020 00:35:17 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 18 Jan 2020 00:35:24 GMT
WORKDIR /var/lib/ghost
# Sat, 18 Jan 2020 00:35:27 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 18 Jan 2020 00:35:28 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 18 Jan 2020 00:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 00:35:33 GMT
EXPOSE 2368
# Sat, 18 Jan 2020 00:35:35 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:a5dee701e1e87430161d8fce67e77ee5e132bdbafe165c52490a36df654c7660`  
		Last Modified: Tue, 24 Dec 2019 19:29:09 GMT  
		Size: 2.8 MB (2816482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393a61207e28e7b7f638d2a40cb3be864aaebac6776e5986fd2f7eb31cf5cbfc`  
		Last Modified: Thu, 09 Jan 2020 01:26:18 GMT  
		Size: 26.5 MB (26549468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e421503cad7b3a18d1f253612367c70f11f80c36b90cd067bbf3ae19566bd8c0`  
		Last Modified: Thu, 09 Jan 2020 01:26:11 GMT  
		Size: 1.3 MB (1327796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9557e31da6c9314adcb43481278046b7c0345133108a3c4b326ab24655114dbb`  
		Last Modified: Thu, 09 Jan 2020 01:26:11 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d0731404762a14b5b11cdd91dcb4a5d43573ab55bb2843f73d823f6016fd50`  
		Last Modified: Sat, 18 Jan 2020 00:56:37 GMT  
		Size: 10.4 KB (10399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cbbc34f13c3b7af274a2edfd6ae3b1272a20f00f480469219bbbc498627171`  
		Last Modified: Sat, 18 Jan 2020 00:56:46 GMT  
		Size: 1.3 MB (1293115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aae19554d44f84a9d18f1666736553923c76ca01c2d51011a0389580c76c126`  
		Last Modified: Sat, 18 Jan 2020 00:57:02 GMT  
		Size: 6.8 MB (6791413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d97c99f26b8b2a72ea168af729a7e786164d03c22a5f3a17793cd954ddde519`  
		Last Modified: Sat, 18 Jan 2020 00:56:54 GMT  
		Size: 73.7 MB (73733533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d39b3f1cfb48a6d8332f78de538f824fcdcc5fc0e7a2aeade90899f4354e47`  
		Last Modified: Sat, 18 Jan 2020 00:56:37 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:241fc8461eb0515e261d31b636dcf5dfb3aa1c4ccb6ed4beca289e8b0d7472a8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108061978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:209ee57dbd814cc8076f5f8fae44d7700f50fde893a13d27fd5d47b1ec05618d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 24 Dec 2019 20:16:56 GMT
ADD file:d26fbcd308b78da175af74382b16ee1f7a3370ab9d618b306d604d292e72c560 in / 
# Tue, 24 Dec 2019 20:16:56 GMT
CMD ["/bin/sh"]
# Wed, 08 Jan 2020 23:47:43 GMT
ENV NODE_VERSION=12.14.1
# Thu, 09 Jan 2020 00:03:30 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="6906577d7b15cc940f47fc88436ac45f73e5abecd15f09d8f2a9ea337fc2fe5e"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Thu, 09 Jan 2020 00:03:30 GMT
ENV YARN_VERSION=1.21.1
# Thu, 09 Jan 2020 00:03:32 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Thu, 09 Jan 2020 00:03:33 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 09 Jan 2020 00:03:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Jan 2020 00:03:33 GMT
CMD ["node"]
# Fri, 17 Jan 2020 23:46:58 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 17 Jan 2020 23:47:00 GMT
RUN apk add --no-cache 		bash
# Fri, 17 Jan 2020 23:47:00 GMT
ENV NODE_ENV=production
# Fri, 17 Jan 2020 23:47:00 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Fri, 17 Jan 2020 23:47:11 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Fri, 17 Jan 2020 23:47:11 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Fri, 17 Jan 2020 23:47:11 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Fri, 17 Jan 2020 23:47:11 GMT
ENV GHOST_VERSION=3.3.0
# Fri, 17 Jan 2020 23:48:50 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Fri, 17 Jan 2020 23:48:51 GMT
WORKDIR /var/lib/ghost
# Fri, 17 Jan 2020 23:48:51 GMT
VOLUME [/var/lib/ghost/content]
# Fri, 17 Jan 2020 23:48:51 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Fri, 17 Jan 2020 23:48:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Jan 2020 23:48:52 GMT
EXPOSE 2368
# Fri, 17 Jan 2020 23:48:52 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:bca389ebb9be8103bf737251d68f962104771b2f9c1fff1f7ae0207458fa4c86`  
		Last Modified: Tue, 24 Dec 2019 20:17:18 GMT  
		Size: 2.6 MB (2579591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63b021d288b5bb39f4097f3b171f03587ef68ba233019c94224938e7c08302d`  
		Last Modified: Thu, 09 Jan 2020 00:09:18 GMT  
		Size: 24.4 MB (24350636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5a3e0fd18eb6dee58877f3198136b0b8ef159d8a26bde22cc254ed1f12c380`  
		Last Modified: Thu, 09 Jan 2020 00:09:15 GMT  
		Size: 1.3 MB (1327667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf858616b25bdf8333a4917c3b10364e6a5524299ab5875197c0da06db5a961`  
		Last Modified: Thu, 09 Jan 2020 00:09:14 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e10f8c6bacafabf9fc610f342b3f12ad1c5677228fbb39bbd1fd7273da98ff`  
		Last Modified: Fri, 17 Jan 2020 23:56:08 GMT  
		Size: 10.0 KB (9994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395a852fb926b13599325a7cd7a7d3aa49f0ed4ea9a2fd4d20e7eace617f7d3c`  
		Last Modified: Fri, 17 Jan 2020 23:56:08 GMT  
		Size: 1.2 MB (1245200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ec6ded3c9ab5ef518dcdadb13708cdd5798779116838b1046cbef29f837387`  
		Last Modified: Fri, 17 Jan 2020 23:56:09 GMT  
		Size: 6.8 MB (6791344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c761da742bc7ff4349d5325722d3143cbcc2bf932cca73280f97218ca3604dd8`  
		Last Modified: Fri, 17 Jan 2020 23:56:22 GMT  
		Size: 71.8 MB (71756718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499292de80e917244da5ef634304c5d973af4fabd3c7d2cb8963733af9e531df`  
		Last Modified: Fri, 17 Jan 2020 23:56:08 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
