## `ghost:alpine`

```console
$ docker pull ghost@sha256:1330400e3b577817c0c5982c9613871e09817e4e4db8d27ae36de7481332ae0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:alpine` - linux; amd64

```console
$ docker pull ghost@sha256:8b3d41947886f5d055755bc129c7604a7baaefc8ea7287c20ccaaf67d22d116f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120529576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546018beef694d3b4989b32210dc5f81cb62094085d87d076f6848fb7db617b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 02 Feb 2022 01:52:47 GMT
ENV NODE_VERSION=14.19.0
# Wed, 02 Feb 2022 01:52:56 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="8d5e638d88b62de2f147dee812a5d74e4860a20468eb7ff32c41a02b58e2aebf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 02 Feb 2022 01:52:56 GMT
ENV YARN_VERSION=1.22.17
# Wed, 02 Feb 2022 01:53:04 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 02 Feb 2022 01:53:04 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 02 Feb 2022 01:53:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 01:53:05 GMT
CMD ["node"]
# Wed, 02 Feb 2022 02:34:21 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 02 Feb 2022 02:34:23 GMT
RUN apk add --no-cache 		bash
# Wed, 02 Feb 2022 02:34:23 GMT
ENV NODE_ENV=production
# Wed, 02 Feb 2022 02:34:23 GMT
ENV GHOST_CLI_VERSION=1.18.1
# Wed, 02 Feb 2022 02:34:46 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 02 Feb 2022 02:34:47 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 02 Feb 2022 02:34:47 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 01 Mar 2022 02:44:46 GMT
ENV GHOST_VERSION=4.37.0
# Thu, 03 Mar 2022 06:34:19 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 03 Mar 2022 06:34:21 GMT
WORKDIR /var/lib/ghost
# Thu, 03 Mar 2022 06:34:21 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 03 Mar 2022 06:34:21 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 03 Mar 2022 06:34:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 06:34:21 GMT
EXPOSE 2368
# Thu, 03 Mar 2022 06:34:21 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ae0bc29be10e5ca7d928631baa84ae04ccc7f89d479e0b186c41c45cb64609`  
		Last Modified: Wed, 02 Feb 2022 02:03:50 GMT  
		Size: 37.1 MB (37133034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5329011e23a3efc9db06dfb6aa70f6cc315c95e7f52331b84947644cf07aa22`  
		Last Modified: Wed, 02 Feb 2022 02:03:46 GMT  
		Size: 2.4 MB (2358528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0eb5127ee8f326b7a00ddd86b1836d7225cf18359bc0bd2e46fa8d2718e5075`  
		Last Modified: Wed, 02 Feb 2022 02:03:45 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6306d7d857224f9d4f7b83ff7d0ef5cd45516acf4ac4b8261a9eced5d26b7e`  
		Last Modified: Wed, 02 Feb 2022 02:37:07 GMT  
		Size: 11.2 KB (11219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efec01ff9868fa693f30cec7123496b2c4b3193eddeda96d66b6936257d80d78`  
		Last Modified: Wed, 02 Feb 2022 02:37:06 GMT  
		Size: 816.9 KB (816876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a20dd0ed17ef3e426bf051604f0e62f66db423b204dace1b98da5dcabd528af`  
		Last Modified: Wed, 02 Feb 2022 02:37:08 GMT  
		Size: 9.4 MB (9428040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8aa2b069188a22f465e179b911ff9d175f42d422df63b5669478df145f0c8e`  
		Last Modified: Thu, 03 Mar 2022 06:35:30 GMT  
		Size: 68.0 MB (67957897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38e663fe63fca3aa8a3b6e67d1195468c5ea4c60f00d77ba15c4a634c0a5a28`  
		Last Modified: Thu, 03 Mar 2022 06:35:17 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:19854fb2ae7f5d7a3fa560e61ec0cbfb5fbc903ca58264a2658b9ecb655f244a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (121991786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2526697fe01bfadcfa4743fbeb3a1c59c21a6727c60de4be10a59390dad7d12a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Tue, 01 Feb 2022 22:50:56 GMT
ENV NODE_VERSION=14.19.0
# Tue, 01 Feb 2022 23:05:33 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="8d5e638d88b62de2f147dee812a5d74e4860a20468eb7ff32c41a02b58e2aebf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 01 Feb 2022 23:05:34 GMT
ENV YARN_VERSION=1.22.17
# Tue, 01 Feb 2022 23:05:43 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 01 Feb 2022 23:05:44 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 01 Feb 2022 23:05:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Feb 2022 23:05:44 GMT
CMD ["node"]
# Tue, 01 Feb 2022 23:45:47 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 01 Feb 2022 23:45:49 GMT
RUN apk add --no-cache 		bash
# Tue, 01 Feb 2022 23:45:50 GMT
ENV NODE_ENV=production
# Tue, 01 Feb 2022 23:45:50 GMT
ENV GHOST_CLI_VERSION=1.18.1
# Tue, 01 Feb 2022 23:47:04 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 01 Feb 2022 23:47:05 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 01 Feb 2022 23:47:06 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 01 Mar 2022 02:08:10 GMT
ENV GHOST_VERSION=4.37.0
# Wed, 02 Mar 2022 18:58:48 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 02 Mar 2022 18:58:52 GMT
WORKDIR /var/lib/ghost
# Wed, 02 Mar 2022 18:58:53 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 02 Mar 2022 18:58:53 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 02 Mar 2022 18:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Mar 2022 18:58:54 GMT
EXPOSE 2368
# Wed, 02 Mar 2022 18:58:55 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167f7cc098c3c222e2194d324ccf21e2d0a60a61eaeb12011919d339732389ab`  
		Last Modified: Tue, 01 Feb 2022 23:28:44 GMT  
		Size: 36.2 MB (36178292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f362566514a930a4d05612e48b72b148b95ac82c776a3a3d5fd86b2e2e1ae7`  
		Last Modified: Tue, 01 Feb 2022 23:28:25 GMT  
		Size: 2.4 MB (2409383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb95236f27701bfe53e30cd7a3eaf957be62c4bd02dec80e148f04f129d9c71`  
		Last Modified: Tue, 01 Feb 2022 23:28:24 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9530afb40266aea04b697effdf1ad5197ccce0e3a2d83e820c3cba2eee82e56`  
		Last Modified: Tue, 01 Feb 2022 23:57:10 GMT  
		Size: 11.0 KB (10980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657757b6f47f42857487430af2f1bbeeb33d689fba2c4afcf0261885da6f1d8b`  
		Last Modified: Tue, 01 Feb 2022 23:57:11 GMT  
		Size: 771.0 KB (770959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f91dfc2421749d8b27e5cb54e7a25576fd20c464d6951ad82af002bc2bc4e63`  
		Last Modified: Tue, 01 Feb 2022 23:57:25 GMT  
		Size: 9.4 MB (9428614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9abcc239bc71a52f8e504376ca1e3ebace29031c38202cec7023be0bb1de334`  
		Last Modified: Wed, 02 Mar 2022 19:00:47 GMT  
		Size: 70.6 MB (70557171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc7dd02b533973bf368a69a459b61d6e5f28c29ce4d07a7c52dc9d90a02e02`  
		Last Modified: Wed, 02 Mar 2022 18:59:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:bea0f1f00372e1496793c6cf3e29762ffa6b74b7b19866ca0cfd863e300809ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.8 MB (120765780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3f750310b2e720b54c9ac5486f9c1efd1d904bf0d336ff8f8a5acd1dcf93bfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Tue, 01 Feb 2022 23:13:21 GMT
ENV NODE_VERSION=14.19.0
# Tue, 01 Feb 2022 23:30:14 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="8d5e638d88b62de2f147dee812a5d74e4860a20468eb7ff32c41a02b58e2aebf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 01 Feb 2022 23:30:15 GMT
ENV YARN_VERSION=1.22.17
# Tue, 01 Feb 2022 23:30:24 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 01 Feb 2022 23:30:24 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 01 Feb 2022 23:30:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Feb 2022 23:30:25 GMT
CMD ["node"]
# Wed, 02 Feb 2022 02:10:15 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 02 Feb 2022 02:10:17 GMT
RUN apk add --no-cache 		bash
# Wed, 02 Feb 2022 02:10:18 GMT
ENV NODE_ENV=production
# Wed, 02 Feb 2022 02:10:18 GMT
ENV GHOST_CLI_VERSION=1.18.1
# Wed, 02 Feb 2022 02:11:12 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 02 Feb 2022 02:11:13 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 02 Feb 2022 02:11:14 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 01 Mar 2022 02:38:12 GMT
ENV GHOST_VERSION=4.37.0
# Thu, 03 Mar 2022 11:42:40 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 03 Mar 2022 11:42:44 GMT
WORKDIR /var/lib/ghost
# Thu, 03 Mar 2022 11:42:44 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 03 Mar 2022 11:42:44 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 03 Mar 2022 11:42:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 11:42:45 GMT
EXPOSE 2368
# Thu, 03 Mar 2022 11:42:46 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce67ae3bc37b951d3ece9b5109a7be73884ed4f18ee1d41287089909a73d31e3`  
		Last Modified: Wed, 02 Feb 2022 00:12:40 GMT  
		Size: 35.7 MB (35744462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35897dda87770e346c117b69ebeb41d0b3b11f35fde3e8d03244cd7b0e2c794`  
		Last Modified: Wed, 02 Feb 2022 00:12:17 GMT  
		Size: 2.4 MB (2409417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c49c18a3ca5964bc9c217f9df8637fe270d1836eb81b99feb382fdf3fff830`  
		Last Modified: Wed, 02 Feb 2022 00:12:16 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c27692d6eaa3163f2a286d5497943a39b75687df39a3ea34f7eff10b89c9920`  
		Last Modified: Wed, 02 Feb 2022 02:21:47 GMT  
		Size: 10.8 KB (10791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c067fcd915b4d22f8ef888196950476bd912bd2f22afcb6c7109057c227097`  
		Last Modified: Wed, 02 Feb 2022 02:21:48 GMT  
		Size: 703.9 KB (703901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fe2d782726c64a20f1088061371afb3684c9b7de92d110912c447c5e2dff5e`  
		Last Modified: Wed, 02 Feb 2022 02:22:02 GMT  
		Size: 9.4 MB (9428253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba9a6d99aa5236ba034a9d720f63c5f43fedefa251d53e4c56d4e4e911dcc81`  
		Last Modified: Thu, 03 Mar 2022 11:46:33 GMT  
		Size: 70.0 MB (70029335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896968e63ac2ce365c765b1b612516c4824eb9c24644bd4267a849346277c969`  
		Last Modified: Thu, 03 Mar 2022 11:45:16 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:17cc23a1cfc957e9a1d3eca339ba1eeeee45c9711f143b9a7f487c35e6a037a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139688154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4e31b45882994bc6086492372763a45a1c3b1459da881570fb0ccf821b11b5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Wed, 02 Feb 2022 00:36:35 GMT
ENV NODE_VERSION=14.19.0
# Wed, 02 Feb 2022 00:57:51 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="8d5e638d88b62de2f147dee812a5d74e4860a20468eb7ff32c41a02b58e2aebf"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 02 Feb 2022 00:57:52 GMT
ENV YARN_VERSION=1.22.17
# Wed, 02 Feb 2022 00:57:57 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 02 Feb 2022 00:57:59 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 02 Feb 2022 00:57:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Feb 2022 00:58:00 GMT
CMD ["node"]
# Wed, 02 Feb 2022 03:28:20 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 02 Feb 2022 03:28:21 GMT
RUN apk add --no-cache 		bash
# Wed, 02 Feb 2022 03:28:22 GMT
ENV NODE_ENV=production
# Wed, 02 Feb 2022 03:28:23 GMT
ENV GHOST_CLI_VERSION=1.18.1
# Wed, 02 Feb 2022 03:28:49 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 02 Feb 2022 03:28:50 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 02 Feb 2022 03:28:51 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 01 Mar 2022 02:28:23 GMT
ENV GHOST_VERSION=4.37.0
# Wed, 02 Mar 2022 20:19:00 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies.sqlite3')"; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python2 vips-dev; 				npm_config_python='python2' su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 02 Mar 2022 20:19:04 GMT
WORKDIR /var/lib/ghost
# Wed, 02 Mar 2022 20:19:06 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 02 Mar 2022 20:19:08 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 02 Mar 2022 20:19:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Mar 2022 20:19:13 GMT
EXPOSE 2368
# Wed, 02 Mar 2022 20:19:16 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880ab3040613ae881a81f710f55b0e02f6cb4630a93a7f360c47a52f65b144eb`  
		Last Modified: Wed, 02 Feb 2022 01:33:16 GMT  
		Size: 37.0 MB (36997475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca57f5503829283c7349de1f6225357495e1b0bf913963a2909b75a32436fe29`  
		Last Modified: Wed, 02 Feb 2022 01:33:10 GMT  
		Size: 2.4 MB (2419991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e5ad76fe44e9dce104a201400fb7c2e6a81b5a52a528592383a01e7766fb50`  
		Last Modified: Wed, 02 Feb 2022 01:33:09 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915ffb4af7d9b775e60fc6cb68076555dd8574c525a5dd98dbfdf98b9f04818c`  
		Last Modified: Wed, 02 Feb 2022 03:33:54 GMT  
		Size: 11.0 KB (11009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fb237f81852d36302b8f70586f421f978a18425dbe20d34919242cd7fc1e93`  
		Last Modified: Wed, 02 Feb 2022 03:33:55 GMT  
		Size: 826.1 KB (826065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb4543ab5a9c0af29f2cb33d822d10829565ab67eb233cfe5a2157aeb8f9785`  
		Last Modified: Wed, 02 Feb 2022 03:33:58 GMT  
		Size: 9.4 MB (9427807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de38665e704c7a504d9440aabf15d3c0ce4bc6d4eb5cc6dba265009fa9ab0b7`  
		Last Modified: Wed, 02 Mar 2022 20:20:41 GMT  
		Size: 87.3 MB (87287111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075c0dbd133dc1347125f77559ef4b3da2a32411d5160319bbdad5d307529070`  
		Last Modified: Wed, 02 Mar 2022 20:20:24 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
