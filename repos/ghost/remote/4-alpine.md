## `ghost:4-alpine`

```console
$ docker pull ghost@sha256:10e18372756276db3ae885bc7c827f2491ffd26277b26aa31fdebffe3cb43986
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:4-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:578d6812f4362394792f221529ecf1862be4af2e1fe4866c5fd7d733293ea8f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138531037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a96aa8ac5df46785fc043e50c29a4f2c082e71c955ec85a0d4ced1a45bd0f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 08 Nov 2022 18:37:00 GMT
ENV NODE_VERSION=14.21.1
# Tue, 08 Nov 2022 18:37:07 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="0fc7c18a1fa7aa6b39ac7b11ba2e56fa12ab1c4d3b4bb32f9c4ac3f7178d613c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 08 Nov 2022 18:37:08 GMT
ENV YARN_VERSION=1.22.19
# Tue, 08 Nov 2022 18:37:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 08 Nov 2022 18:37:12 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 08 Nov 2022 18:37:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Nov 2022 18:37:12 GMT
CMD ["node"]
# Tue, 08 Nov 2022 20:11:48 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 08 Nov 2022 20:11:49 GMT
RUN apk add --no-cache 		bash
# Tue, 08 Nov 2022 20:11:49 GMT
ENV NODE_ENV=production
# Tue, 08 Nov 2022 20:11:49 GMT
ENV GHOST_CLI_VERSION=1.23.1
# Tue, 08 Nov 2022 20:12:16 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 08 Nov 2022 20:12:17 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 08 Nov 2022 20:12:17 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 08 Nov 2022 20:12:17 GMT
ENV GHOST_VERSION=4.48.7
# Tue, 08 Nov 2022 20:13:56 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 08 Nov 2022 20:13:59 GMT
WORKDIR /var/lib/ghost
# Tue, 08 Nov 2022 20:13:59 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 08 Nov 2022 20:13:59 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 08 Nov 2022 20:13:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Nov 2022 20:13:59 GMT
EXPOSE 2368
# Tue, 08 Nov 2022 20:13:59 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c017beec90fbc61c6f5157d956001f117c8b03fed537385dc73e31c6b25d87`  
		Last Modified: Tue, 08 Nov 2022 18:51:09 GMT  
		Size: 37.7 MB (37724399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b4aabc0b09aade4c0d2860a516445c9211a7fde95681a3d4d2cebdf7ab4297`  
		Last Modified: Tue, 08 Nov 2022 18:51:04 GMT  
		Size: 2.4 MB (2368635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9f836f8ff28cd8cd3a44f8293157a8380d66649ce5fc7cc06a7a8b866e42e1`  
		Last Modified: Tue, 08 Nov 2022 18:51:03 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd90a4d77d0c71877c94adbe4fc9dc323a445b3ef9dda19ffe813721a0376b3`  
		Last Modified: Tue, 08 Nov 2022 20:16:05 GMT  
		Size: 11.3 KB (11274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0a99ec9ab92fb55cc8c4cec7235338de29aef450ec1452efb3eed2dbb233bf`  
		Last Modified: Tue, 08 Nov 2022 20:16:05 GMT  
		Size: 820.0 KB (820041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44af21dae7f67f586699fa220fc7e670ab24bfadfe609e67446eedc84a2e18f0`  
		Last Modified: Tue, 08 Nov 2022 20:16:08 GMT  
		Size: 10.2 MB (10244531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e3bc90bc5e45ac47dc798c99d30c493c508fdf0a0885b76c992f76b7089f39`  
		Last Modified: Tue, 08 Nov 2022 20:16:22 GMT  
		Size: 84.6 MB (84555104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6501bb9fa7f0a265982eba9ff1c4f20c33cf93b5e641e95e776d8feb7bc5794`  
		Last Modified: Tue, 08 Nov 2022 20:16:05 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:4349ec085a29c9cd124ab9d0b566a1cf7994db3adb42b74fac26b156517cdc19
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142196833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3863a91bf9af84d5474dcef4091df72dfd939e7c37a7e33c0d3aabe0d97f8386`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Nov 2022 00:14:32 GMT
ENV NODE_VERSION=14.21.1
# Wed, 09 Nov 2022 00:49:50 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="0fc7c18a1fa7aa6b39ac7b11ba2e56fa12ab1c4d3b4bb32f9c4ac3f7178d613c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 09 Nov 2022 00:49:51 GMT
ENV YARN_VERSION=1.22.19
# Wed, 09 Nov 2022 00:49:56 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 09 Nov 2022 00:49:57 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 09 Nov 2022 00:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Nov 2022 00:49:57 GMT
CMD ["node"]
# Wed, 09 Nov 2022 01:31:15 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 09 Nov 2022 01:31:16 GMT
RUN apk add --no-cache 		bash
# Wed, 09 Nov 2022 01:31:16 GMT
ENV NODE_ENV=production
# Wed, 09 Nov 2022 01:31:16 GMT
ENV GHOST_CLI_VERSION=1.23.1
# Wed, 09 Nov 2022 01:31:54 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 09 Nov 2022 01:31:55 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 09 Nov 2022 01:31:55 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 09 Nov 2022 01:31:55 GMT
ENV GHOST_VERSION=4.48.7
# Wed, 09 Nov 2022 01:37:40 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 09 Nov 2022 01:37:46 GMT
WORKDIR /var/lib/ghost
# Wed, 09 Nov 2022 01:37:46 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 09 Nov 2022 01:37:46 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 09 Nov 2022 01:37:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Nov 2022 01:37:46 GMT
EXPOSE 2368
# Wed, 09 Nov 2022 01:37:47 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840623bf71fdcf83f4e35c3768434a7a3209ea027d6f37f5e0b3be9b6ea64aa5`  
		Last Modified: Wed, 09 Nov 2022 00:57:21 GMT  
		Size: 37.1 MB (37149207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5185ba0199b6102cce793ac0a5380e5fd734695b4fd522cd66f322e7525cb87e`  
		Last Modified: Wed, 09 Nov 2022 00:57:14 GMT  
		Size: 2.4 MB (2417731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bf60f232c1a4809e6109078ddb40dfae97478bfaa5dc330b0c3d71324dcb08`  
		Last Modified: Wed, 09 Nov 2022 00:57:13 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d304ff716a87f595881ce94536b7d33af32eb86407a69b1ec847c5697930cf31`  
		Last Modified: Wed, 09 Nov 2022 01:39:08 GMT  
		Size: 11.0 KB (10997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8272cb6dbe2cc07a6d9a206d937e2046612a071ab5eacda2d529d0f9153269c8`  
		Last Modified: Wed, 09 Nov 2022 01:39:09 GMT  
		Size: 772.0 KB (771961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19fbc5c0c30637ab95c1b2500048172bf30cb5e321e66fc0f6ff2e3ba7c085f`  
		Last Modified: Wed, 09 Nov 2022 01:39:13 GMT  
		Size: 10.2 MB (10244705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a344ff1acd1fddfad3ef80cbb4dc3013c35b7c0eeabe5bb3b5d7cc75b4cbebf8`  
		Last Modified: Wed, 09 Nov 2022 01:39:36 GMT  
		Size: 89.0 MB (88987274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d7e72d8475069c38507a82f40896ff562bf1d1a6640aae40f52cdebb32ff2e`  
		Last Modified: Wed, 09 Nov 2022 01:39:08 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:acdde2a097dba9fa2e67ffd63e6c0753e9a74b94be416f22cf1e42d8485d5e08
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140897600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f1aeaa991a4d5a1a57836187122bc5d40878ac1721378d9bd1b250890d957d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 09 Nov 2022 00:51:35 GMT
ENV NODE_VERSION=14.21.1
# Wed, 09 Nov 2022 01:12:05 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="0fc7c18a1fa7aa6b39ac7b11ba2e56fa12ab1c4d3b4bb32f9c4ac3f7178d613c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 09 Nov 2022 01:12:06 GMT
ENV YARN_VERSION=1.22.19
# Wed, 09 Nov 2022 01:12:11 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 09 Nov 2022 01:12:11 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 09 Nov 2022 01:12:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Nov 2022 01:12:11 GMT
CMD ["node"]
# Wed, 09 Nov 2022 02:56:03 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 09 Nov 2022 02:56:04 GMT
RUN apk add --no-cache 		bash
# Wed, 09 Nov 2022 02:56:04 GMT
ENV NODE_ENV=production
# Wed, 09 Nov 2022 02:56:04 GMT
ENV GHOST_CLI_VERSION=1.23.1
# Wed, 09 Nov 2022 02:56:32 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 09 Nov 2022 02:56:33 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 09 Nov 2022 02:56:33 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 09 Nov 2022 02:56:33 GMT
ENV GHOST_VERSION=4.48.7
# Wed, 09 Nov 2022 03:00:57 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 09 Nov 2022 03:01:03 GMT
WORKDIR /var/lib/ghost
# Wed, 09 Nov 2022 03:01:03 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 09 Nov 2022 03:01:04 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 09 Nov 2022 03:01:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 09 Nov 2022 03:01:04 GMT
EXPOSE 2368
# Wed, 09 Nov 2022 03:01:04 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8199a0e5d1f6fb4a3c9fc12990986e94048caef3af7a10a582efad8b1b4cb69`  
		Last Modified: Wed, 09 Nov 2022 01:34:00 GMT  
		Size: 36.7 MB (36669246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc34de3418d04c2c3c6511ac1f98737b693d542bb87ff92966a56d5596f05a28`  
		Last Modified: Wed, 09 Nov 2022 01:33:53 GMT  
		Size: 2.4 MB (2417649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ac74543280e7fda3e9b17a4cc1f2f89d512a44cc8220723a9b94c87a4b291`  
		Last Modified: Wed, 09 Nov 2022 01:33:53 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024e82a82c352e84e99e8073e1812d378c588a65dc25776166e24b6dae4081c5`  
		Last Modified: Wed, 09 Nov 2022 03:04:17 GMT  
		Size: 10.8 KB (10770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14281c0000672acc7b7168c1768870b30fc2cfa752506e16030d6b0820167039`  
		Last Modified: Wed, 09 Nov 2022 03:04:18 GMT  
		Size: 704.6 KB (704639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0142bc42d9943e57bd6d4d31432f92c82e8f8cd4a862448797405964cf100a9`  
		Last Modified: Wed, 09 Nov 2022 03:04:22 GMT  
		Size: 10.2 MB (10244489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e0edf5435a438d85562dbb4032cc84507fa169bedaea51b595d62ea7c360e5`  
		Last Modified: Wed, 09 Nov 2022 03:04:45 GMT  
		Size: 88.4 MB (88432749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43734de84c37206cde49e1edfbfb65af41e6e8a861eb92e7e18c0f9bd07c1d0f`  
		Last Modified: Wed, 09 Nov 2022 03:04:17 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:177666ad66874ebb56092b15662e0607e1dccd4d05816034190d6e3f873e0bd9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.9 MB (135877378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a60e46b6892ba366ba0a9ed623b3ebe4d3f9f3b4be5a75462e3c87b0f1d1de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 08 Nov 2022 21:32:46 GMT
ENV NODE_VERSION=14.21.1
# Tue, 08 Nov 2022 21:46:57 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="0fc7c18a1fa7aa6b39ac7b11ba2e56fa12ab1c4d3b4bb32f9c4ac3f7178d613c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 08 Nov 2022 21:46:57 GMT
ENV YARN_VERSION=1.22.19
# Tue, 08 Nov 2022 21:47:02 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 08 Nov 2022 21:47:02 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 08 Nov 2022 21:47:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Nov 2022 21:47:02 GMT
CMD ["node"]
# Tue, 08 Nov 2022 23:35:32 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 08 Nov 2022 23:35:33 GMT
RUN apk add --no-cache 		bash
# Tue, 08 Nov 2022 23:35:33 GMT
ENV NODE_ENV=production
# Tue, 08 Nov 2022 23:35:33 GMT
ENV GHOST_CLI_VERSION=1.23.1
# Tue, 08 Nov 2022 23:35:56 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 08 Nov 2022 23:35:57 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 08 Nov 2022 23:35:57 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 08 Nov 2022 23:35:57 GMT
ENV GHOST_VERSION=4.48.7
# Tue, 08 Nov 2022 23:37:19 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 08 Nov 2022 23:37:25 GMT
WORKDIR /var/lib/ghost
# Tue, 08 Nov 2022 23:37:25 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 08 Nov 2022 23:37:25 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 08 Nov 2022 23:37:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Nov 2022 23:37:25 GMT
EXPOSE 2368
# Tue, 08 Nov 2022 23:37:25 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b049d45b1d5ebfe018124a2ea938deafaa2bde6eddbeb9019706ef9d174137c8`  
		Last Modified: Tue, 08 Nov 2022 22:00:58 GMT  
		Size: 38.0 MB (37958581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc108c6289ad28c8e2c00f532c23100a8f6af859cf425649cb6a658fbfc29a36`  
		Last Modified: Tue, 08 Nov 2022 22:00:55 GMT  
		Size: 2.4 MB (2425833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0d9cdee91a705c2ed5d4a0afacb15e29a4874feaa1748306665be38b6a9f17`  
		Last Modified: Tue, 08 Nov 2022 22:00:54 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7611171ebcdca356adb0902b1e252b87c48bee583caefb1d7b5344dbf5f9bc`  
		Last Modified: Tue, 08 Nov 2022 23:39:24 GMT  
		Size: 11.1 KB (11107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738fa1facfdfbf7e427aa1fc73fec0e21ba27cbe7b7e89502932aaf111d39ee3`  
		Last Modified: Tue, 08 Nov 2022 23:39:24 GMT  
		Size: 826.3 KB (826333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba4bf9806fa1310695477be5ffc3ab7cb24202e072b1a03abdcf409594a5acd`  
		Last Modified: Tue, 08 Nov 2022 23:39:27 GMT  
		Size: 10.2 MB (10244490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96976e05e797c73945d0c29a0f2e4530278e16eaa644fc9aee0fdcfce7f48b2c`  
		Last Modified: Tue, 08 Nov 2022 23:39:37 GMT  
		Size: 81.7 MB (81702377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d545fca4d6ba40a86d37e0650519ba23690a5a896eb12c39030bc2d158e2f56f`  
		Last Modified: Tue, 08 Nov 2022 23:39:24 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
