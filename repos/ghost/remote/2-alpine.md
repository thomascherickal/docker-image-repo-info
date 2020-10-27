## `ghost:2-alpine`

```console
$ docker pull ghost@sha256:7a5302f2d02b97d37276aa15dc6a2dd7d50a814e9d4cea41d5e4c32b4ccef099
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
$ docker pull ghost@sha256:76db80cf5c2dd1e0c40d55f0d00ddec43fdd25ed63b821646c9d5182b90e7ba6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.9 MB (107918133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:250da8ae63f65fe40512f8f763fc26cab2fe760c3d50fd633e9b78f5f1d1b115`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 15:27:27 GMT
ENV NODE_VERSION=10.22.1
# Fri, 02 Oct 2020 21:31:50 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 02 Oct 2020 21:31:51 GMT
ENV YARN_VERSION=1.22.4
# Fri, 02 Oct 2020 21:31:53 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 02 Oct 2020 21:31:53 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Fri, 02 Oct 2020 21:31:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Oct 2020 21:31:54 GMT
CMD ["node"]
# Fri, 02 Oct 2020 21:55:32 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Fri, 02 Oct 2020 21:55:34 GMT
RUN apk add --no-cache 		bash
# Fri, 02 Oct 2020 21:55:34 GMT
ENV NODE_ENV=production
# Mon, 12 Oct 2020 22:28:34 GMT
ENV GHOST_CLI_VERSION=1.15.0
# Mon, 12 Oct 2020 22:28:51 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Mon, 12 Oct 2020 22:28:52 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Mon, 12 Oct 2020 22:28:52 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 12 Oct 2020 22:28:52 GMT
ENV GHOST_VERSION=2.38.2
# Mon, 12 Oct 2020 22:29:43 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 12 Oct 2020 22:29:44 GMT
WORKDIR /var/lib/ghost
# Mon, 12 Oct 2020 22:29:44 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 12 Oct 2020 22:29:44 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 12 Oct 2020 22:29:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 22:29:45 GMT
EXPOSE 2368
# Mon, 12 Oct 2020 22:29:45 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b94f5c25d22b3cb16c1622dd71d4d69cd0e5abd624e82b272cd23d72743ff77`  
		Last Modified: Fri, 02 Oct 2020 21:36:54 GMT  
		Size: 22.5 MB (22451143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadffac7f58bcdeb36823fe4da75f59c055dd3d34c7af1eee03a0cfdf2a6f1df`  
		Last Modified: Fri, 02 Oct 2020 21:36:48 GMT  
		Size: 2.3 MB (2344698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a934b75286fbda4597e51fb2ffae322646c4b2be15c6ce556659aeb6c22f86b`  
		Last Modified: Fri, 02 Oct 2020 21:36:47 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c685bd0550238e6a1e30126edd18f7c2092a7203ed99d4baeb212a1a92cfd02d`  
		Last Modified: Fri, 02 Oct 2020 21:58:49 GMT  
		Size: 9.9 KB (9909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa855ad208b0e4894dbc9aba9e7ba27720f3b3594b9daac323d92b69fb3a99`  
		Last Modified: Fri, 02 Oct 2020 21:58:49 GMT  
		Size: 780.5 KB (780526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d49905a804cc50f954484f535ee2c119fa44956deb36a615b9137bc264f1a6`  
		Last Modified: Mon, 12 Oct 2020 22:31:56 GMT  
		Size: 7.4 MB (7447890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3924a2e2f17b08bddf7c37cfda9aba8d9efb8216531611abe3b2886754e0db55`  
		Last Modified: Mon, 12 Oct 2020 22:32:06 GMT  
		Size: 72.1 MB (72069818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28db79fe884839e24c8ee63d27d541ecc07559496284cbdf35fab14b9be8e08`  
		Last Modified: Mon, 12 Oct 2020 22:31:53 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:e9164622ffc4c944c3a5b0d711d505f8abbd639c9373d6a2e6943849a7491ef7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.9 MB (91941509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f09b1958c3a89491847a9ff47014ebce3dec2ee53c238ff95ad12738f15572e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:06:47 GMT
ENV NODE_VERSION=10.22.1
# Fri, 02 Oct 2020 23:48:45 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 02 Oct 2020 23:48:51 GMT
ENV YARN_VERSION=1.22.4
# Fri, 02 Oct 2020 23:49:00 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 02 Oct 2020 23:49:01 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Fri, 02 Oct 2020 23:49:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Oct 2020 23:49:04 GMT
CMD ["node"]
# Sat, 03 Oct 2020 00:09:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 03 Oct 2020 00:09:33 GMT
RUN apk add --no-cache 		bash
# Sat, 03 Oct 2020 00:09:34 GMT
ENV NODE_ENV=production
# Mon, 12 Oct 2020 23:05:47 GMT
ENV GHOST_CLI_VERSION=1.15.0
# Mon, 12 Oct 2020 23:06:57 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Mon, 12 Oct 2020 23:07:14 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Mon, 12 Oct 2020 23:07:22 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 12 Oct 2020 23:07:26 GMT
ENV GHOST_VERSION=2.38.2
# Mon, 12 Oct 2020 23:14:09 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 12 Oct 2020 23:14:18 GMT
WORKDIR /var/lib/ghost
# Mon, 12 Oct 2020 23:14:20 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 12 Oct 2020 23:14:21 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 12 Oct 2020 23:14:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 23:14:24 GMT
EXPOSE 2368
# Mon, 12 Oct 2020 23:14:26 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b352d436471345198b31970d9ff7732650036ebfc426653dc1ace71fe13c20`  
		Last Modified: Fri, 02 Oct 2020 23:56:27 GMT  
		Size: 21.9 MB (21858504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bb62fd144811d9a330c608646641b16582a83b620bc4ae8b4db8f1c06df923`  
		Last Modified: Fri, 02 Oct 2020 23:56:17 GMT  
		Size: 2.4 MB (2360912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b6e09c14f759dff3f24fe8408a9872cf93a9bef507ca9284b41dc7639a4647`  
		Last Modified: Fri, 02 Oct 2020 23:56:15 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293f965e1d526ca159b55fa17223034d0da027a38916fc4a7ecc41e33202aa5c`  
		Last Modified: Sat, 03 Oct 2020 00:17:55 GMT  
		Size: 9.7 KB (9733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810f7d4ab829d28a85fc405c298c2cd344f0550a3c7b05b975938c189c4b5578`  
		Last Modified: Sat, 03 Oct 2020 00:17:53 GMT  
		Size: 733.5 KB (733455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf9732676caac7bf04da757fb989f3704a4e0dd856594c1281af7c14e91b4c0`  
		Last Modified: Mon, 12 Oct 2020 23:14:48 GMT  
		Size: 7.4 MB (7448905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2d93fea113906f3b2edda133bb490e042cc8a93c45071cfba320d6db4dc492`  
		Last Modified: Mon, 12 Oct 2020 23:15:07 GMT  
		Size: 56.9 MB (56909236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e7d4fef35f0dabbdd4fff2350a8f9fac62d8f3844a7b121c6a366976893b14`  
		Last Modified: Mon, 12 Oct 2020 23:14:41 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:79967f78daf4473467c5cbf003f96f428d80517d5e9c4dc08c4bdbeff7308fc6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90812379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6dee419dd6d5847e077fb8ddf8f24767878d20b0da50781c8cb5c7780fb37875`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 20:05:01 GMT
ENV NODE_VERSION=10.22.1
# Fri, 02 Oct 2020 23:58:46 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 02 Oct 2020 23:58:51 GMT
ENV YARN_VERSION=1.22.4
# Fri, 02 Oct 2020 23:58:57 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 02 Oct 2020 23:59:00 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Fri, 02 Oct 2020 23:59:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Oct 2020 23:59:04 GMT
CMD ["node"]
# Sat, 03 Oct 2020 00:23:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 03 Oct 2020 00:23:35 GMT
RUN apk add --no-cache 		bash
# Sat, 03 Oct 2020 00:23:38 GMT
ENV NODE_ENV=production
# Mon, 12 Oct 2020 22:12:38 GMT
ENV GHOST_CLI_VERSION=1.15.0
# Mon, 12 Oct 2020 22:13:20 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Mon, 12 Oct 2020 22:13:22 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Mon, 12 Oct 2020 22:13:23 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 12 Oct 2020 22:13:23 GMT
ENV GHOST_VERSION=2.38.2
# Tue, 27 Oct 2020 00:17:21 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 27 Oct 2020 00:17:24 GMT
WORKDIR /var/lib/ghost
# Tue, 27 Oct 2020 00:17:25 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 27 Oct 2020 00:17:25 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 27 Oct 2020 00:17:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 00:17:26 GMT
EXPOSE 2368
# Tue, 27 Oct 2020 00:17:27 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1505296873a17ab1f8cdc4e82b0d12ffefde768586cc0d0dc54699a8bf0616`  
		Last Modified: Sat, 03 Oct 2020 00:09:29 GMT  
		Size: 21.5 MB (21458497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3c14245845de32502057f62ab5f179fa3a817e9ff77a7b3d95fafb93cc8c9d`  
		Last Modified: Sat, 03 Oct 2020 00:09:22 GMT  
		Size: 2.4 MB (2360975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7212b1dafd85952cab55a9e613038036d576618d060c6fa79abc651cddc645f9`  
		Last Modified: Sat, 03 Oct 2020 00:09:21 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21beee18b89a91aee30e81476f4f963c8b4df647f6973148f884b225365ad3b4`  
		Last Modified: Sat, 03 Oct 2020 00:31:56 GMT  
		Size: 9.5 KB (9522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5a3e0fb7779af98f703efcf1f970c7b7a6b2eed147960ffba57561a713ccb8`  
		Last Modified: Sat, 03 Oct 2020 00:31:56 GMT  
		Size: 669.0 KB (669046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f392feb3f8ffe39e9da909a732868305df8709abf6ce7bea707d3f780c941e`  
		Last Modified: Mon, 12 Oct 2020 22:19:35 GMT  
		Size: 7.4 MB (7447536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ef2f9bd2a33ed760b3b1a6c02ef3b7875caef047c92ffc03b28ccf789846fb`  
		Last Modified: Tue, 27 Oct 2020 00:19:34 GMT  
		Size: 56.4 MB (56443912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3830e795ef3e6d83a6f6c2f75c30cecb8510adcd17a7577270027c461d1b75c2`  
		Last Modified: Tue, 27 Oct 2020 00:19:12 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:0875102ba83e5bcf294391b8c04e472187a81858575199bf0fa1e39bb7b71167
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93114493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c40e6baeafcc0853b294a26452c148e70aa90428a4a28d99602a2697af1a63c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:25:10 GMT
ENV NODE_VERSION=10.22.1
# Fri, 02 Oct 2020 23:44:02 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 02 Oct 2020 23:44:05 GMT
ENV YARN_VERSION=1.22.4
# Fri, 02 Oct 2020 23:44:17 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 02 Oct 2020 23:44:20 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Fri, 02 Oct 2020 23:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Oct 2020 23:44:24 GMT
CMD ["node"]
# Sat, 03 Oct 2020 00:10:20 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 03 Oct 2020 00:10:24 GMT
RUN apk add --no-cache 		bash
# Sat, 03 Oct 2020 00:10:25 GMT
ENV NODE_ENV=production
# Mon, 12 Oct 2020 23:31:35 GMT
ENV GHOST_CLI_VERSION=1.15.0
# Mon, 12 Oct 2020 23:32:06 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Mon, 12 Oct 2020 23:32:08 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Mon, 12 Oct 2020 23:32:09 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 12 Oct 2020 23:32:09 GMT
ENV GHOST_VERSION=2.38.2
# Tue, 27 Oct 2020 00:58:53 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 27 Oct 2020 00:58:58 GMT
WORKDIR /var/lib/ghost
# Tue, 27 Oct 2020 00:58:58 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 27 Oct 2020 00:58:59 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 27 Oct 2020 00:59:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 00:59:01 GMT
EXPOSE 2368
# Tue, 27 Oct 2020 00:59:02 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafee548faa95e20f1dbf3acddd8d7d1348af986dbde1e1846b63e928e628c55`  
		Last Modified: Fri, 02 Oct 2020 23:56:32 GMT  
		Size: 22.7 MB (22681247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d4627dc65410235107d69896e0182e756d961b30bc1267b689bba191346dd8`  
		Last Modified: Fri, 02 Oct 2020 23:56:22 GMT  
		Size: 2.4 MB (2401265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8002d69d1979d4c894d92dfcc7b33e6a001efe4c689608cc2af1ad6907e499e`  
		Last Modified: Fri, 02 Oct 2020 23:56:22 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a71f1e8dff50541cd2b5bffc9d19dcb6f98f046b0b2d5fbaaecf29f6aa57c75`  
		Last Modified: Sat, 03 Oct 2020 00:17:36 GMT  
		Size: 9.8 KB (9844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60883fcf443feb552da4d0ff7caaa32b4ebac11f720ca24b9a6b7255e1bc936`  
		Last Modified: Sat, 03 Oct 2020 00:17:36 GMT  
		Size: 792.1 KB (792145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5157d28931f13fc075552468f7dca7a40e336a49ca9ea0a6816646e1f3b8a8`  
		Last Modified: Mon, 12 Oct 2020 23:37:56 GMT  
		Size: 7.4 MB (7447728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198c60ddc6c0066bd947bb94437672edd3b5153e8d8f19d0d5ea4f1cdd1eb215`  
		Last Modified: Tue, 27 Oct 2020 01:00:42 GMT  
		Size: 57.1 MB (57057010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be4ec3588f1d56c07eb6c8d5184f5abc3456d53b12e9226a6949acee72f3d0e`  
		Last Modified: Tue, 27 Oct 2020 01:00:25 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; 386

```console
$ docker pull ghost@sha256:97de36aa7efc27414339e342f7ec0c671c799da8a9d4b0f395c1ae303c119f86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93254571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60970cb55da55e157167c1ba75477c8a88fabdc8c457b74e556917ca9e7dd46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 18:31:39 GMT
ENV NODE_VERSION=10.22.1
# Sat, 03 Oct 2020 00:08:36 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 03 Oct 2020 00:08:37 GMT
ENV YARN_VERSION=1.22.4
# Sat, 03 Oct 2020 00:08:40 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 03 Oct 2020 00:08:40 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Sat, 03 Oct 2020 00:08:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Oct 2020 00:08:40 GMT
CMD ["node"]
# Sat, 03 Oct 2020 00:16:23 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 03 Oct 2020 00:16:24 GMT
RUN apk add --no-cache 		bash
# Sat, 03 Oct 2020 00:16:25 GMT
ENV NODE_ENV=production
# Mon, 12 Oct 2020 22:39:23 GMT
ENV GHOST_CLI_VERSION=1.15.0
# Mon, 12 Oct 2020 22:39:46 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Mon, 12 Oct 2020 22:39:46 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Mon, 12 Oct 2020 22:39:47 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 12 Oct 2020 22:39:47 GMT
ENV GHOST_VERSION=2.38.2
# Tue, 27 Oct 2020 00:41:41 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 27 Oct 2020 00:41:42 GMT
WORKDIR /var/lib/ghost
# Tue, 27 Oct 2020 00:41:42 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 27 Oct 2020 00:41:42 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 27 Oct 2020 00:41:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 00:41:43 GMT
EXPOSE 2368
# Tue, 27 Oct 2020 00:41:43 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153c7e596857c8f1730ecdf5fdd4bd66e2a8f340468628a89492f1a7b08b7ed8`  
		Last Modified: Sat, 03 Oct 2020 00:09:49 GMT  
		Size: 22.7 MB (22655209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a15862ae807d9e30271efdbdff70cd8e170f02afd6b6306275c1943510c47d5`  
		Last Modified: Sat, 03 Oct 2020 00:09:44 GMT  
		Size: 2.4 MB (2360964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9974f50e9976746827c8d328d9e04cbf2320bc5b4d5292df995e37a63e49ad30`  
		Last Modified: Sat, 03 Oct 2020 00:09:42 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b047121947a094c53db9ad363062fa02dd89fad4a759c16a8cba915242039a`  
		Last Modified: Sat, 03 Oct 2020 00:22:01 GMT  
		Size: 10.0 KB (9983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaddea27276411268e50e668e5f599517d08e2d5081e4fd8766b9f008b98b871`  
		Last Modified: Sat, 03 Oct 2020 00:22:01 GMT  
		Size: 831.1 KB (831099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123c9dcdc03f79d42d40e8bcb119b14f90c07590a177670c950063c267825f58`  
		Last Modified: Mon, 12 Oct 2020 22:43:19 GMT  
		Size: 7.4 MB (7447838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeccdd42790e5991e351743fda428dae98aba9c4de532179284081097cb4b31`  
		Last Modified: Tue, 27 Oct 2020 00:42:22 GMT  
		Size: 57.1 MB (57140234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08125158b330e864f3ce196d0fb38085bc1a25f88ad5aaeb8f95589f910cdea0`  
		Last Modified: Tue, 27 Oct 2020 00:42:04 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:d19d1bb6d9e8b53d49d5e1e3fd4333d23ea6fe57365cb19453b4aba3895c1ca9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95895500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af10ce35bfcba019dde1b214a55d3a2653cde8215ede70fccd3f1f70ee0e6600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 19:03:12 GMT
ENV NODE_VERSION=10.22.1
# Sat, 03 Oct 2020 03:02:40 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 03 Oct 2020 03:02:49 GMT
ENV YARN_VERSION=1.22.4
# Sat, 03 Oct 2020 03:03:11 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 03 Oct 2020 03:03:14 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Sat, 03 Oct 2020 03:03:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Oct 2020 03:03:33 GMT
CMD ["node"]
# Sat, 03 Oct 2020 03:44:11 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 03 Oct 2020 03:44:24 GMT
RUN apk add --no-cache 		bash
# Sat, 03 Oct 2020 03:44:28 GMT
ENV NODE_ENV=production
# Mon, 12 Oct 2020 23:05:05 GMT
ENV GHOST_CLI_VERSION=1.15.0
# Mon, 12 Oct 2020 23:05:56 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Mon, 12 Oct 2020 23:06:01 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Mon, 12 Oct 2020 23:06:02 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 12 Oct 2020 23:06:04 GMT
ENV GHOST_VERSION=2.38.2
# Tue, 27 Oct 2020 00:45:53 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 27 Oct 2020 00:46:07 GMT
WORKDIR /var/lib/ghost
# Tue, 27 Oct 2020 00:46:10 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 27 Oct 2020 00:46:11 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 27 Oct 2020 00:46:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 00:46:16 GMT
EXPOSE 2368
# Tue, 27 Oct 2020 00:46:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911b051b5e51e7b99b3b1f2ace8bef6b2c2c10fd5810e76aeb062ef41aa91b67`  
		Last Modified: Sat, 03 Oct 2020 03:17:12 GMT  
		Size: 24.4 MB (24409254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1baf017d8042a9a2124021ee44c837d98d2fd3d7becdb30421aa7caf298944`  
		Last Modified: Sat, 03 Oct 2020 03:17:05 GMT  
		Size: 2.4 MB (2401104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b8428f5dc27dfc711917216e39fe1ef4817c92c99ed34c353c7105eef0fe07`  
		Last Modified: Sat, 03 Oct 2020 03:17:04 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9705042ce37a9a79de6ea15ee04120100fedad2baa8c38296dbd4f46be3c56`  
		Last Modified: Sat, 03 Oct 2020 03:59:27 GMT  
		Size: 10.4 KB (10408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900e81b0587af32828c4d66197bd4abe3a05ff0fdf4ff13e8c08ace4665eb654`  
		Last Modified: Sat, 03 Oct 2020 03:59:31 GMT  
		Size: 862.6 KB (862613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5d059a3c9a085d3bbdfa6d44724cf48cc6d1d92dce1413261b4fb5519f3f01`  
		Last Modified: Mon, 12 Oct 2020 23:17:33 GMT  
		Size: 7.4 MB (7447594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af16399747c1faa3f704b31113e24d7eed2e9bdb5752fb865b9f7dcdf767813`  
		Last Modified: Tue, 27 Oct 2020 00:48:13 GMT  
		Size: 57.9 MB (57941854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c3b11c8e846ee87d8b202cf717e7b4c8a038bb410e3499fa54b015de70dcf1`  
		Last Modified: Tue, 27 Oct 2020 00:47:57 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:2-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:f0575a611f629dc56915ade466ed48bc05013febcc615e9753717ed148360e62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92690037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21e372caa1e4887d9a6afcf70ccd6a6da4af57476712baaddd2451e3a323c24b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 16 Sep 2020 19:04:10 GMT
ENV NODE_VERSION=10.22.1
# Sat, 03 Oct 2020 00:49:17 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="72f0693db768ef07c712e7a575bd6914b8a74338e91e9e969c8d7e2a832d38f3"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 03 Oct 2020 00:49:19 GMT
ENV YARN_VERSION=1.22.4
# Sat, 03 Oct 2020 00:49:21 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 03 Oct 2020 00:49:22 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Sat, 03 Oct 2020 00:49:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Oct 2020 00:49:22 GMT
CMD ["node"]
# Sat, 03 Oct 2020 00:59:38 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 03 Oct 2020 00:59:39 GMT
RUN apk add --no-cache 		bash
# Sat, 03 Oct 2020 00:59:39 GMT
ENV NODE_ENV=production
# Mon, 12 Oct 2020 22:51:32 GMT
ENV GHOST_CLI_VERSION=1.15.0
# Mon, 12 Oct 2020 22:51:48 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Mon, 12 Oct 2020 22:51:50 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Mon, 12 Oct 2020 22:51:50 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 12 Oct 2020 22:51:50 GMT
ENV GHOST_VERSION=2.38.2
# Tue, 27 Oct 2020 01:00:13 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 27 Oct 2020 01:00:26 GMT
WORKDIR /var/lib/ghost
# Tue, 27 Oct 2020 01:00:26 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 27 Oct 2020 01:00:27 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 27 Oct 2020 01:00:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 01:00:27 GMT
EXPOSE 2368
# Tue, 27 Oct 2020 01:00:28 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9682ac970b82cf09d92b6a77c6416c06ee200ad028d0ce80575af2a1506ac5be`  
		Last Modified: Sat, 03 Oct 2020 00:53:13 GMT  
		Size: 22.5 MB (22472816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa4a053c94d94d932675d44cd651bcc1456bc82cadacbf635c70ca5dfd5f7d6`  
		Last Modified: Sat, 03 Oct 2020 00:53:10 GMT  
		Size: 2.4 MB (2396887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7ca57a887e95168e60033b38b8e9b16de259fbe2bf84be13ae37b9bf23d3f4`  
		Last Modified: Sat, 03 Oct 2020 00:53:09 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3538246b8868f90c0a4269d168f8a24375daba739304fa58067dd5b1205359`  
		Last Modified: Sat, 03 Oct 2020 01:02:44 GMT  
		Size: 10.0 KB (10001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5b158d24a177cfa1e9033da7126840b077d24844bdae1905b763b99e1ecb8b`  
		Last Modified: Sat, 03 Oct 2020 01:02:45 GMT  
		Size: 813.9 KB (813878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c892dcbab45dc09fea591e4de2fc8776e88e266f1792040594501b8068b3d2b9`  
		Last Modified: Mon, 12 Oct 2020 22:56:00 GMT  
		Size: 7.4 MB (7447831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d7cf94cd0d9f45d9d04d144e4de1fd2cfe8d254d7c6f5b89a5358bcbd0abd5`  
		Last Modified: Tue, 27 Oct 2020 01:01:48 GMT  
		Size: 57.0 MB (56964938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810a4a70167054cb1aae890fe70874894614aafc5b06cf7a11579920bdc9aea7`  
		Last Modified: Tue, 27 Oct 2020 01:01:39 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
