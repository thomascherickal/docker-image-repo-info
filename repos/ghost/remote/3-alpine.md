## `ghost:3-alpine`

```console
$ docker pull ghost@sha256:e710de0b97f5d03e31b3d269328d6a19027930071e40945b6d2c1d56ae0f98dd
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
$ docker pull ghost@sha256:966c6857977bbdfd23cb0ebf139e16927f091d45d9af5dd6e6205981c1b9342e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.0 MB (117979921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e62dcee248afa6682943991f6ce2550331e6962b744cd34d0b0c6cc62e163ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:56:32 GMT
ENV NODE_VERSION=12.16.1
# Mon, 23 Mar 2020 22:56:37 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="7606d86e842b710e4321fe1c7f7a32a8e145f5e0659de406399cda5a37411d92"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Mon, 23 Mar 2020 22:56:37 GMT
ENV YARN_VERSION=1.22.0
# Mon, 23 Mar 2020 22:56:40 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Mon, 23 Mar 2020 22:56:40 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Mon, 23 Mar 2020 22:56:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 22:56:40 GMT
CMD ["node"]
# Tue, 24 Mar 2020 04:11:46 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 24 Mar 2020 04:11:48 GMT
RUN apk add --no-cache 		bash
# Tue, 24 Mar 2020 04:11:48 GMT
ENV NODE_ENV=production
# Tue, 24 Mar 2020 04:11:48 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Tue, 24 Mar 2020 04:12:13 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 24 Mar 2020 04:12:14 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 24 Mar 2020 04:12:14 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 09 Apr 2020 00:20:43 GMT
ENV GHOST_VERSION=3.13.1
# Thu, 09 Apr 2020 00:21:40 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 09 Apr 2020 00:21:40 GMT
WORKDIR /var/lib/ghost
# Thu, 09 Apr 2020 00:21:40 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 09 Apr 2020 00:21:41 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 09 Apr 2020 00:21:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Apr 2020 00:21:41 GMT
EXPOSE 2368
# Thu, 09 Apr 2020 00:21:41 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd41271d385d2b7237c0dc7529efec09c24b814210f63ed880556227dc5f48a`  
		Last Modified: Mon, 23 Mar 2020 23:00:41 GMT  
		Size: 24.5 MB (24481434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd731a7214510cbae667108943d0e07b96c7beb3a3ade18bd756445b2b79a209`  
		Last Modified: Mon, 23 Mar 2020 23:00:33 GMT  
		Size: 2.2 MB (2238680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495807fcdd3718329576cee98e15dc29b9fd68fb864a89c4f415d7ba011b9ffb`  
		Last Modified: Mon, 23 Mar 2020 23:00:32 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646ef71e27691d80a96dacc1334f33a7b5f4c66d6301e63579ee63edf5ea1d7a`  
		Last Modified: Tue, 24 Mar 2020 04:17:43 GMT  
		Size: 9.9 KB (9906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b98b913546642772383288939202d33a9bd4bd876774f1374d48b3cb89ebebe`  
		Last Modified: Tue, 24 Mar 2020 04:17:43 GMT  
		Size: 780.5 KB (780523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fdd7a70519c4905f8f7177d9bf4057dffed8681f6392e4051ee896c147f9da`  
		Last Modified: Tue, 24 Mar 2020 04:17:47 GMT  
		Size: 6.8 MB (6791357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e8ce2b2c1f098c25f65feea50802e3212159b1d2d1505089d6e1c547db884a`  
		Last Modified: Thu, 09 Apr 2020 00:25:07 GMT  
		Size: 80.9 MB (80873934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87c1b81e7c58507aa0bc081187578d42cd9447ec2e3b5bdf6091720ab1a9666`  
		Last Modified: Thu, 09 Apr 2020 00:24:39 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:798b0fb4c452b4b9e86dbd2041308c22e29568a7086114c32a38813131f0a9e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108331570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffde4f5f4300d504150c8d0112174ed6ad64c1adef2b2f7b0790a821b370b4be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:05:38 GMT
ENV NODE_VERSION=12.16.1
# Tue, 24 Mar 2020 00:17:52 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="7606d86e842b710e4321fe1c7f7a32a8e145f5e0659de406399cda5a37411d92"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 24 Mar 2020 00:17:54 GMT
ENV YARN_VERSION=1.22.0
# Tue, 24 Mar 2020 00:18:01 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 24 Mar 2020 00:18:02 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:18:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 00:18:04 GMT
CMD ["node"]
# Tue, 24 Mar 2020 03:48:37 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 24 Mar 2020 03:48:41 GMT
RUN apk add --no-cache 		bash
# Tue, 24 Mar 2020 03:48:41 GMT
ENV NODE_ENV=production
# Tue, 24 Mar 2020 03:48:42 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Tue, 24 Mar 2020 03:49:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 24 Mar 2020 03:49:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 24 Mar 2020 03:49:30 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 08 Apr 2020 23:49:26 GMT
ENV GHOST_VERSION=3.13.1
# Wed, 08 Apr 2020 23:55:53 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 08 Apr 2020 23:56:01 GMT
WORKDIR /var/lib/ghost
# Wed, 08 Apr 2020 23:56:01 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 08 Apr 2020 23:56:02 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 08 Apr 2020 23:56:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Apr 2020 23:56:03 GMT
EXPOSE 2368
# Wed, 08 Apr 2020 23:56:04 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b960f9ebb83029c8e9fb3689bd4aac92cdd6bd03ad745bf33999052d16dff07`  
		Last Modified: Tue, 24 Mar 2020 00:27:12 GMT  
		Size: 23.9 MB (23933195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004e42e6ed8495795b74aea40ea4ee887778c2101a310c124894325a6d2188db`  
		Last Modified: Tue, 24 Mar 2020 00:27:01 GMT  
		Size: 2.3 MB (2294376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6619b0e8f04857b54d8beea55aefc427b2d2a592f2f430bfcebfddbd28b345bf`  
		Last Modified: Tue, 24 Mar 2020 00:27:00 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7b8896d90e2c95b529bb259ba8edaddb658e1be9d1b3c8ba7beef36722f0d0`  
		Last Modified: Tue, 24 Mar 2020 04:14:48 GMT  
		Size: 9.7 KB (9730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d259a27b709805a62fc14e25bc3402fdb6da11ae4580c07290c5db4f00374e8`  
		Last Modified: Tue, 24 Mar 2020 04:14:48 GMT  
		Size: 733.4 KB (733443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7744a72adb6a9842513c74b0bcf27f16892581073cbeaf1ff58a743158bc3c59`  
		Last Modified: Tue, 24 Mar 2020 04:14:53 GMT  
		Size: 6.8 MB (6791439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d513805460739e4c91d5bdb7bece4b0ca6d04e2b4404f39c4a80d4aee892d2bf`  
		Last Modified: Thu, 09 Apr 2020 00:03:04 GMT  
		Size: 71.9 MB (71949981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0891b88d849e23ed32198f1fd937551e59c5fae56211a3302055d3ca3e5d728`  
		Last Modified: Thu, 09 Apr 2020 00:02:37 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:327adb4dc57b27e2545c811eb8a14f13fb66dc52e5e2d806161c9c69ac06e295
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106699337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85312e8a6106396294b1bdbf461c203c0e5046fd59caf75f659eaf5bf1ea0b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:12:45 GMT
ENV NODE_VERSION=12.16.1
# Mon, 23 Mar 2020 23:21:37 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="7606d86e842b710e4321fe1c7f7a32a8e145f5e0659de406399cda5a37411d92"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Mon, 23 Mar 2020 23:21:40 GMT
ENV YARN_VERSION=1.22.0
# Mon, 23 Mar 2020 23:21:44 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Mon, 23 Mar 2020 23:21:45 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:21:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:21:46 GMT
CMD ["node"]
# Tue, 24 Mar 2020 02:18:22 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 24 Mar 2020 02:18:31 GMT
RUN apk add --no-cache 		bash
# Tue, 24 Mar 2020 02:18:33 GMT
ENV NODE_ENV=production
# Tue, 24 Mar 2020 02:18:35 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Tue, 24 Mar 2020 02:19:11 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 24 Mar 2020 02:19:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 24 Mar 2020 02:19:13 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 09 Apr 2020 00:03:03 GMT
ENV GHOST_VERSION=3.13.1
# Thu, 09 Apr 2020 00:07:34 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 09 Apr 2020 00:07:39 GMT
WORKDIR /var/lib/ghost
# Thu, 09 Apr 2020 00:07:39 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 09 Apr 2020 00:07:40 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 09 Apr 2020 00:07:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Apr 2020 00:07:41 GMT
EXPOSE 2368
# Thu, 09 Apr 2020 00:07:42 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f462b27032291962f65896d2d56a038c7d192675f532e6dc83c7b58759232c`  
		Last Modified: Mon, 23 Mar 2020 23:29:46 GMT  
		Size: 23.5 MB (23496708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67d7062b0aff379ef5ca55dc9d75a26d50a5eab6ca102a147daad2cefdc818b`  
		Last Modified: Mon, 23 Mar 2020 23:29:38 GMT  
		Size: 2.3 MB (2294324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374b2e5695f35a3e6c5cc6de0ac12fda523f323705a63c2fe18f88b2e565c116`  
		Last Modified: Mon, 23 Mar 2020 23:29:38 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ca30da3b7045ce68d6f90338d928bb2905ddaf25494ca65922556869e72b8b`  
		Last Modified: Tue, 24 Mar 2020 02:34:12 GMT  
		Size: 9.5 KB (9514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2be70874728d68733693ba854e8455d32673c7e33bf76a9dc7b6f7a7410c94`  
		Last Modified: Tue, 24 Mar 2020 02:34:11 GMT  
		Size: 669.0 KB (669020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a37850d4084b74693e507a7d357212dd037af506fe577e4d5191dd66e32774`  
		Last Modified: Tue, 24 Mar 2020 02:34:13 GMT  
		Size: 6.8 MB (6791286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bef0b45eb9d0f334a44d4cdafd170335453a86fb189056996bd041929c90ecf`  
		Last Modified: Thu, 09 Apr 2020 00:17:45 GMT  
		Size: 71.0 MB (71017164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57371e8db9842d6b33c8747eb5b4e4eb04ec08a98ede86360ae1c5224ffafe08`  
		Last Modified: Thu, 09 Apr 2020 00:17:20 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:32a7f30f456ad6231dea155bc2bb6c3e7b3bb9fb97559f56cd2af0062c162530
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109527200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ed6eff836b55a25bdeaf6f184eb9ef01f788f3b5b5243f6650d4ec3f4659268`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:04:00 GMT
ENV NODE_VERSION=12.16.1
# Tue, 24 Mar 2020 00:15:29 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="7606d86e842b710e4321fe1c7f7a32a8e145f5e0659de406399cda5a37411d92"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 24 Mar 2020 00:15:30 GMT
ENV YARN_VERSION=1.22.0
# Tue, 24 Mar 2020 00:15:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 24 Mar 2020 00:15:35 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:15:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 00:15:36 GMT
CMD ["node"]
# Tue, 24 Mar 2020 06:11:07 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 24 Mar 2020 06:11:09 GMT
RUN apk add --no-cache 		bash
# Tue, 24 Mar 2020 06:11:09 GMT
ENV NODE_ENV=production
# Tue, 24 Mar 2020 06:11:10 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Tue, 24 Mar 2020 06:11:34 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 24 Mar 2020 06:11:36 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 24 Mar 2020 06:11:37 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 08 Apr 2020 23:44:49 GMT
ENV GHOST_VERSION=3.13.1
# Wed, 08 Apr 2020 23:49:23 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 08 Apr 2020 23:49:32 GMT
WORKDIR /var/lib/ghost
# Wed, 08 Apr 2020 23:49:33 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 08 Apr 2020 23:49:34 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 08 Apr 2020 23:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Apr 2020 23:49:36 GMT
EXPOSE 2368
# Wed, 08 Apr 2020 23:49:37 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae83d6cf561de522630ffbd8a33786609687a3214a91921074853052083e81b`  
		Last Modified: Tue, 24 Mar 2020 00:25:22 GMT  
		Size: 24.7 MB (24664754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628a2d4ecfce483b5a53f3d29ef73910447f3f623afafa8bb2c060f4dc105888`  
		Last Modified: Tue, 24 Mar 2020 00:25:15 GMT  
		Size: 2.3 MB (2302059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e22b9da614c080eb77945d19e5b1702635adc51ec7aee19e8c3745d40aa88`  
		Last Modified: Tue, 24 Mar 2020 00:25:14 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434031c56b4d28a4c7260a3b3ca197b82f94b0a09d9266db3715f27c52d3b82f`  
		Last Modified: Tue, 24 Mar 2020 06:26:14 GMT  
		Size: 9.8 KB (9844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22c032740a3274e0b68e7b233ca956ffdd0fc57f40eda4308fc982d7e7c39ee`  
		Last Modified: Tue, 24 Mar 2020 06:26:14 GMT  
		Size: 792.1 KB (792139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed95e8544f2eb848ea463f1a89a3ec3425a72e5502be946056db89accd8c1ce`  
		Last Modified: Tue, 24 Mar 2020 06:26:18 GMT  
		Size: 6.8 MB (6791251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6d2c4159e4bce8f00b9a17b8a39029a0a43aac2e7167dfa827f0e0220094ec`  
		Last Modified: Wed, 08 Apr 2020 23:59:43 GMT  
		Size: 72.2 MB (72243185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9feaa9b4a97ec9cb797707203d2ffbb9d63a013619c526d45cbc4da8f17cce`  
		Last Modified: Wed, 08 Apr 2020 23:59:18 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; 386

```console
$ docker pull ghost@sha256:93939e8cd92dda61d4a41b0c977b947e22d50e9c556e312f65b3795abbfde74c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (109952428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015cf576019e106245304d64416b3d0bcbfdc28e17d361d6e514ecd41b6d8352`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 23 Mar 2020 21:38:28 GMT
ADD file:99c8234abafd4fa915c0b826eb0e3be0e6aaa7c1e33cb1214ef71a99e9c02e06 in / 
# Mon, 23 Mar 2020 21:38:28 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:56:35 GMT
ENV NODE_VERSION=12.16.1
# Mon, 23 Mar 2020 23:48:21 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="7606d86e842b710e4321fe1c7f7a32a8e145f5e0659de406399cda5a37411d92"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Mon, 23 Mar 2020 23:48:21 GMT
ENV YARN_VERSION=1.22.0
# Mon, 23 Mar 2020 23:48:24 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Mon, 23 Mar 2020 23:48:25 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:48:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:48:25 GMT
CMD ["node"]
# Tue, 24 Mar 2020 05:53:33 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 24 Mar 2020 05:53:34 GMT
RUN apk add --no-cache 		bash
# Tue, 24 Mar 2020 05:53:34 GMT
ENV NODE_ENV=production
# Tue, 24 Mar 2020 05:53:35 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Tue, 24 Mar 2020 05:53:53 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 24 Mar 2020 05:53:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 24 Mar 2020 05:53:54 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 08 Apr 2020 23:50:39 GMT
ENV GHOST_VERSION=3.13.1
# Wed, 08 Apr 2020 23:53:38 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 08 Apr 2020 23:53:39 GMT
WORKDIR /var/lib/ghost
# Wed, 08 Apr 2020 23:53:39 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 08 Apr 2020 23:53:40 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 08 Apr 2020 23:53:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Apr 2020 23:53:40 GMT
EXPOSE 2368
# Wed, 08 Apr 2020 23:53:40 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:43f6a4398e1c9e860dfb5c93d7049ab9eedf814513bd6d07e06077c560303c7a`  
		Last Modified: Mon, 23 Mar 2020 21:38:48 GMT  
		Size: 2.8 MB (2806122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcb303c7a458ddb7fb13f8c8f33c8de75c45104187bc5eae5b4c87a3245ab8d`  
		Last Modified: Tue, 24 Mar 2020 00:35:36 GMT  
		Size: 24.8 MB (24805465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07310f5a3d021d435b78a77e2a78c5db6a03772ff6ea613b6872407a9c41bf9`  
		Last Modified: Tue, 24 Mar 2020 00:35:30 GMT  
		Size: 2.3 MB (2294219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea20132dcfb099691cd776af92a4a7502619eca84026a94c9e685786d54cd27`  
		Last Modified: Tue, 24 Mar 2020 00:35:29 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086a41a4c0a4a70c088c01be3b957a594c37fa56cabf1ba1a38ec72898644bcf`  
		Last Modified: Tue, 24 Mar 2020 06:06:52 GMT  
		Size: 10.0 KB (9985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4120e464a58540938d5fb23662b7327769e5b927c302456fbcaa0383773faa`  
		Last Modified: Tue, 24 Mar 2020 06:06:52 GMT  
		Size: 831.1 KB (831111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c1a240523e49778caae076a5c9fd6a7280a7cea22c1d032958a5b97be7a3ea`  
		Last Modified: Tue, 24 Mar 2020 06:06:56 GMT  
		Size: 6.8 MB (6791160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3fcf643a7c0d535fd3034ef8e87be571b5c3846f9095929f41f536cfc38025`  
		Last Modified: Thu, 09 Apr 2020 00:04:02 GMT  
		Size: 72.4 MB (72413536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9e902b825aad3f650cf8f5e06ba86f36c8e7f763c1fe1c50073b4541981a71`  
		Last Modified: Thu, 09 Apr 2020 00:03:41 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:97ad04fb2983a4d09770cc6d6459cb7d091a952bc3a7631522bb00836b853744
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.9 MB (112905316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:952ff372f18ff3d8ded5d747f121ded96e41387d1399e57b2acd302da3a4276f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 22:56:36 GMT
ENV NODE_VERSION=12.16.1
# Mon, 23 Mar 2020 23:13:24 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="7606d86e842b710e4321fe1c7f7a32a8e145f5e0659de406399cda5a37411d92"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Mon, 23 Mar 2020 23:13:32 GMT
ENV YARN_VERSION=1.22.0
# Mon, 23 Mar 2020 23:13:42 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Mon, 23 Mar 2020 23:13:44 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Mon, 23 Mar 2020 23:13:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Mar 2020 23:13:54 GMT
CMD ["node"]
# Tue, 24 Mar 2020 03:05:10 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 24 Mar 2020 03:05:18 GMT
RUN apk add --no-cache 		bash
# Tue, 24 Mar 2020 03:05:21 GMT
ENV NODE_ENV=production
# Tue, 24 Mar 2020 03:05:24 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Tue, 24 Mar 2020 03:06:09 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 24 Mar 2020 03:06:14 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 24 Mar 2020 03:06:16 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 31 Mar 2020 00:25:16 GMT
ENV GHOST_VERSION=3.12.1
# Tue, 31 Mar 2020 00:29:37 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 31 Mar 2020 00:29:44 GMT
WORKDIR /var/lib/ghost
# Tue, 31 Mar 2020 00:29:48 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 31 Mar 2020 00:29:49 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 31 Mar 2020 00:29:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 00:29:57 GMT
EXPOSE 2368
# Tue, 31 Mar 2020 00:30:01 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66001588e98b68c12a2b67a7ed4dea9b64b26bd6c45a61b4c55697ec95eda60e`  
		Last Modified: Mon, 23 Mar 2020 23:29:10 GMT  
		Size: 26.8 MB (26798233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478ad4c3eca91fd3e18b0e69d4905136d020f72d2570684339ec498e4339f6cf`  
		Last Modified: Mon, 23 Mar 2020 23:29:04 GMT  
		Size: 2.3 MB (2301835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7de88bef8d697c5008b0f57c58cbbb330419f3b8c67f8e194e75fa239b02a79`  
		Last Modified: Mon, 23 Mar 2020 23:29:03 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685de773e4568e304b393e111839a76827a857f9a03d99e29f4c7247c1ccac7e`  
		Last Modified: Tue, 24 Mar 2020 03:23:51 GMT  
		Size: 10.4 KB (10394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307d5bb5cf2f6b29c8cfa4af2d36b1f2060dd3b8c53b45c578ce8fe57d7a87d8`  
		Last Modified: Tue, 24 Mar 2020 03:23:51 GMT  
		Size: 862.6 KB (862600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d68b7673719473cb58ffbd0d962c295a5e09496810ae8ad990bad3265694b87b`  
		Last Modified: Tue, 24 Mar 2020 03:24:07 GMT  
		Size: 6.8 MB (6791295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c9c0562c00297337596067697da3aea7513fe27c50e1249084b36b76559e80`  
		Last Modified: Tue, 31 Mar 2020 00:31:54 GMT  
		Size: 73.3 MB (73320080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21196d5ad85a0f22c23860293b5244744310f67feccbb6096ac98e15be0f73ba`  
		Last Modified: Tue, 31 Mar 2020 00:31:38 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:19112fa7fa0ec64e51da21bbde009511d091af5b499deb3f32a2c1b6e1e1f52d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.1 MB (109118837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1faa0290be8c34b4f4e05ffabfa550780cc8ac0e4bf47da523cd39348b88f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 23 Mar 2020 21:41:34 GMT
ADD file:b6d4ad8fd0ec7f66e6d54b8cd8937ba7821b44096806af78692b4cab6d087a9c in / 
# Mon, 23 Mar 2020 21:41:34 GMT
CMD ["/bin/sh"]
# Mon, 23 Mar 2020 23:49:02 GMT
ENV NODE_VERSION=12.16.1
# Tue, 24 Mar 2020 00:06:29 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="7606d86e842b710e4321fe1c7f7a32a8e145f5e0659de406399cda5a37411d92"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 24 Mar 2020 00:06:31 GMT
ENV YARN_VERSION=1.22.0
# Tue, 24 Mar 2020 00:06:33 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 24 Mar 2020 00:06:34 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:06:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 00:06:34 GMT
CMD ["node"]
# Tue, 24 Mar 2020 02:00:50 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 24 Mar 2020 02:00:51 GMT
RUN apk add --no-cache 		bash
# Tue, 24 Mar 2020 02:00:51 GMT
ENV NODE_ENV=production
# Tue, 24 Mar 2020 02:00:51 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Tue, 24 Mar 2020 02:01:05 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 24 Mar 2020 02:01:06 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 24 Mar 2020 02:01:06 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 08 Apr 2020 23:14:13 GMT
ENV GHOST_VERSION=3.13.1
# Wed, 08 Apr 2020 23:16:02 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 08 Apr 2020 23:16:07 GMT
WORKDIR /var/lib/ghost
# Wed, 08 Apr 2020 23:16:07 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 08 Apr 2020 23:16:07 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 08 Apr 2020 23:16:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Apr 2020 23:16:08 GMT
EXPOSE 2368
# Wed, 08 Apr 2020 23:16:08 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:ca1c6795bfb97df28a926fd646127ba4944b69beb1cea7b00d62787b8b3c0108`  
		Last Modified: Mon, 23 Mar 2020 21:41:56 GMT  
		Size: 2.6 MB (2582073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f08b531d31e8ba334976893a531e9a6c0b35e2b3ae4daa26fe10f0cc5281a0`  
		Last Modified: Tue, 24 Mar 2020 00:19:15 GMT  
		Size: 24.6 MB (24569650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556fe4a382c614f903360decdf2f447d071b3fbe3e5f19c728ef64704d05f92c`  
		Last Modified: Tue, 24 Mar 2020 00:19:11 GMT  
		Size: 2.3 MB (2304127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165836b35ce11f2f6462597ed45ecaf44f3692af44aaca5e965b1e390cd9cbd3`  
		Last Modified: Tue, 24 Mar 2020 00:19:16 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6468ae00e258d0ea57eb2e5215db0423f3ead42c174477fb520d55aa225cb4`  
		Last Modified: Tue, 24 Mar 2020 02:09:27 GMT  
		Size: 10.0 KB (9978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e31bb04c3f04c627d05863508e1cf9b7773e508674dd1ad242835966f269890`  
		Last Modified: Tue, 24 Mar 2020 02:09:33 GMT  
		Size: 813.9 KB (813869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00d21f979d24bd990a0d15ce105125eb54f633ca014d413646e673293b5d168`  
		Last Modified: Tue, 24 Mar 2020 02:09:29 GMT  
		Size: 6.8 MB (6790953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb93e4adcc6bb691a30d978c7a1b6675c5e3e4e3d9fd3332fcb300419131294f`  
		Last Modified: Wed, 08 Apr 2020 23:25:58 GMT  
		Size: 72.0 MB (72047361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a712e877c07e9231305e63f098a5b55f4d787a9958db0cb811a3161d37a6cc6`  
		Last Modified: Wed, 08 Apr 2020 23:26:01 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
