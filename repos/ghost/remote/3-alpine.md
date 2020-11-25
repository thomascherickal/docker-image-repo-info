## `ghost:3-alpine`

```console
$ docker pull ghost@sha256:1c814a9bf9f94f4e20618dda6decdaad5aa6a694c016d5b1d99e15b0f0312e53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:3-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:4b932614701a855a9abd0e3568f9ed17e31c23ac1669ff23a64a3b8c4731c801
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115094273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6afeeeaae60ecda21b58ba006e6af127ea05c79170628ad66d6f601b8bc60b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Wed, 25 Nov 2020 00:38:07 GMT
ENV NODE_VERSION=12.20.0
# Wed, 25 Nov 2020 00:38:13 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="9a25589439ebec4e74fc2652893b5887b33130c0dd7dad2daa1d200024fa676c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       1C050899334244A8AF75E53792EF661D867B9DFA       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 25 Nov 2020 00:38:13 GMT
ENV YARN_VERSION=1.22.5
# Wed, 25 Nov 2020 00:38:16 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 25 Nov 2020 00:38:16 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 25 Nov 2020 00:38:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:38:16 GMT
CMD ["node"]
# Wed, 25 Nov 2020 04:33:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 25 Nov 2020 04:33:06 GMT
RUN apk add --no-cache 		bash
# Wed, 25 Nov 2020 04:33:06 GMT
ENV NODE_ENV=production
# Wed, 25 Nov 2020 04:33:07 GMT
ENV GHOST_CLI_VERSION=1.15.2
# Wed, 25 Nov 2020 04:33:36 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 25 Nov 2020 04:33:37 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 25 Nov 2020 04:33:37 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 25 Nov 2020 04:33:37 GMT
ENV GHOST_VERSION=3.38.3
# Wed, 25 Nov 2020 04:35:23 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 25 Nov 2020 04:35:25 GMT
WORKDIR /var/lib/ghost
# Wed, 25 Nov 2020 04:35:25 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 25 Nov 2020 04:35:25 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 25 Nov 2020 04:35:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 04:35:25 GMT
EXPOSE 2368
# Wed, 25 Nov 2020 04:35:26 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acae492d4aa9f9e42b463125dab7185271949a0f0c1360af15b454a4dc998aae`  
		Last Modified: Wed, 25 Nov 2020 00:46:16 GMT  
		Size: 25.0 MB (24967950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5796282d0e2d0b709b554e87a776009f523f3b0b3f678bbd979d050eda9ef22f`  
		Last Modified: Wed, 25 Nov 2020 00:46:08 GMT  
		Size: 2.4 MB (2362049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c2b8306406924333d7abfbcec03a796122273160eab2cae37770a96cf90b2b9`  
		Last Modified: Wed, 25 Nov 2020 00:46:07 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86acd64fa03ad4fe40ed7057bf35b0e523337828d7f2c7bef1765f2a2a41ddeb`  
		Last Modified: Wed, 25 Nov 2020 04:36:15 GMT  
		Size: 10.1 KB (10070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c60de49796acacbbcbaf54d63aa501c877efb7cd21329464b165cf2ae072790`  
		Last Modified: Wed, 25 Nov 2020 04:36:16 GMT  
		Size: 779.6 KB (779608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff0f370569ada0456787bf81d714faaf5e48a90078f5a6ba5e93a4e6186afd5`  
		Last Modified: Wed, 25 Nov 2020 04:36:18 GMT  
		Size: 7.5 MB (7456189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3397d7a639db2df6e3baca0463f5bdd7c62cc6636acbf2fd19535aa8ca362092`  
		Last Modified: Wed, 25 Nov 2020 04:36:34 GMT  
		Size: 76.7 MB (76720719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b6e45f155a7fd6d9f5c08336b6eeb9369ba45e70393ce54e64d0ee8f0d072b`  
		Last Modified: Wed, 25 Nov 2020 04:36:15 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:04bd4da8628ef75e93f2c3089247e8383ee344aa9a295a6215410365e21ce974
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99407805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a227229d51615727239e037d4e1eeeb77b379d034a242c506ff4f54bd528fa53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Wed, 25 Nov 2020 01:57:53 GMT
ENV NODE_VERSION=12.20.0
# Wed, 25 Nov 2020 02:12:30 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="9a25589439ebec4e74fc2652893b5887b33130c0dd7dad2daa1d200024fa676c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       1C050899334244A8AF75E53792EF661D867B9DFA       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 25 Nov 2020 02:12:33 GMT
ENV YARN_VERSION=1.22.5
# Wed, 25 Nov 2020 02:12:40 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 25 Nov 2020 02:12:40 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 25 Nov 2020 02:12:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 02:12:42 GMT
CMD ["node"]
# Wed, 25 Nov 2020 04:32:48 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 25 Nov 2020 04:32:50 GMT
RUN apk add --no-cache 		bash
# Wed, 25 Nov 2020 04:32:51 GMT
ENV NODE_ENV=production
# Wed, 25 Nov 2020 04:32:52 GMT
ENV GHOST_CLI_VERSION=1.15.2
# Wed, 25 Nov 2020 04:33:32 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 25 Nov 2020 04:33:34 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 25 Nov 2020 04:33:35 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 25 Nov 2020 04:33:35 GMT
ENV GHOST_VERSION=3.38.3
# Wed, 25 Nov 2020 04:41:18 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 25 Nov 2020 04:41:24 GMT
WORKDIR /var/lib/ghost
# Wed, 25 Nov 2020 04:41:25 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 25 Nov 2020 04:41:25 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 25 Nov 2020 04:41:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 04:41:27 GMT
EXPOSE 2368
# Wed, 25 Nov 2020 04:41:28 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6608532c31d962fe1b882b06af451da07b673872efd9afb7b7796eb2d578c14d`  
		Last Modified: Wed, 25 Nov 2020 02:29:36 GMT  
		Size: 24.8 MB (24769795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986a61b3dae199ad3cf8a9a72e3f470cac0d19e4280f61bfffcf838199d6e337`  
		Last Modified: Wed, 25 Nov 2020 02:29:28 GMT  
		Size: 2.4 MB (2413220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b735cce3d23b4837a1fb7b0a72f2922439dd1226c1e8f213d085206375f4eb2`  
		Last Modified: Wed, 25 Nov 2020 02:29:27 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be11e04f118e39d8c0a43b6ff30dfa5aebc410794d621decd1593b0241c2b1c2`  
		Last Modified: Wed, 25 Nov 2020 04:41:52 GMT  
		Size: 9.9 KB (9936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418ae885563f889127ecd10852cce96bf5e76aeca8a1fd9049dc7816590eb708`  
		Last Modified: Wed, 25 Nov 2020 04:41:52 GMT  
		Size: 734.1 KB (734051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810b3a1e5bfc53b169ea5882731c1f16ae2e009c54f7cb5907b4d11609171b32`  
		Last Modified: Wed, 25 Nov 2020 04:41:57 GMT  
		Size: 7.5 MB (7456673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0eecaeea42a72f3b34e6b5e328b8b43e28d3cdc161331f967e5cc48ac1d8ac`  
		Last Modified: Wed, 25 Nov 2020 04:42:24 GMT  
		Size: 61.4 MB (61421391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e472a82f5ae595bea7b29c9f999c042d5686dcbc96075dccd21bed1453f783a`  
		Last Modified: Wed, 25 Nov 2020 04:41:52 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:8d1de76088add7ae7ee13ea72c09d5c8be3f1332def86a8fb7f32ae8c20379f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.1 MB (98135060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:718765cab74617dfae47f84d28ca8b3e4c07709dc921fb533c035406ecd97344`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Tue, 17 Nov 2020 01:51:30 GMT
ENV NODE_VERSION=12.19.1
# Tue, 17 Nov 2020 02:02:43 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="eaf8642a5577bb91daf22ce37281d10ac381eee678bc15b0f1501deeb52b84d5"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       1C050899334244A8AF75E53792EF661D867B9DFA       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 17 Nov 2020 02:02:46 GMT
ENV YARN_VERSION=1.22.5
# Tue, 17 Nov 2020 02:02:55 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 17 Nov 2020 02:02:57 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 17 Nov 2020 02:02:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 02:03:01 GMT
CMD ["node"]
# Tue, 17 Nov 2020 02:57:04 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 17 Nov 2020 02:57:06 GMT
RUN apk add --no-cache 		bash
# Tue, 17 Nov 2020 02:57:07 GMT
ENV NODE_ENV=production
# Tue, 17 Nov 2020 02:57:07 GMT
ENV GHOST_CLI_VERSION=1.15.2
# Tue, 17 Nov 2020 02:57:35 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 17 Nov 2020 02:57:37 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 17 Nov 2020 02:57:38 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 24 Nov 2020 00:10:25 GMT
ENV GHOST_VERSION=3.38.3
# Tue, 24 Nov 2020 00:16:04 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 24 Nov 2020 00:16:13 GMT
WORKDIR /var/lib/ghost
# Tue, 24 Nov 2020 00:16:14 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 24 Nov 2020 00:16:15 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 24 Nov 2020 00:16:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:16:18 GMT
EXPOSE 2368
# Tue, 24 Nov 2020 00:16:19 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613859ad7a6109858240d7265f026452b42ae1220bed02b01792aa8fb4abca4`  
		Last Modified: Tue, 17 Nov 2020 02:18:55 GMT  
		Size: 23.9 MB (23911457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e6b058553c38fe81645bb76a12a549c8c3f5c6c903c5c4a6d8f58222c43bbd`  
		Last Modified: Tue, 17 Nov 2020 02:18:46 GMT  
		Size: 2.4 MB (2413045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798907802a028ff88c3dc594de5316e5efcb72912ce43133880c0b797f7ae442`  
		Last Modified: Tue, 17 Nov 2020 02:18:45 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9626c4a7d486067b89a62b01891c2f2aad6cfb371fa9deec2ce3a0ca7a10401`  
		Last Modified: Tue, 17 Nov 2020 03:03:32 GMT  
		Size: 9.7 KB (9683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd5ec3a4b037d30eea321ec699abb84041cde1e611a74e852fa3966ae83faac`  
		Last Modified: Tue, 17 Nov 2020 03:03:31 GMT  
		Size: 671.1 KB (671124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed512ff646178c63c12f001874c5ab46bdfadbeb20a98465f83d8867f10a1b6c`  
		Last Modified: Tue, 17 Nov 2020 03:03:38 GMT  
		Size: 7.5 MB (7463409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e651219b65a245554cf21924ab522efd4be99e096bf70ceaa12cee19af01a1`  
		Last Modified: Tue, 24 Nov 2020 00:18:07 GMT  
		Size: 61.3 MB (61259840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93b9be59515b0215ae77143ef4fde5ac1fec0dfa2f8c45b04648df92cf9e757`  
		Last Modified: Tue, 24 Nov 2020 00:17:37 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:a1d4ed28797a86f6c3d374ee9b0cc71a06097508b3308ecc2fd11080b65cb4f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100451017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aac8879284d89ed6736eef58adfeb3c98ebb1b9f1066687260d5640824610c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Tue, 17 Nov 2020 01:30:18 GMT
ENV NODE_VERSION=12.19.1
# Tue, 17 Nov 2020 01:43:53 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="eaf8642a5577bb91daf22ce37281d10ac381eee678bc15b0f1501deeb52b84d5"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       1C050899334244A8AF75E53792EF661D867B9DFA       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 17 Nov 2020 01:44:01 GMT
ENV YARN_VERSION=1.22.5
# Tue, 17 Nov 2020 01:44:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 17 Nov 2020 01:44:18 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 17 Nov 2020 01:44:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Nov 2020 01:44:26 GMT
CMD ["node"]
# Tue, 17 Nov 2020 02:39:10 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 17 Nov 2020 02:39:13 GMT
RUN apk add --no-cache 		bash
# Tue, 17 Nov 2020 02:39:14 GMT
ENV NODE_ENV=production
# Tue, 17 Nov 2020 02:39:14 GMT
ENV GHOST_CLI_VERSION=1.15.2
# Tue, 17 Nov 2020 02:39:41 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 17 Nov 2020 02:39:47 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 17 Nov 2020 02:39:49 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 24 Nov 2020 00:17:31 GMT
ENV GHOST_VERSION=3.38.3
# Tue, 24 Nov 2020 00:22:44 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				npm_config_python='python3' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 24 Nov 2020 00:22:53 GMT
WORKDIR /var/lib/ghost
# Tue, 24 Nov 2020 00:22:53 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 24 Nov 2020 00:22:54 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 24 Nov 2020 00:22:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:22:56 GMT
EXPOSE 2368
# Tue, 24 Nov 2020 00:22:57 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab60a874c554942a5b1ec0bb46e44d5a17af9fee5aec7f86d65b096a3987ce31`  
		Last Modified: Tue, 17 Nov 2020 02:03:19 GMT  
		Size: 25.1 MB (25066848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cfa79aaef27b8521dba70266be748bd070ab317bd2ea0c122296f0434f566`  
		Last Modified: Tue, 17 Nov 2020 02:03:10 GMT  
		Size: 2.4 MB (2422011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206cc4145cf13e1e813be12812b242622b45e920172a4aba56f7c9b85b78e36b`  
		Last Modified: Tue, 17 Nov 2020 02:03:09 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dee9caf76d8f3a4f3825943f07fb9bf5917a343c53bc8d97a080bd6e3fb08d`  
		Last Modified: Tue, 17 Nov 2020 02:45:35 GMT  
		Size: 10.0 KB (10012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7dc8a6560dbbda0792cb5724ea390e7ba30e3d5d145d2bbc82ab9fd437bbec`  
		Last Modified: Tue, 17 Nov 2020 02:45:35 GMT  
		Size: 791.7 KB (791697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69fc322ca7e7f0bac2ce5c1fa9b7dbc7ed8d8cf5e9e1500dd07dd6f5ed01a1d`  
		Last Modified: Tue, 17 Nov 2020 02:45:39 GMT  
		Size: 7.5 MB (7463411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e279a2a389e8b44565e020b4495936887041e92797cbf3867c687bf4cd153076`  
		Last Modified: Tue, 24 Nov 2020 00:24:27 GMT  
		Size: 62.0 MB (61989658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13d8dbb076e9b670c2173b8e23d05b8059646151fc0d11e6e903252efde0c4e`  
		Last Modified: Tue, 24 Nov 2020 00:24:02 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
