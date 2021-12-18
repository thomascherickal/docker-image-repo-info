## `ghost:3-alpine`

```console
$ docker pull ghost@sha256:607b6d188c8aee9254fb4c5deecc6be2dca3114231a604845a6e06a4d49210f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:3-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:8362086f7bf73f64d8f4207cc855cdd667d659cf530ad6bff3554653eaf43810
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e80c4c64660b80edc2833b93cd2272c052801610cc59a5e0be35c690dad79fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 12 Nov 2021 17:20:08 GMT
ADD file:8f5bc5ce64ef781adadca88e4004e17affc72e6f20dbd08b9c478def12fe1dd3 in / 
# Fri, 12 Nov 2021 17:20:08 GMT
CMD ["/bin/sh"]
# Sat, 18 Dec 2021 04:29:08 GMT
ENV NODE_VERSION=12.22.8
# Sat, 18 Dec 2021 04:29:16 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="9cc1d120c404d66a62d6e4daaba361e8e1996bdc5b9643f97bbd1241247332df"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 18 Dec 2021 04:29:17 GMT
ENV YARN_VERSION=1.22.17
# Sat, 18 Dec 2021 04:29:24 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 18 Dec 2021 04:29:24 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 18 Dec 2021 04:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 04:29:24 GMT
CMD ["node"]
# Sat, 18 Dec 2021 07:46:02 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 18 Dec 2021 07:46:03 GMT
RUN apk add --no-cache 		bash
# Sat, 18 Dec 2021 07:46:04 GMT
ENV NODE_ENV=production
# Sat, 18 Dec 2021 07:46:04 GMT
ENV GHOST_CLI_VERSION=1.18.1
# Sat, 18 Dec 2021 07:46:28 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 18 Dec 2021 07:46:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 18 Dec 2021 07:46:29 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 18 Dec 2021 07:46:29 GMT
ENV GHOST_VERSION=3.42.8
# Sat, 18 Dec 2021 07:47:36 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 18 Dec 2021 07:47:38 GMT
WORKDIR /var/lib/ghost
# Sat, 18 Dec 2021 07:47:38 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 18 Dec 2021 07:47:39 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 18 Dec 2021 07:47:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 07:47:39 GMT
EXPOSE 2368
# Sat, 18 Dec 2021 07:47:39 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:8572bc8fb8a32061648dd183b2c0451c82be1bd053a4ea8fae991436b92faebb`  
		Last Modified: Fri, 12 Nov 2021 17:21:10 GMT  
		Size: 2.8 MB (2809473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5d9ca13a73e33fb8208d39ad36967e16a5e59043482dfe2adad3017e96156b`  
		Last Modified: Sat, 18 Dec 2021 04:39:32 GMT  
		Size: 24.7 MB (24741862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488666e3ed33ad7297cf6031141b9a9ff6d8e44550ff068aae3730bdca632351`  
		Last Modified: Sat, 18 Dec 2021 04:39:28 GMT  
		Size: 2.4 MB (2367124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9b3b406668c183eae02d6cf9b9b97377e6df5519e51dab3a07c6c4fd9f61b0`  
		Last Modified: Sat, 18 Dec 2021 04:39:27 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e19d163b23376a147813667476945eb1967f38fe5bb93a2a947cf487e50b1b`  
		Last Modified: Sat, 18 Dec 2021 07:48:30 GMT  
		Size: 10.6 KB (10643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcede974cd328a543aca7784a170246398aac554fab75420d128b6d9b73ec5c9`  
		Last Modified: Sat, 18 Dec 2021 07:48:30 GMT  
		Size: 780.2 KB (780157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f366c7c56a0011a7ab8c215fe5edcfa031ab4e96b4135b7b1607b6d043d8a5d`  
		Last Modified: Sat, 18 Dec 2021 07:48:33 GMT  
		Size: 9.4 MB (9419178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffca934eb9058c00736c92959b800dcff0209009cbc0de87c7cac8820f33b9c8`  
		Last Modified: Sat, 18 Dec 2021 07:48:45 GMT  
		Size: 70.8 MB (70830127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b4c46c5a21a78661ab5dc4daff970d194a8f8d97915eb611232db0a16400e1`  
		Last Modified: Sat, 18 Dec 2021 07:48:30 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:1b717073e7135ceaecd0419c95bee5d43071c364a14db22bfb5a8e7231315b36
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.9 MB (94903007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4507d70733f432ae2a335827cc6224e0a724bbc41538b9c6d09ca28279291775`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 12 Nov 2021 16:50:10 GMT
ADD file:ac6b513ac63ef55629819b36950ebf1d4a6f63acf8a5e81ae847130c0da531c2 in / 
# Fri, 12 Nov 2021 16:50:11 GMT
CMD ["/bin/sh"]
# Sat, 18 Dec 2021 04:04:05 GMT
ENV NODE_VERSION=12.22.8
# Sat, 18 Dec 2021 04:17:13 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="9cc1d120c404d66a62d6e4daaba361e8e1996bdc5b9643f97bbd1241247332df"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 18 Dec 2021 04:17:14 GMT
ENV YARN_VERSION=1.22.17
# Sat, 18 Dec 2021 04:17:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 18 Dec 2021 04:17:23 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 18 Dec 2021 04:17:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 04:17:23 GMT
CMD ["node"]
# Sat, 18 Dec 2021 05:36:32 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 18 Dec 2021 05:36:35 GMT
RUN apk add --no-cache 		bash
# Sat, 18 Dec 2021 05:36:35 GMT
ENV NODE_ENV=production
# Sat, 18 Dec 2021 05:36:36 GMT
ENV GHOST_CLI_VERSION=1.18.1
# Sat, 18 Dec 2021 05:37:44 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 18 Dec 2021 05:37:46 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 18 Dec 2021 05:37:46 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 18 Dec 2021 05:37:47 GMT
ENV GHOST_VERSION=3.42.8
# Sat, 18 Dec 2021 05:46:24 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 18 Dec 2021 05:46:28 GMT
WORKDIR /var/lib/ghost
# Sat, 18 Dec 2021 05:46:28 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 18 Dec 2021 05:46:29 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 18 Dec 2021 05:46:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 05:46:29 GMT
EXPOSE 2368
# Sat, 18 Dec 2021 05:46:30 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cc2d125b852eb4fc619fb0bd6520e82b356b99d979766953db21ffaeeee43767`  
		Last Modified: Fri, 12 Nov 2021 16:52:07 GMT  
		Size: 2.6 MB (2616086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c023e72ac6c2bd63c8ac1258bc871d01ed8c9c2704712be5f905a20258438a`  
		Last Modified: Sat, 18 Dec 2021 04:57:22 GMT  
		Size: 24.2 MB (24163370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5b357f2e631432e5d7572ca50d9bdda424c58955a044a188ab80bcdd277243`  
		Last Modified: Sat, 18 Dec 2021 04:57:05 GMT  
		Size: 2.4 MB (2418347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1bcef3fba7a5f7faf60a4c2aa6ec8aedcf757feb2bcc182ce7bef6ad576f52`  
		Last Modified: Sat, 18 Dec 2021 04:57:03 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b517952e6d8f10115db8fad3e74851f91b6e9c3a0fa931294ae921264efc666`  
		Last Modified: Sat, 18 Dec 2021 05:46:56 GMT  
		Size: 10.5 KB (10475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bfa9bd01ee7c0d5ea08c6d9635d6ed4fe745e281102a7aa07504affd0f2cf9`  
		Last Modified: Sat, 18 Dec 2021 05:46:56 GMT  
		Size: 734.5 KB (734512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e294b897e4fcd333f8586d22677e371a1b5bfc722405e05679550f12e45b0e`  
		Last Modified: Sat, 18 Dec 2021 05:47:10 GMT  
		Size: 9.4 MB (9420187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad74024c6d1cd06ade87317572e9dc7984cb8d56bd028dd9d902bf064e00de0`  
		Last Modified: Sat, 18 Dec 2021 05:48:10 GMT  
		Size: 55.5 MB (55539035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072c31abbf054baec4d6a2360b3200c921f03352321b71196844060db9a613cf`  
		Last Modified: Sat, 18 Dec 2021 05:46:56 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:beef617bb000178297c38f72cdbc2c4cea823bbcc8e63b0d5f8ef1f67a59593f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93711901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44e44a0843639fe17b76d3667a1b78c7d3acf96e93d9936ce3bbcb32bd294590`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 12 Nov 2021 16:58:09 GMT
ADD file:e2781b305845c5b40422993da5f1397cf715a6315eed789e54a7fb53b88ae50a in / 
# Fri, 12 Nov 2021 16:58:10 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 08:38:02 GMT
ENV NODE_VERSION=12.22.7
# Sat, 13 Nov 2021 08:59:47 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 13 Nov 2021 08:59:48 GMT
ENV YARN_VERSION=1.22.15
# Sat, 13 Nov 2021 08:59:55 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 13 Nov 2021 08:59:56 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 13 Nov 2021 08:59:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 08:59:57 GMT
CMD ["node"]
# Sat, 13 Nov 2021 19:15:15 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 13 Nov 2021 19:15:18 GMT
RUN apk add --no-cache 		bash
# Sat, 13 Nov 2021 19:15:18 GMT
ENV NODE_ENV=production
# Wed, 24 Nov 2021 23:06:00 GMT
ENV GHOST_CLI_VERSION=1.18.1
# Wed, 24 Nov 2021 23:06:52 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 24 Nov 2021 23:06:54 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 24 Nov 2021 23:06:54 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 14 Dec 2021 23:39:08 GMT
ENV GHOST_VERSION=3.42.8
# Tue, 14 Dec 2021 23:45:45 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 14 Dec 2021 23:45:49 GMT
WORKDIR /var/lib/ghost
# Tue, 14 Dec 2021 23:45:49 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 14 Dec 2021 23:45:50 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 14 Dec 2021 23:45:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Dec 2021 23:45:51 GMT
EXPOSE 2368
# Tue, 14 Dec 2021 23:45:51 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:80ca8924263de5db5111df92957a4aee8d9538912e596b729a38795558b75a55`  
		Last Modified: Fri, 12 Nov 2021 17:00:14 GMT  
		Size: 2.4 MB (2418296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087046ac52d5362279aef6b4123346ee113d85b4b0fcb8289e431a99ca19d77b`  
		Last Modified: Sat, 13 Nov 2021 10:06:41 GMT  
		Size: 23.7 MB (23729266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d0b4ce47db3ab08043d0a30ca5a14e975a8ab80cb55e2c0c0db7418b7e5bd8`  
		Last Modified: Sat, 13 Nov 2021 10:06:24 GMT  
		Size: 2.4 MB (2418458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcb90ce023ffb895c541fbde97ebe241ef1b291231f37271664050afbc6d73e`  
		Last Modified: Sat, 13 Nov 2021 10:06:23 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050c9570e639df08b1960d2b6c0dec97a3bd9cf0da9a280a611b7f90dc293594`  
		Last Modified: Sat, 13 Nov 2021 19:24:02 GMT  
		Size: 10.3 KB (10260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93a36ba4ca03d400f2cbfcec3f215a90f5805ad83d1ced2699ed6b9acdf35de`  
		Last Modified: Sat, 13 Nov 2021 19:24:02 GMT  
		Size: 671.9 KB (671884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6d43caf6b8741a9a89ee928a9848f45dd4da40937ae7f2d2dd579ee0bb09a5`  
		Last Modified: Wed, 24 Nov 2021 23:17:50 GMT  
		Size: 9.4 MB (9426675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfb9c9716f4d017c8e043fb4177f80084f639b8f9a9075dd40013006e2a9346`  
		Last Modified: Tue, 14 Dec 2021 23:51:08 GMT  
		Size: 55.0 MB (55036063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac18dd523d15cebbae5c6a531eb2f40a9d6a65b51dff07f1224b196243be7f4`  
		Last Modified: Tue, 14 Dec 2021 23:49:48 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:6d1ee17bb574406440d1f26eead9e60cacb1518e2566ff14f7947d2aa88de50f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95964653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb6987f680282d9a512c8e31eed626e997cd21b124cadb8d09ad32f0dc18f8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:12 GMT
ADD file:56fd98a7471802f25445d89571945fd5f6b0d87ca0d53d5dc664c0087b39fa14 in / 
# Fri, 12 Nov 2021 16:40:12 GMT
CMD ["/bin/sh"]
# Sat, 18 Dec 2021 03:44:55 GMT
ENV NODE_VERSION=12.22.8
# Sat, 18 Dec 2021 04:00:23 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="9cc1d120c404d66a62d6e4daaba361e8e1996bdc5b9643f97bbd1241247332df"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 18 Dec 2021 04:00:24 GMT
ENV YARN_VERSION=1.22.17
# Sat, 18 Dec 2021 04:00:29 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 18 Dec 2021 04:00:31 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 18 Dec 2021 04:00:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 04:00:32 GMT
CMD ["node"]
# Sat, 18 Dec 2021 07:31:47 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 18 Dec 2021 07:31:48 GMT
RUN apk add --no-cache 		bash
# Sat, 18 Dec 2021 07:31:49 GMT
ENV NODE_ENV=production
# Sat, 18 Dec 2021 07:31:50 GMT
ENV GHOST_CLI_VERSION=1.18.1
# Sat, 18 Dec 2021 07:32:13 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 18 Dec 2021 07:32:14 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 18 Dec 2021 07:32:15 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 18 Dec 2021 07:32:16 GMT
ENV GHOST_VERSION=3.42.8
# Sat, 18 Dec 2021 07:35:20 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 18 Dec 2021 07:35:24 GMT
WORKDIR /var/lib/ghost
# Sat, 18 Dec 2021 07:35:27 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 18 Dec 2021 07:35:30 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 18 Dec 2021 07:35:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 07:35:36 GMT
EXPOSE 2368
# Sat, 18 Dec 2021 07:35:39 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:8c28cc2212ffeecd224e6ac2336baf880f2958f01d082bf60c0bb8156fbb1701`  
		Last Modified: Fri, 12 Nov 2021 16:41:25 GMT  
		Size: 2.7 MB (2720990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73834d5d0687532e7f3ec812ca7ae05f4ded7e1ed4b76912e9e2d5c121bd6813`  
		Last Modified: Sat, 18 Dec 2021 04:48:34 GMT  
		Size: 24.9 MB (24875340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d769b1578d5acc59617404d262b1f98ce508e4f83c9a968aeeadd514b6fa120`  
		Last Modified: Sat, 18 Dec 2021 04:48:29 GMT  
		Size: 2.4 MB (2425655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1676865a74f075e6990b285c8a8c30b30d281aee2f0baafbcf0e33924b8935`  
		Last Modified: Sat, 18 Dec 2021 04:48:29 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c90957ffa085e82cfac7b340121d487df29de14d7ed6f4280e28a458683759d`  
		Last Modified: Sat, 18 Dec 2021 07:36:36 GMT  
		Size: 10.5 KB (10508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3f02296c0c3ac70a82d0c8743e9793d596f26d9a877bafb417fa8959c32056`  
		Last Modified: Sat, 18 Dec 2021 07:36:37 GMT  
		Size: 792.1 KB (792132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3fe713a940ef05a85f47db0862b23089af01796a5e13ce83841eda71142667`  
		Last Modified: Sat, 18 Dec 2021 07:36:39 GMT  
		Size: 9.4 MB (9418939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2109190f64e8056d14b91ab4babe42748957801575d33c1d4384b998feccbfcd`  
		Last Modified: Sat, 18 Dec 2021 07:36:51 GMT  
		Size: 55.7 MB (55720094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61a0f30d27e3cf6d92b1cbc26b348025012200e5e5aadec905413251d4231ff`  
		Last Modified: Sat, 18 Dec 2021 07:36:36 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
