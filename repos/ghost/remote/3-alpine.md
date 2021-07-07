## `ghost:3-alpine`

```console
$ docker pull ghost@sha256:307648de4d721aabb506f929e1131827bc66dff121b0e898ea4c0cb6160daa87
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:3-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:16a43683b3135111c9252961d8bf5059366f97e097091b4d7848db78f74ae7d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110901916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58861e56840a287e5c88d0f2b3dc209f10a0beda40e1b1ae068982f4c9ca086`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 07 Jul 2021 00:30:08 GMT
ENV NODE_VERSION=12.22.2
# Wed, 07 Jul 2021 00:30:14 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="242bc6f948186d64be162ea7fd5c64fe15d5863100db0d0478ae8853533859c2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 07 Jul 2021 00:30:14 GMT
ENV YARN_VERSION=1.22.5
# Wed, 07 Jul 2021 00:30:18 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 07 Jul 2021 00:30:19 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 07 Jul 2021 00:30:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jul 2021 00:30:19 GMT
CMD ["node"]
# Wed, 07 Jul 2021 01:04:58 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 07 Jul 2021 01:04:59 GMT
RUN apk add --no-cache 		bash
# Wed, 07 Jul 2021 01:04:59 GMT
ENV NODE_ENV=production
# Wed, 07 Jul 2021 01:04:59 GMT
ENV GHOST_CLI_VERSION=1.17.3
# Wed, 07 Jul 2021 01:05:19 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 07 Jul 2021 01:05:19 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 07 Jul 2021 01:05:20 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 07 Jul 2021 01:08:18 GMT
ENV GHOST_VERSION=3.42.5
# Wed, 07 Jul 2021 01:09:23 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 07 Jul 2021 01:09:25 GMT
WORKDIR /var/lib/ghost
# Wed, 07 Jul 2021 01:09:25 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 07 Jul 2021 01:09:25 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 07 Jul 2021 01:09:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jul 2021 01:09:26 GMT
EXPOSE 2368
# Wed, 07 Jul 2021 01:09:26 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0afcceedd32b025601b4a6277e4d2bdca9ce64325934f296b8f47eef883c28`  
		Last Modified: Wed, 07 Jul 2021 00:43:22 GMT  
		Size: 24.7 MB (24723278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74fa7d35a79f3a21b78578199b64a952e9969d5f956c140a5e899973f96ae13`  
		Last Modified: Wed, 07 Jul 2021 00:43:17 GMT  
		Size: 2.4 MB (2362396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4cc69f945b6cdf9a03670a9c783d5b1331a7e29ee822d3557f64c2e6da46bd`  
		Last Modified: Wed, 07 Jul 2021 00:43:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949b0c6c1e3b8fce83cacec224b86bf60e4e3e3eef76c8c148a0cb92f9ef354`  
		Last Modified: Wed, 07 Jul 2021 01:10:16 GMT  
		Size: 10.1 KB (10066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d373daf5352aef36cd48632b94a4d5e97b2eff33c5aa3adbe1f0142a8e6c2fc`  
		Last Modified: Wed, 07 Jul 2021 01:10:17 GMT  
		Size: 779.6 KB (779637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d189184905c29a2d5619f163fd1d59ea7d3d83d82e5106accf79e28d42576fe`  
		Last Modified: Wed, 07 Jul 2021 01:10:20 GMT  
		Size: 9.4 MB (9402725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed07765c7bc93c5c1ed62e2fabccc704e76562e5d9a7469a50236d966362d0`  
		Last Modified: Wed, 07 Jul 2021 01:11:28 GMT  
		Size: 70.8 MB (70822419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2ad8a3683e97157778e06e947338751ccc046b0da719ccdf544f5bfdae58bc`  
		Last Modified: Wed, 07 Jul 2021 01:11:13 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:2031b0cfaf2c0ee62e868b82a37ad607006fbaacbfe1d9242887a6f92f58e7c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94848703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8d38d1fba1cd336974580aafb1dadf4485bdb64e9666bbc1ced766bda75e0cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 07 Jul 2021 02:25:24 GMT
ENV NODE_VERSION=12.22.2
# Wed, 07 Jul 2021 02:41:52 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="242bc6f948186d64be162ea7fd5c64fe15d5863100db0d0478ae8853533859c2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 07 Jul 2021 02:41:54 GMT
ENV YARN_VERSION=1.22.5
# Wed, 07 Jul 2021 02:42:02 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 07 Jul 2021 02:42:04 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 07 Jul 2021 02:42:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jul 2021 02:42:05 GMT
CMD ["node"]
# Wed, 07 Jul 2021 03:43:44 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 07 Jul 2021 03:43:46 GMT
RUN apk add --no-cache 		bash
# Wed, 07 Jul 2021 03:43:47 GMT
ENV NODE_ENV=production
# Wed, 07 Jul 2021 03:43:47 GMT
ENV GHOST_CLI_VERSION=1.17.3
# Wed, 07 Jul 2021 03:44:42 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 07 Jul 2021 03:44:43 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 07 Jul 2021 03:44:44 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 07 Jul 2021 04:02:09 GMT
ENV GHOST_VERSION=3.42.5
# Wed, 07 Jul 2021 04:10:38 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 07 Jul 2021 04:10:42 GMT
WORKDIR /var/lib/ghost
# Wed, 07 Jul 2021 04:10:42 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 07 Jul 2021 04:10:43 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 07 Jul 2021 04:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jul 2021 04:10:44 GMT
EXPOSE 2368
# Wed, 07 Jul 2021 04:10:44 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a34f62082e5125bab771aea5280f5a0876905fbe6a04aa63191b5ef269963d2`  
		Last Modified: Wed, 07 Jul 2021 02:52:19 GMT  
		Size: 24.1 MB (24145736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9757f8258bbedcccb1fbf1b2778e1a321570148128f45e45ad35dcf564257f`  
		Last Modified: Wed, 07 Jul 2021 02:52:08 GMT  
		Size: 2.4 MB (2413250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e271606e73e1f9a679fa7e03c0d8c9f6cd720db95c24f9030e7c198e65f2194c`  
		Last Modified: Wed, 07 Jul 2021 02:52:07 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e972311f95eb667db17083f5ba7a3b82c3795e6f78158c4303639aefedc31b`  
		Last Modified: Wed, 07 Jul 2021 04:11:18 GMT  
		Size: 9.9 KB (9910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473e9379fd1fb95a9632e5feed37313be08ac4b1ec992e9729f5b1a02db1cd49`  
		Last Modified: Wed, 07 Jul 2021 04:11:18 GMT  
		Size: 734.0 KB (734018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1662f3aa24c9aa4b94afa28b24d5677f5ca79ab61b9dd8a909664e88fe47f7dd`  
		Last Modified: Wed, 07 Jul 2021 04:11:32 GMT  
		Size: 9.4 MB (9402966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc1da71cbef1ab61e2e555def0c4768c050be8ca5c6559193d3df8f592bb100`  
		Last Modified: Wed, 07 Jul 2021 04:12:34 GMT  
		Size: 55.5 MB (55536745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d9d764ed8439f8a81321b9c4b04c1a1a8bf5e00c9c7f03107a740daf01fb26`  
		Last Modified: Wed, 07 Jul 2021 04:11:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:5f97561b3856fcfcd95a1a101d8fa6aaf9a8315e9bbadc457470a4b8eeb030da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.6 MB (93643266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46f8f01d3ee6820d169b513856f0079384a5e6c112ef190eaa8190cdc7f68f5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:24 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Tue, 15 Jun 2021 23:15:25 GMT
CMD ["/bin/sh"]
# Wed, 07 Jul 2021 03:19:36 GMT
ENV NODE_VERSION=12.22.2
# Wed, 07 Jul 2021 03:34:05 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="242bc6f948186d64be162ea7fd5c64fe15d5863100db0d0478ae8853533859c2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 07 Jul 2021 03:34:06 GMT
ENV YARN_VERSION=1.22.5
# Wed, 07 Jul 2021 03:34:13 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 07 Jul 2021 03:34:14 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 07 Jul 2021 03:34:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jul 2021 03:34:15 GMT
CMD ["node"]
# Wed, 07 Jul 2021 04:17:05 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 07 Jul 2021 04:17:08 GMT
RUN apk add --no-cache 		bash
# Wed, 07 Jul 2021 04:17:09 GMT
ENV NODE_ENV=production
# Wed, 07 Jul 2021 04:17:09 GMT
ENV GHOST_CLI_VERSION=1.17.3
# Wed, 07 Jul 2021 04:17:51 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 07 Jul 2021 04:17:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 07 Jul 2021 04:17:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 07 Jul 2021 04:40:04 GMT
ENV GHOST_VERSION=3.42.5
# Wed, 07 Jul 2021 04:46:32 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 07 Jul 2021 04:46:36 GMT
WORKDIR /var/lib/ghost
# Wed, 07 Jul 2021 04:46:36 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 07 Jul 2021 04:46:37 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 07 Jul 2021 04:46:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jul 2021 04:46:38 GMT
EXPOSE 2368
# Wed, 07 Jul 2021 04:46:38 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71677a64d8f8d6a09a1062e62ee971c73441c76e9ca9c4441a2314da0196c0e4`  
		Last Modified: Wed, 07 Jul 2021 04:04:03 GMT  
		Size: 23.7 MB (23699995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee837d1fb8731497965a63172fd9e9c437391b3a6c80fae11df643314fcfda0b`  
		Last Modified: Wed, 07 Jul 2021 04:03:46 GMT  
		Size: 2.4 MB (2413227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a309bcd52a73268e50866a75b7ff7e58a2fcbfb326d71c445ba6e600a0cb2c92`  
		Last Modified: Wed, 07 Jul 2021 04:03:44 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260305ac196905a6dcb0e75b721514a3109a4a03edeee62129f60ed373ea4ccf`  
		Last Modified: Wed, 07 Jul 2021 04:50:49 GMT  
		Size: 9.7 KB (9689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6694b273dfad04916a7a1f73d12ef1f2e736b2274b116186321cee2cadce9bb7`  
		Last Modified: Wed, 07 Jul 2021 04:50:49 GMT  
		Size: 671.1 KB (671144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36b1d899f77f8a2e02d559d24cf02f517149595c532bfeb5aca77004fd38c9d`  
		Last Modified: Wed, 07 Jul 2021 04:51:04 GMT  
		Size: 9.4 MB (9402843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94db5b692773b09c11f4fb04de84196e3c2040509c7753f8290fce26a413aced`  
		Last Modified: Wed, 07 Jul 2021 04:52:06 GMT  
		Size: 55.0 MB (55036365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7101b0d9f5c864fa14eb1fd75e9d68065c682b776220a13b5ac6eef355938403`  
		Last Modified: Wed, 07 Jul 2021 04:50:49 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:c798f6dec6be846c084e1a3159fe808467c58c2051c45aa7e9b660664771ab42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95907860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1fb90f3368747572741cc2a27b0d07756c1898cc4b4bdeefb8babe071ff39fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Wed, 07 Jul 2021 04:49:16 GMT
ENV NODE_VERSION=12.22.2
# Wed, 07 Jul 2021 05:16:48 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="242bc6f948186d64be162ea7fd5c64fe15d5863100db0d0478ae8853533859c2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 07 Jul 2021 05:16:49 GMT
ENV YARN_VERSION=1.22.5
# Wed, 07 Jul 2021 05:16:53 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 07 Jul 2021 05:16:53 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 07 Jul 2021 05:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jul 2021 05:16:54 GMT
CMD ["node"]
# Wed, 07 Jul 2021 05:43:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 07 Jul 2021 05:43:05 GMT
RUN apk add --no-cache 		bash
# Wed, 07 Jul 2021 05:43:06 GMT
ENV NODE_ENV=production
# Wed, 07 Jul 2021 05:43:06 GMT
ENV GHOST_CLI_VERSION=1.17.3
# Wed, 07 Jul 2021 05:43:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 07 Jul 2021 05:43:26 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 07 Jul 2021 05:43:26 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 07 Jul 2021 05:53:50 GMT
ENV GHOST_VERSION=3.42.5
# Wed, 07 Jul 2021 05:57:02 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 07 Jul 2021 05:57:04 GMT
WORKDIR /var/lib/ghost
# Wed, 07 Jul 2021 05:57:04 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 07 Jul 2021 05:57:05 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 07 Jul 2021 05:57:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Jul 2021 05:57:05 GMT
EXPOSE 2368
# Wed, 07 Jul 2021 05:57:05 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f244cad67b0e8f7732e5977f274a3d99fdbf2443ef3ce10eb9e62c70f0608ea`  
		Last Modified: Wed, 07 Jul 2021 05:33:45 GMT  
		Size: 24.9 MB (24854152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbf3709d143c732364cd1518a6a2b6fcea2012385cd2b6f97a6088918c47233`  
		Last Modified: Wed, 07 Jul 2021 05:33:41 GMT  
		Size: 2.4 MB (2421974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b4dd62501ece4fcdd0fcecf4e518b5dd9b7c61d6464d1cb973bcac56334e3f`  
		Last Modified: Wed, 07 Jul 2021 05:33:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be20261c33be1b914155d5d3dbcfeaa81f32dad67d754f00ac608eea9f5bbb2e`  
		Last Modified: Wed, 07 Jul 2021 05:58:47 GMT  
		Size: 10.0 KB (10006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6711977bfa49cd8a3237f0d96441d268811ae6d6985f9908642f4c8160934f1`  
		Last Modified: Wed, 07 Jul 2021 05:58:48 GMT  
		Size: 791.7 KB (791708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493cc3900aecf0f8477b80f36c6b61b9e602f6d0ee552d41ae54cb3e38b2f9b5`  
		Last Modified: Wed, 07 Jul 2021 05:58:50 GMT  
		Size: 9.4 MB (9402799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d5286dcfe4b32a207b08f5d9708a0075ee91548adbac8b2540feb0b05cb9f3`  
		Last Modified: Wed, 07 Jul 2021 05:59:03 GMT  
		Size: 55.7 MB (55715702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa8cd8992d63b8184351077dbcf9c0acfc66ed68a902824df20a0ca43fc9102`  
		Last Modified: Wed, 07 Jul 2021 05:58:47 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
