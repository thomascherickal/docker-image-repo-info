## `ghost:alpine`

```console
$ docker pull ghost@sha256:1516aee932ca601120ffb0a5c2f185f49ca1f6cdf9155040a0372095dafce81d
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
$ docker pull ghost@sha256:da0a2a4b088ca9132868bbc8f1e0c42ec0829b6a76709a4b58e08c681d8da679
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112117727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2629fea3f380792e86b92129868f3d6e7919c17263ce9526436887fdcfccc9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 18 Dec 2019 16:31:53 GMT
ENV NODE_VERSION=10.18.0
# Wed, 18 Dec 2019 16:31:57 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="043f9e1c412a391f42a9667373b851590a9a77c08cf6fde6828a3cdb3fb8f316"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 18 Dec 2019 16:31:58 GMT
ENV YARN_VERSION=1.21.1
# Wed, 18 Dec 2019 16:32:00 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 18 Dec 2019 16:32:00 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 18 Dec 2019 16:32:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 16:32:01 GMT
CMD ["node"]
# Wed, 18 Dec 2019 16:58:21 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 18 Dec 2019 16:58:24 GMT
RUN apk add --no-cache 		bash
# Wed, 18 Dec 2019 16:58:24 GMT
ENV NODE_ENV=production
# Wed, 18 Dec 2019 16:58:24 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 18 Dec 2019 16:58:53 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 18 Dec 2019 16:58:54 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 18 Dec 2019 16:58:54 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 19 Dec 2019 03:25:21 GMT
ENV GHOST_VERSION=3.2.0
# Thu, 19 Dec 2019 03:26:28 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(npm view . optionalDependencies.sqlite3)"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 19 Dec 2019 03:26:29 GMT
WORKDIR /var/lib/ghost
# Thu, 19 Dec 2019 03:26:29 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 19 Dec 2019 03:26:29 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 19 Dec 2019 03:26:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 03:26:29 GMT
EXPOSE 2368
# Thu, 19 Dec 2019 03:26:30 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ff64b59cc9440ac59e93503fc6fc303a0d49db3ca7a60e31c8bfdb07396192`  
		Last Modified: Wed, 18 Dec 2019 16:39:04 GMT  
		Size: 22.4 MB (22429829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4251edd6597852afee09f3ef1ce24a14815cd5b9b696300953e4386581cf0298`  
		Last Modified: Wed, 18 Dec 2019 16:39:00 GMT  
		Size: 1.3 MB (1263995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa308999cb81de4ce2ca1db7198b0486c7128a3ad8f0edefaae14a10d8aa9d`  
		Last Modified: Wed, 18 Dec 2019 16:38:59 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b608d3c8d9cc7c51d137a59d0db7ed0e303c1507458f486c1f3cf8fbdea92816`  
		Last Modified: Wed, 18 Dec 2019 17:09:12 GMT  
		Size: 9.6 KB (9628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f613d48acf3938bc03d7b997165731c7e197f311c320017e49d78eb5a80051a3`  
		Last Modified: Wed, 18 Dec 2019 17:09:12 GMT  
		Size: 1.2 MB (1210556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d5cb966491aae5e838559cba2a9ab2bac106e1b25d6776396d9d03e9a66254`  
		Last Modified: Wed, 18 Dec 2019 17:09:17 GMT  
		Size: 6.8 MB (6788346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4acf8158a862a698f7fa208ff5e39ece771ebf1b8d82494568fc425188440b`  
		Last Modified: Thu, 19 Dec 2019 03:33:13 GMT  
		Size: 77.6 MB (77627411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4b5793dca838a5a7fe81ea03a4bae6b1fdae4ac8bceca8be1628cbeed58293`  
		Last Modified: Thu, 19 Dec 2019 03:32:52 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:e78a82d7ea6c0b3154ef3e3f0aae96b237b31bf187fbb72cb19b5b0f61f71177
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101647526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5287cfbc278a9901e692738b84a37d231f9d33a208b2abbc33c40c40d87fd267`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 18 Dec 2019 17:30:08 GMT
ENV NODE_VERSION=10.18.0
# Wed, 18 Dec 2019 17:35:24 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="043f9e1c412a391f42a9667373b851590a9a77c08cf6fde6828a3cdb3fb8f316"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 18 Dec 2019 17:35:27 GMT
ENV YARN_VERSION=1.21.1
# Wed, 18 Dec 2019 17:35:37 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 18 Dec 2019 17:35:37 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 18 Dec 2019 17:35:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 17:35:43 GMT
CMD ["node"]
# Wed, 18 Dec 2019 17:56:56 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 18 Dec 2019 17:57:02 GMT
RUN apk add --no-cache 		bash
# Wed, 18 Dec 2019 17:57:06 GMT
ENV NODE_ENV=production
# Wed, 18 Dec 2019 17:57:09 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 18 Dec 2019 17:57:56 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 18 Dec 2019 17:58:01 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 18 Dec 2019 17:58:02 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 18 Dec 2019 23:58:15 GMT
ENV GHOST_VERSION=3.2.0
# Thu, 19 Dec 2019 00:03:59 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(npm view . optionalDependencies.sqlite3)"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 19 Dec 2019 00:04:05 GMT
WORKDIR /var/lib/ghost
# Thu, 19 Dec 2019 00:04:06 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 19 Dec 2019 00:04:08 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 19 Dec 2019 00:04:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 00:04:14 GMT
EXPOSE 2368
# Thu, 19 Dec 2019 00:04:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a8f7e489f079f6fd089871a4dc68772f1419fcf2646ec377b48b2ca729844`  
		Last Modified: Wed, 18 Dec 2019 17:38:32 GMT  
		Size: 21.6 MB (21615171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5ff4d42fdd657733b3d27a2b6118529578f1b3264c8e89e043ae9223d6bde3`  
		Last Modified: Wed, 18 Dec 2019 17:38:21 GMT  
		Size: 1.3 MB (1327169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e984fd2ecc12ddaef7b9f50af4e9c318e886f4dea3025c0cb51095adb60c352`  
		Last Modified: Wed, 18 Dec 2019 17:38:20 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250409212b9d83c6c70010742edb443b90c0672eaa84e6b71832c86c29e904f5`  
		Last Modified: Wed, 18 Dec 2019 18:17:35 GMT  
		Size: 9.4 KB (9416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9b2551b01551976de62e232eda8e8b8e86679f836cba25a5a26467cdf8f3eb`  
		Last Modified: Wed, 18 Dec 2019 18:17:36 GMT  
		Size: 1.2 MB (1158128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee79cfcb2383520290952bf74771291d263e88d47395dbc79081812fe833e4e6`  
		Last Modified: Wed, 18 Dec 2019 18:17:40 GMT  
		Size: 6.8 MB (6788541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696ba5c066d16bea79317392204c809535119f536624033aa7b9b88d4e450dbf`  
		Last Modified: Thu, 19 Dec 2019 00:17:20 GMT  
		Size: 68.2 MB (68176967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4678242763cd1259c52fcb0d406b97fb6f08b930d70354194b1bc1b779d036a7`  
		Last Modified: Thu, 19 Dec 2019 00:16:48 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:4070061be873f071e501e3a0963c3ebdb78f4dcd085a9849ceecd879d752591b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.2 MB (100178336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9227ab4d63d70f539da06ec63a079a465a86283763d519d936dd74adcea0fbea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 18 Dec 2019 18:08:10 GMT
ENV NODE_VERSION=10.18.0
# Wed, 18 Dec 2019 18:12:43 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="043f9e1c412a391f42a9667373b851590a9a77c08cf6fde6828a3cdb3fb8f316"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 18 Dec 2019 18:12:48 GMT
ENV YARN_VERSION=1.21.1
# Wed, 18 Dec 2019 18:12:53 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 18 Dec 2019 18:12:54 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 18 Dec 2019 18:12:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 18:12:57 GMT
CMD ["node"]
# Wed, 18 Dec 2019 18:45:48 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 18 Dec 2019 18:45:52 GMT
RUN apk add --no-cache 		bash
# Wed, 18 Dec 2019 18:45:54 GMT
ENV NODE_ENV=production
# Wed, 18 Dec 2019 18:45:54 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 18 Dec 2019 18:46:28 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 18 Dec 2019 18:46:34 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 18 Dec 2019 18:46:35 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 19 Dec 2019 01:04:06 GMT
ENV GHOST_VERSION=3.2.0
# Thu, 19 Dec 2019 01:08:49 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(npm view . optionalDependencies.sqlite3)"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 19 Dec 2019 01:08:54 GMT
WORKDIR /var/lib/ghost
# Thu, 19 Dec 2019 01:08:55 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 19 Dec 2019 01:08:57 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 19 Dec 2019 01:08:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 01:08:59 GMT
EXPOSE 2368
# Thu, 19 Dec 2019 01:09:00 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d513bd79f1d4db53d963c048968deccfacb7c47560f96a211d19e08dd92f79a`  
		Last Modified: Wed, 18 Dec 2019 18:24:40 GMT  
		Size: 21.3 MB (21259606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04667baf0e5d8ace3e403167c5a9bb2ea5e8887d4834aa0170667dc7cc005351`  
		Last Modified: Wed, 18 Dec 2019 18:24:33 GMT  
		Size: 1.3 MB (1327156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c559f950c84f5719ee75600ecb8cdd64eab7b15679fccad78642751090c52c06`  
		Last Modified: Wed, 18 Dec 2019 18:24:32 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21947d7ec942303d0c67f0cce376f5c7cb8d2843e56819e9d6af0c5255c527d`  
		Last Modified: Wed, 18 Dec 2019 19:12:16 GMT  
		Size: 9.2 KB (9224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b6560bb2f3d950cfd8c1262cf7ad5088dfa4180292ef2ad048a0a0ef5bca8b`  
		Last Modified: Wed, 18 Dec 2019 19:12:18 GMT  
		Size: 1.1 MB (1092587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7f3192ecbf34e402792412d8b5743efec57fff824cf652c31d0d1189013b8f`  
		Last Modified: Wed, 18 Dec 2019 19:12:24 GMT  
		Size: 6.8 MB (6788617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb89b34f2b1769a8bd9c07dda7d7f08bcbb476daefdd5b2724b3c36a6ab93402`  
		Last Modified: Thu, 19 Dec 2019 01:32:26 GMT  
		Size: 67.3 MB (67321886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54ebaffd8d828653c4d4012c45d541075cc925c4e57a861d73592226a4a4031`  
		Last Modified: Thu, 19 Dec 2019 01:32:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:af85d401b2e70a7e77110fa9d193d3671b547adacb32e6c3e393cf21f9c4e301
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.3 MB (103317258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a09176a6f48a2d2e6576c4c2e67b82cc915cad091c92a9e81613e0842828e23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 18 Dec 2019 17:44:03 GMT
ENV NODE_VERSION=10.18.0
# Wed, 18 Dec 2019 17:50:18 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="043f9e1c412a391f42a9667373b851590a9a77c08cf6fde6828a3cdb3fb8f316"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 18 Dec 2019 17:50:21 GMT
ENV YARN_VERSION=1.21.1
# Wed, 18 Dec 2019 17:50:32 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 18 Dec 2019 17:50:33 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 18 Dec 2019 17:50:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 17:50:36 GMT
CMD ["node"]
# Wed, 18 Dec 2019 18:27:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 18 Dec 2019 18:27:18 GMT
RUN apk add --no-cache 		bash
# Wed, 18 Dec 2019 18:27:18 GMT
ENV NODE_ENV=production
# Wed, 18 Dec 2019 18:27:19 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 18 Dec 2019 18:27:39 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 18 Dec 2019 18:27:42 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 18 Dec 2019 18:27:43 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 19 Dec 2019 01:52:21 GMT
ENV GHOST_VERSION=3.2.0
# Thu, 19 Dec 2019 02:01:11 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(npm view . optionalDependencies.sqlite3)"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 19 Dec 2019 02:01:25 GMT
WORKDIR /var/lib/ghost
# Thu, 19 Dec 2019 02:01:32 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 19 Dec 2019 02:01:34 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 19 Dec 2019 02:01:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 02:01:52 GMT
EXPOSE 2368
# Thu, 19 Dec 2019 02:01:56 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe3a2f4e5d8216e33f83be1ee3cc621c627df822879ce99a65762dc665c5bc4`  
		Last Modified: Wed, 18 Dec 2019 18:03:09 GMT  
		Size: 22.6 MB (22604999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e514f58acd661f958b7a7e748fbd033a7d3d21b2cb11a0fe1599bc93e4f980ef`  
		Last Modified: Wed, 18 Dec 2019 18:02:43 GMT  
		Size: 1.3 MB (1327179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd216ec5248e34b1671e694c9fae169b7d0ce9d32a78e1e5cbd4bd74a271df7`  
		Last Modified: Wed, 18 Dec 2019 18:02:42 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b50e1de4f3dd3299af7c877d61dbc17922ac3e7c0e6ced6e2dfb49b6264582`  
		Last Modified: Wed, 18 Dec 2019 18:52:18 GMT  
		Size: 9.6 KB (9593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2d557a8b7148e8d1760d98512eb44ea4e37be84afdaa15248d22440c5f2538`  
		Last Modified: Wed, 18 Dec 2019 18:52:19 GMT  
		Size: 1.2 MB (1225145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096b31901bbf1ab1e3cfa851fb5df1a3980c38a215298f8858ef4122f70c20bb`  
		Last Modified: Wed, 18 Dec 2019 18:52:19 GMT  
		Size: 6.8 MB (6787734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89971fce1d67806acd4ad12a0d66b2521756152ccfe51df8b1c1db3aff04bd0`  
		Last Modified: Thu, 19 Dec 2019 02:23:46 GMT  
		Size: 68.6 MB (68644001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0338ecf8ebd4084551cc873f8e8549000e8d7dc0c526ebdfaa0daa1a39c56a3`  
		Last Modified: Thu, 19 Dec 2019 02:23:24 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; 386

```console
$ docker pull ghost@sha256:6619dd2738d54d7cd629df041ccb6f4d92b3cb1c79bfb20049f8d7443d6be07c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.4 MB (103403513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:636d28744a5cc4cb85a3fcc9d59b92fe89352210d85a5efb4061f414899d452a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Wed, 18 Dec 2019 19:51:28 GMT
ENV NODE_VERSION=10.18.0
# Wed, 18 Dec 2019 20:19:18 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="043f9e1c412a391f42a9667373b851590a9a77c08cf6fde6828a3cdb3fb8f316"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 18 Dec 2019 20:19:18 GMT
ENV YARN_VERSION=1.21.1
# Wed, 18 Dec 2019 20:19:21 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 18 Dec 2019 20:19:21 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 18 Dec 2019 20:19:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 20:19:21 GMT
CMD ["node"]
# Wed, 18 Dec 2019 20:39:19 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 18 Dec 2019 20:39:21 GMT
RUN apk add --no-cache 		bash
# Wed, 18 Dec 2019 20:39:21 GMT
ENV NODE_ENV=production
# Wed, 18 Dec 2019 20:39:21 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 18 Dec 2019 20:39:37 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 18 Dec 2019 20:39:37 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 18 Dec 2019 20:39:38 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 19 Dec 2019 04:02:31 GMT
ENV GHOST_VERSION=3.2.0
# Thu, 19 Dec 2019 04:07:19 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(npm view . optionalDependencies.sqlite3)"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 19 Dec 2019 04:07:20 GMT
WORKDIR /var/lib/ghost
# Thu, 19 Dec 2019 04:07:20 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 19 Dec 2019 04:07:20 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 19 Dec 2019 04:07:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 04:07:21 GMT
EXPOSE 2368
# Thu, 19 Dec 2019 04:07:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4567cf6d84b7623433f67347038df483ce3de3c472bbc7b2a42609078e28ab05`  
		Last Modified: Wed, 18 Dec 2019 20:23:07 GMT  
		Size: 22.6 MB (22568017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62ebb339e6fdadb786223ca7e3a694c6f6a95b8e6acd97376ebc63c89ed6d4`  
		Last Modified: Wed, 18 Dec 2019 20:23:01 GMT  
		Size: 1.3 MB (1327176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a797ab565b23f566d364e891639323b295e57040d0248b01ea9101fb4da20d`  
		Last Modified: Wed, 18 Dec 2019 20:23:00 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe380f3d9e0dc3df515ccf53cd059b255e7a8a651298153b5f8a086ce6a903b7`  
		Last Modified: Wed, 18 Dec 2019 20:49:35 GMT  
		Size: 9.7 KB (9696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697e9d376f0e714b12fd33790700db955257a520ec34382b02a49081ded5d9a`  
		Last Modified: Wed, 18 Dec 2019 20:49:36 GMT  
		Size: 1.3 MB (1259200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0246d0f541f7fe31f8fd70d4bdaa0a8c40812c5196f58305113358a860e597`  
		Last Modified: Wed, 18 Dec 2019 20:49:39 GMT  
		Size: 6.8 MB (6786983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c3364babf2ac2ef53f4940855b7c7cde48940467993d9de247310e58e6e8ee`  
		Last Modified: Thu, 19 Dec 2019 04:16:26 GMT  
		Size: 68.7 MB (68665676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b42a770d86ed35177ca04672ce7c36d1636287fa20e69839e27e317f2847b2`  
		Last Modified: Thu, 19 Dec 2019 04:16:06 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:b381f71a0af619b64964c061f06f7fbad144e282d32d0db2c1dbbf38e9abfb0d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106922015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49d7d5ca15aeb7b776cfd9d04d807eab50b3cf0c4f8f3f4b67946951cee7d5f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 21 Oct 2019 17:52:55 GMT
ADD file:11a2dd0058b1642e9ee52239d03223819a53ca346fd42826eead7729c50e1257 in / 
# Mon, 21 Oct 2019 17:53:00 GMT
CMD ["/bin/sh"]
# Wed, 18 Dec 2019 19:00:55 GMT
ENV NODE_VERSION=10.18.0
# Wed, 18 Dec 2019 19:12:21 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="043f9e1c412a391f42a9667373b851590a9a77c08cf6fde6828a3cdb3fb8f316"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 18 Dec 2019 19:12:27 GMT
ENV YARN_VERSION=1.21.1
# Wed, 18 Dec 2019 19:12:37 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 18 Dec 2019 19:12:39 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 18 Dec 2019 19:12:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 19:12:45 GMT
CMD ["node"]
# Wed, 18 Dec 2019 20:06:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 18 Dec 2019 20:07:07 GMT
RUN apk add --no-cache 		bash
# Wed, 18 Dec 2019 20:07:10 GMT
ENV NODE_ENV=production
# Wed, 18 Dec 2019 20:07:13 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 18 Dec 2019 20:07:47 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 18 Dec 2019 20:07:52 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 18 Dec 2019 20:07:55 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 19 Dec 2019 02:26:23 GMT
ENV GHOST_VERSION=3.2.0
# Thu, 19 Dec 2019 02:30:19 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(npm view . optionalDependencies.sqlite3)"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 19 Dec 2019 02:30:26 GMT
WORKDIR /var/lib/ghost
# Thu, 19 Dec 2019 02:30:29 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 19 Dec 2019 02:30:30 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 19 Dec 2019 02:30:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 02:30:35 GMT
EXPOSE 2368
# Thu, 19 Dec 2019 02:30:37 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cd18d16ea896a0f0eb99be52a9722ffae9a5ac35cf28cb8b96f589352f8e71d6`  
		Last Modified: Mon, 21 Oct 2019 17:53:53 GMT  
		Size: 2.8 MB (2808504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e98a4a2dcaa94e03c52b865aa7581dd1c35ec116ecbddd47b33e301c0de1aa`  
		Last Modified: Wed, 18 Dec 2019 19:33:40 GMT  
		Size: 24.3 MB (24347604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeb7e8bb439d7c8cb125f3857b8de563055da0d1e363cbb61442997c29cd14e`  
		Last Modified: Wed, 18 Dec 2019 19:33:31 GMT  
		Size: 1.3 MB (1327146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5192012ffadfd10f819cc7cf28bd11e2a3050cfdb2b15b463e900870016732`  
		Last Modified: Wed, 18 Dec 2019 19:33:31 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47acea8a79ff1d2533a6747f352a0e99600360bc9d9590ba0bc54265875ff0c8`  
		Last Modified: Wed, 18 Dec 2019 20:42:53 GMT  
		Size: 10.2 KB (10175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc9f7b733e23242c4955a62d872169cc395c0733b22f0cde0d02c099ed614b2`  
		Last Modified: Wed, 18 Dec 2019 20:42:59 GMT  
		Size: 1.3 MB (1297128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d757f5ff4c7788ff2f5233418a695422074f43da8b8b0b5bc9cb622ab8004768`  
		Last Modified: Wed, 18 Dec 2019 20:43:15 GMT  
		Size: 6.8 MB (6788409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08b8afd5e0b229c13a2346e15cb6e20e0d73112582e78dbe7766091e72b3935`  
		Last Modified: Thu, 19 Dec 2019 02:59:14 GMT  
		Size: 70.3 MB (70342227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e5f3f4cda8313cbd11e57479a03f182c5cb372715265d98c1524f69b14afc`  
		Last Modified: Thu, 19 Dec 2019 02:58:21 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; s390x

```console
$ docker pull ghost@sha256:6853c457ee6f4de77ed94ec5c768087116d3366cf76e86cced3cee1ed637fdf8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102780047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76b022e0989678807e2b350325b1d1513a01a8b3f528e902ee15fea1d94806ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 21 Oct 2019 16:47:28 GMT
ADD file:49020543846e4f93b34d71c0e4234ade7bd6dde3f45cb73784aa73ce0522c8bc in / 
# Mon, 21 Oct 2019 16:47:29 GMT
CMD ["/bin/sh"]
# Wed, 18 Dec 2019 18:01:13 GMT
ENV NODE_VERSION=10.18.0
# Wed, 18 Dec 2019 18:15:03 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="043f9e1c412a391f42a9667373b851590a9a77c08cf6fde6828a3cdb3fb8f316"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps
# Wed, 18 Dec 2019 18:15:03 GMT
ENV YARN_VERSION=1.21.1
# Wed, 18 Dec 2019 18:15:05 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn
# Wed, 18 Dec 2019 18:15:05 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 18 Dec 2019 18:15:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Dec 2019 18:15:06 GMT
CMD ["node"]
# Wed, 18 Dec 2019 18:39:31 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 18 Dec 2019 18:39:32 GMT
RUN apk add --no-cache 		bash
# Wed, 18 Dec 2019 18:39:33 GMT
ENV NODE_ENV=production
# Wed, 18 Dec 2019 18:39:33 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 18 Dec 2019 18:39:45 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 18 Dec 2019 18:39:47 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 18 Dec 2019 18:39:47 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 19 Dec 2019 00:43:09 GMT
ENV GHOST_VERSION=3.2.0
# Thu, 19 Dec 2019 00:44:44 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(npm view . optionalDependencies.sqlite3)"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 19 Dec 2019 00:44:45 GMT
WORKDIR /var/lib/ghost
# Thu, 19 Dec 2019 00:44:45 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 19 Dec 2019 00:44:46 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 19 Dec 2019 00:44:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 00:44:46 GMT
EXPOSE 2368
# Thu, 19 Dec 2019 00:44:46 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:fb7172052a60e640810f01efff381654bf9ed44082461455cfcc6306d192d541`  
		Last Modified: Mon, 21 Oct 2019 16:48:40 GMT  
		Size: 2.6 MB (2573587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486cb3f3dc921608c4caa80daf4f64d5d9278d597ae6e0b1ad9e20e361bce85b`  
		Last Modified: Wed, 18 Dec 2019 18:21:18 GMT  
		Size: 22.4 MB (22374684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cbbb0885d6ef462455d5c65b0b442936a1390a0358d97ba80ae927b5e0153f`  
		Last Modified: Wed, 18 Dec 2019 18:21:15 GMT  
		Size: 1.3 MB (1327149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3283987b6c6594af58ac54d83b6f9dce6fbac66c7044234984d417578ba2ea9`  
		Last Modified: Wed, 18 Dec 2019 18:21:14 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b805d614ee28b85de65f8cb210948b3cd1dadfe54863c7037038544261303f2e`  
		Last Modified: Wed, 18 Dec 2019 18:50:49 GMT  
		Size: 9.7 KB (9723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c637e0a2f0ffafe32277a596f7916569989da0527011a8c7e7c704493a9c5b`  
		Last Modified: Wed, 18 Dec 2019 18:50:49 GMT  
		Size: 1.2 MB (1245121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4a3b55e1ff4043a217a8d1a5ddf7b7dd3ef63c72ef77cc78ad0b12dc76633c`  
		Last Modified: Wed, 18 Dec 2019 18:50:51 GMT  
		Size: 6.8 MB (6786481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dacf7cc964338ccc9af6db100f9b844f6f68551945282af67254de2e1592a2`  
		Last Modified: Thu, 19 Dec 2019 00:55:25 GMT  
		Size: 68.5 MB (68462479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8e71e9fc74854cfa86a31b0a58d29cc9a06a291770bfc09092318e03263d62`  
		Last Modified: Thu, 19 Dec 2019 00:55:16 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
