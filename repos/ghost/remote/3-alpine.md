## `ghost:3-alpine`

```console
$ docker pull ghost@sha256:13541a6dcbad4dd5e67ab98cb0f945245f3ca1f093b050ec890a80d55524f9f8
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
$ docker pull ghost@sha256:d04fc5bcc6f9152951d3d850dae0f7bbf0795d3febf62f9f1459060be196b17a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106074599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55eea437b430234d4ecaf2bf912c32639418b33c515891133521db3bd7fdf30b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 02:28:07 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 02:28:12 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 02:28:13 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 02:28:17 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 02:28:17 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 02:28:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 02:28:17 GMT
CMD ["node"]
# Wed, 29 Apr 2020 04:34:02 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 04:34:04 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 04:34:04 GMT
ENV NODE_ENV=production
# Wed, 29 Apr 2020 04:34:05 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 29 Apr 2020 04:34:35 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Apr 2020 04:34:36 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Apr 2020 04:34:36 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 07 May 2020 15:20:40 GMT
ENV GHOST_VERSION=3.15.0
# Thu, 07 May 2020 15:21:35 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 07 May 2020 15:21:36 GMT
WORKDIR /var/lib/ghost
# Thu, 07 May 2020 15:21:36 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 07 May 2020 15:21:36 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 07 May 2020 15:21:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 15:21:37 GMT
EXPOSE 2368
# Thu, 07 May 2020 15:21:37 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3938f7d3bdaad20ea7fff408083bb1f14a4e5662ef39cc3c4729b6949aa5b4`  
		Last Modified: Wed, 29 Apr 2020 02:31:09 GMT  
		Size: 24.6 MB (24624708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3c12f5dc1029a72c23cec6f3fe541ca5f33bdd1aa8f3c2909191819d212c30`  
		Last Modified: Wed, 29 Apr 2020 02:31:05 GMT  
		Size: 2.2 MB (2239235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0cb7a9eeee13492aa5ac241e25e87e86317b49ef8fe9fa89019ec1460aa9b3`  
		Last Modified: Wed, 29 Apr 2020 02:31:05 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08533764f382593abfb931046d99c3e6a692979c8a559351a11021cd1b27d683`  
		Last Modified: Wed, 29 Apr 2020 04:37:29 GMT  
		Size: 9.9 KB (9907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d93d179246dfbc75556b65c479f91ed8c480f42386ecbacd63303b7f3eae74`  
		Last Modified: Wed, 29 Apr 2020 04:37:29 GMT  
		Size: 779.3 KB (779318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2cb768d1a708a187b3388c42b02c46979049c894ec052c0eecabf4a8338110`  
		Last Modified: Wed, 29 Apr 2020 04:37:35 GMT  
		Size: 6.8 MB (6769286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58744fc55bfde9574af2b7bb79475d22c1e245ee832e15396093a27d8c5d7ec`  
		Last Modified: Thu, 07 May 2020 15:22:29 GMT  
		Size: 68.8 MB (68837998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e337d9263645ce2ceaf3b96548d65c86906c93bf48f2cb1daf45a37fa8e6300f`  
		Last Modified: Thu, 07 May 2020 15:22:16 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:3edc1e07016364eab953a779a57c3678cbd72463d525979c310312fc3c326303
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89410617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ba7251209c03b003aff33e3f672609aba45f45d8354342e59ba43050565e85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 03:43:27 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 03:53:59 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 03:54:01 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 03:54:09 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 03:54:11 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 03:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 03:54:14 GMT
CMD ["node"]
# Wed, 29 Apr 2020 04:55:14 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 04:55:16 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 04:55:17 GMT
ENV NODE_ENV=production
# Wed, 29 Apr 2020 04:55:18 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 29 Apr 2020 04:56:02 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Apr 2020 04:56:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Apr 2020 04:56:06 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 07 May 2020 14:49:44 GMT
ENV GHOST_VERSION=3.15.0
# Thu, 07 May 2020 14:56:33 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 07 May 2020 14:56:37 GMT
WORKDIR /var/lib/ghost
# Thu, 07 May 2020 14:56:37 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 07 May 2020 14:56:38 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 07 May 2020 14:56:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 14:56:39 GMT
EXPOSE 2368
# Thu, 07 May 2020 14:56:39 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a762f3ab8e9ca9588cfb098615c9cd37ab18bc650478364e822aadf8000847`  
		Last Modified: Wed, 29 Apr 2020 03:55:50 GMT  
		Size: 24.1 MB (24058166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab02e90fed213526843504df49512e4ab833c96a6d16a1c809dec659c3998572`  
		Last Modified: Wed, 29 Apr 2020 03:55:40 GMT  
		Size: 2.3 MB (2294463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080a5fc8f30e6ecf91152815bdf244f51f77e2f2ddd6a77be9e4dab5f62a619e`  
		Last Modified: Wed, 29 Apr 2020 03:55:40 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ff3ca17765394c3bae6471680e74aceed23d26d5d92a87c746b30217e94d90`  
		Last Modified: Wed, 29 Apr 2020 05:03:02 GMT  
		Size: 9.7 KB (9734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5d0e63744292b74702e67a477edd578e07ec617a71cc71dc9abbf0b052e92b`  
		Last Modified: Wed, 29 Apr 2020 05:03:02 GMT  
		Size: 732.3 KB (732324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74bc81633484a69ddb7ee9a3bad25f736b5c6383e7a08e4b33545ad8ada9206`  
		Last Modified: Wed, 29 Apr 2020 05:03:08 GMT  
		Size: 6.8 MB (6769583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66016ab0761b624fc6be7574efecfb9dbd2424e15e6ecbc0d0d0483853854f99`  
		Last Modified: Thu, 07 May 2020 14:57:29 GMT  
		Size: 52.9 MB (52925583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123497d87a8a5f686acbf24d23262414fb87483b01b6e22f84d8d181547974ca`  
		Last Modified: Thu, 07 May 2020 14:57:02 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:6ea0e5b16f6483e68cc2200416553217ecd69d4bd361d81d523a33b5dd0be6f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.2 MB (88237939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6464cdf24fbab77d9873e2f595eb342af238fdbe924da0ce2ee7f5b97925ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 04:05:52 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 04:14:36 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 04:14:40 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 04:14:45 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 04:14:46 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 04:14:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 04:14:47 GMT
CMD ["node"]
# Wed, 29 Apr 2020 05:26:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 05:27:00 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 05:27:00 GMT
ENV NODE_ENV=production
# Wed, 29 Apr 2020 05:27:01 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 29 Apr 2020 05:27:28 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Apr 2020 05:27:30 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Apr 2020 05:27:31 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 07 May 2020 15:02:30 GMT
ENV GHOST_VERSION=3.15.0
# Thu, 07 May 2020 15:07:10 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 07 May 2020 15:07:15 GMT
WORKDIR /var/lib/ghost
# Thu, 07 May 2020 15:07:15 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 07 May 2020 15:07:16 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 07 May 2020 15:07:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 15:07:17 GMT
EXPOSE 2368
# Thu, 07 May 2020 15:07:18 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194c2687741a4c309a174979cf358db1f39ab3d29acebb9be2e68fbec4333d4d`  
		Last Modified: Wed, 29 Apr 2020 04:19:31 GMT  
		Size: 23.6 MB (23624116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa62051444244200ee6f4c32908ba92298cd322c7a8d0df3f142c8e672cd6ce3`  
		Last Modified: Wed, 29 Apr 2020 04:19:22 GMT  
		Size: 2.3 MB (2294716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a230cbec1f938a60e848c9f6c7985176548ed604bd8281b45b55ab1321b14e17`  
		Last Modified: Wed, 29 Apr 2020 04:19:20 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb3c013e42b2d047b9ae4ba43fc558251649cf42411e310517ebd303494515b`  
		Last Modified: Wed, 29 Apr 2020 05:33:21 GMT  
		Size: 9.5 KB (9517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b95f3fe3d1602e6aa7a1232de84d4778945067617590b643d0d74b545c6274`  
		Last Modified: Wed, 29 Apr 2020 05:33:21 GMT  
		Size: 669.1 KB (669126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d40efc2598fc73ef7a50c000347fe4b0caefc0ed8eeb054b81abe991a3ee52`  
		Last Modified: Wed, 29 Apr 2020 05:33:25 GMT  
		Size: 6.8 MB (6769227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174de7623eb0720042e26cb409cb639b7bcaddd35023d9e207796bfacec2a4e7`  
		Last Modified: Thu, 07 May 2020 15:08:57 GMT  
		Size: 52.4 MB (52448348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb6d644656f5259c93d5dfcfecc4feb83e100883bd329af305fe07b9ebef0a6`  
		Last Modified: Thu, 07 May 2020 15:08:33 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:89ea6e40a2f33457da86ce95ff95e4a5a721499c110e82460a61290859c07f5b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90472416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44cb6ab6b4a500f1a8373cbd19c311c6e03e80b7b9a4d0e1cdd7116c6a899517`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 03:14:20 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 03:25:21 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 03:25:26 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 03:25:36 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 03:25:38 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 03:25:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 03:25:45 GMT
CMD ["node"]
# Wed, 29 Apr 2020 05:20:53 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 05:20:55 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 05:20:56 GMT
ENV NODE_ENV=production
# Wed, 29 Apr 2020 05:20:57 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 29 Apr 2020 05:21:22 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Apr 2020 05:21:24 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Apr 2020 05:21:24 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 07 May 2020 14:43:44 GMT
ENV GHOST_VERSION=3.15.0
# Thu, 07 May 2020 14:48:26 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 07 May 2020 14:48:31 GMT
WORKDIR /var/lib/ghost
# Thu, 07 May 2020 14:48:31 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 07 May 2020 14:48:32 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 07 May 2020 14:48:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 14:48:33 GMT
EXPOSE 2368
# Thu, 07 May 2020 14:48:34 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d225dfe749d02a9c816430b13e9d42df6d01e60edd8b40a7a3da752e71287a36`  
		Last Modified: Wed, 29 Apr 2020 03:32:53 GMT  
		Size: 24.8 MB (24784078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d039f495375355afd6cdb0e53e506f7b39160ac0a03c7ffabfa86c7ad9f684`  
		Last Modified: Wed, 29 Apr 2020 03:32:46 GMT  
		Size: 2.3 MB (2302007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ae23a308483639c691f955826f00ef1e6fffc2494322f5d9ad3f9860816130`  
		Last Modified: Wed, 29 Apr 2020 03:32:46 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85be0b668d031687b6002147c702f5949466b15793fec336fccf6f8787e2a963`  
		Last Modified: Wed, 29 Apr 2020 05:26:45 GMT  
		Size: 9.8 KB (9847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe041863ce98237b3623161d6e84888b56bece5e3a319442ddcfc8cd86bdb5d`  
		Last Modified: Wed, 29 Apr 2020 05:26:45 GMT  
		Size: 791.3 KB (791337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e159d3e27a1ecea20809edc10e42d3c4a367f7a20017b9d2c92310580409504a`  
		Last Modified: Wed, 29 Apr 2020 05:26:49 GMT  
		Size: 6.8 MB (6769245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a7d3d411a52df5eef84c78a7327a8f02cae4fba6e80ca700e8d861d03fcff`  
		Last Modified: Thu, 07 May 2020 14:49:58 GMT  
		Size: 53.1 MB (53090652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76feda4aef039a4ed626d918b97d5f24b57f12614b7ab2610db7a4db8c6d5fd9`  
		Last Modified: Thu, 07 May 2020 14:49:39 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; 386

```console
$ docker pull ghost@sha256:e2c6c6b04597be9af57b639f72cf627577a40f0729cb6f5668e820e4136b54a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.8 MB (90804368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3b8cbcc9b569818cae94810dd213f6e9d6becc35ec0b59ec277e92dd3fe84de`
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
# Wed, 29 Apr 2020 06:19:39 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 29 Apr 2020 06:19:57 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Apr 2020 06:19:57 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Apr 2020 06:19:57 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 07 May 2020 14:38:28 GMT
ENV GHOST_VERSION=3.15.0
# Thu, 07 May 2020 14:41:28 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 07 May 2020 14:41:29 GMT
WORKDIR /var/lib/ghost
# Thu, 07 May 2020 14:41:29 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 07 May 2020 14:41:29 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 07 May 2020 14:41:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 14:41:30 GMT
EXPOSE 2368
# Thu, 07 May 2020 14:41:30 GMT
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
	-	`sha256:5d02b78e277adc01d6c71ef1dab466837a85204adb8d8f941a68181519074d8f`  
		Last Modified: Wed, 29 Apr 2020 06:23:20 GMT  
		Size: 6.8 MB (6769129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d205fde6300628b57651290c96eb78f7a938069c4f27324532971f41cc38a4a9`  
		Last Modified: Thu, 07 May 2020 14:42:12 GMT  
		Size: 53.2 MB (53160278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b0028048006df5d412a7535e8a1380874b7420fddd4d28e8fa1e0770fc9c27`  
		Last Modified: Thu, 07 May 2020 14:41:53 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; ppc64le

```console
$ docker pull ghost@sha256:4f87d46321e034b50061b5b8dc1a3b678089413499573f09736f55daae0d2199
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.7 MB (93708850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b067c925c9daba06a361b13fe9c21ad38ebf3ff2eb093d801c034ff21d9ba5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 03:37:45 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 03:54:35 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 03:54:38 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 03:54:47 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 03:54:48 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 03:54:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 03:54:52 GMT
CMD ["node"]
# Wed, 29 Apr 2020 04:39:43 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 04:39:48 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 04:39:51 GMT
ENV NODE_ENV=production
# Wed, 29 Apr 2020 04:39:53 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 29 Apr 2020 04:40:26 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Apr 2020 04:40:29 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Apr 2020 04:40:31 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 07 May 2020 15:24:28 GMT
ENV GHOST_VERSION=3.15.0
# Thu, 07 May 2020 15:29:24 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 07 May 2020 15:29:31 GMT
WORKDIR /var/lib/ghost
# Thu, 07 May 2020 15:29:35 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 07 May 2020 15:29:37 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 07 May 2020 15:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 15:29:46 GMT
EXPOSE 2368
# Thu, 07 May 2020 15:29:49 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96424fc634e75f33dcc5c3439f046b61280674b82f305977bc3527cd3847eb7`  
		Last Modified: Wed, 29 Apr 2020 04:00:25 GMT  
		Size: 26.9 MB (26939117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d59830dda23ab1d9e983e75e328077e4713223cf0e1a73985bacd7aa1b01dbb`  
		Last Modified: Wed, 29 Apr 2020 04:00:19 GMT  
		Size: 2.3 MB (2302072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c16920d6879dabf667d1a6fef59820dd5cef06cf6771a646b8859a23efa0c0a`  
		Last Modified: Wed, 29 Apr 2020 04:00:18 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637ea9713e199bcc39a70d529a3863a97e8ce7f28c7f1344fc47e4732d050f48`  
		Last Modified: Wed, 29 Apr 2020 04:46:12 GMT  
		Size: 10.4 KB (10398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7169d4f22099d3faad2e4905f393d333628b3b81b1bc960ab692d594346f7334`  
		Last Modified: Wed, 29 Apr 2020 04:46:13 GMT  
		Size: 862.6 KB (862586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d79ffcf08e48af7b607b3862619b7e7880b89b77f539a8561d9e292cdbe4dba`  
		Last Modified: Wed, 29 Apr 2020 04:46:28 GMT  
		Size: 6.8 MB (6768936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d07d55cedbb3d9d9f3e8b2014ad808153e8c856a20e26378f3b0211946dede`  
		Last Modified: Thu, 07 May 2020 15:32:34 GMT  
		Size: 54.0 MB (54003070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdb273d2eb133790457033b7478ac4edef4bcf2e9bfef515685ebe85adf2a5d`  
		Last Modified: Thu, 07 May 2020 15:32:19 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:3-alpine` - linux; s390x

```console
$ docker pull ghost@sha256:67e11542cb4365f6d227d64154099a9169e4351b2c92aba33209f36b4a16cdc2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90170765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c047ba109b80612e3fcaf9e7c0af61e079d1f573c55e3979eecf3327f8a41de4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Wed, 29 Apr 2020 03:17:58 GMT
ENV NODE_VERSION=12.16.3
# Wed, 29 Apr 2020 03:33:31 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="af47aa64de372d9a9d16307b6af9785ee28bdf9892f1de28a78b85917dacf257"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 29 Apr 2020 03:33:32 GMT
ENV YARN_VERSION=1.22.4
# Wed, 29 Apr 2020 03:33:34 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 29 Apr 2020 03:33:35 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 29 Apr 2020 03:33:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Apr 2020 03:33:35 GMT
CMD ["node"]
# Wed, 29 Apr 2020 05:07:18 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 29 Apr 2020 05:07:19 GMT
RUN apk add --no-cache 		bash
# Wed, 29 Apr 2020 05:07:20 GMT
ENV NODE_ENV=production
# Wed, 29 Apr 2020 05:07:20 GMT
ENV GHOST_CLI_VERSION=1.13.1
# Wed, 29 Apr 2020 05:07:34 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 29 Apr 2020 05:07:36 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 29 Apr 2020 05:07:36 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 07 May 2020 14:43:28 GMT
ENV GHOST_VERSION=3.15.0
# Thu, 07 May 2020 14:45:19 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip 0.0.0.0 --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps python make gcc g++ libc-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 07 May 2020 14:45:24 GMT
WORKDIR /var/lib/ghost
# Thu, 07 May 2020 14:45:24 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 07 May 2020 14:45:25 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 07 May 2020 14:45:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 14:45:25 GMT
EXPOSE 2368
# Thu, 07 May 2020 14:45:25 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e153d32276dd38ffaab972ef44b1909a0f15e11a3e4d909675c2a0779d1bb1ab`  
		Last Modified: Wed, 29 Apr 2020 03:36:49 GMT  
		Size: 24.7 MB (24700632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348835d2293b70c40580bfca55d5fda417d664dea8fcecc7430999519bedeeda`  
		Last Modified: Wed, 29 Apr 2020 03:36:45 GMT  
		Size: 2.3 MB (2304559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542996d7c004ddc09e71199b5906795e150abd9d406112383787c5f863638ee4`  
		Last Modified: Wed, 29 Apr 2020 03:36:45 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4313b26c98d46a5c597b9090a011ce7ad89fdb40df5c4a222fa484ed03c705a3`  
		Last Modified: Wed, 29 Apr 2020 05:10:32 GMT  
		Size: 10.0 KB (9997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb075b69f4d46d4285745ae89e9d34f839f4c4f2feab447c885edfe5da3e6efe`  
		Last Modified: Wed, 29 Apr 2020 05:10:32 GMT  
		Size: 813.9 KB (813944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb49656528968a7ad6f6397e6a26158f5177569e34655988aa27e5b1a57ff969`  
		Last Modified: Wed, 29 Apr 2020 05:10:33 GMT  
		Size: 6.8 MB (6769138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a88612d2288dbc018ed6a69ea4bb0bf1d164235cd35a1a1735c48e6800f17dc`  
		Last Modified: Thu, 07 May 2020 14:46:18 GMT  
		Size: 53.0 MB (52988810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2bb4e68319321aff5bdffc78ab66a0b531934d514d3931008cea50bfd18c4b`  
		Last Modified: Thu, 07 May 2020 14:46:13 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
