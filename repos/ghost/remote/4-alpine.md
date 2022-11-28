## `ghost:4-alpine`

```console
$ docker pull ghost@sha256:2b7cab33777b99fafaf4ef7c2226c11c7ae873d9257c4b3865d066f2801f2c8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:4-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:4e0e37f29a5e84a04ccbc31ec1fd1908ed707c1d4108f978cac31f350736059f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138538779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1377e25717a4730d1d8e4c1c055596227c492e3ea08dbc9d6a0697a882e6fcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 06:32:07 GMT
ENV NODE_VERSION=14.21.1
# Sat, 12 Nov 2022 06:32:15 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="0fc7c18a1fa7aa6b39ac7b11ba2e56fa12ab1c4d3b4bb32f9c4ac3f7178d613c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 12 Nov 2022 06:32:16 GMT
ENV YARN_VERSION=1.22.19
# Sat, 12 Nov 2022 06:32:20 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 12 Nov 2022 06:32:20 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 12 Nov 2022 06:32:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 06:32:20 GMT
CMD ["node"]
# Sat, 12 Nov 2022 11:27:35 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 11:27:36 GMT
RUN apk add --no-cache 		bash
# Sat, 12 Nov 2022 11:27:36 GMT
ENV NODE_ENV=production
# Sat, 12 Nov 2022 11:27:36 GMT
ENV GHOST_CLI_VERSION=1.23.1
# Sat, 12 Nov 2022 11:28:00 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 12 Nov 2022 11:28:00 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 12 Nov 2022 11:28:01 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 28 Nov 2022 14:40:25 GMT
ENV GHOST_VERSION=4.48.9
# Mon, 28 Nov 2022 14:42:06 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 28 Nov 2022 14:42:09 GMT
WORKDIR /var/lib/ghost
# Mon, 28 Nov 2022 14:42:09 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 28 Nov 2022 14:42:09 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 28 Nov 2022 14:42:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Nov 2022 14:42:09 GMT
EXPOSE 2368
# Mon, 28 Nov 2022 14:42:09 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c774934c91f00c542a1fb93212d42cf819d47de47169f00eba8db7e7026f51`  
		Last Modified: Sat, 12 Nov 2022 06:37:20 GMT  
		Size: 37.7 MB (37724346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d9211bf297cc0df2b07d2ad8ee5a83f5f479165228a1a513004dba925cfc20`  
		Last Modified: Sat, 12 Nov 2022 06:37:15 GMT  
		Size: 2.4 MB (2368725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14523e6c1be223f204f3266fd2d66cc5d9caf28f41364bfa565923c09ed3b4db`  
		Last Modified: Sat, 12 Nov 2022 06:37:14 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6df5a33c8d055ce1259d2b29b7854405e699e1b444b523db9b1bf8342f9fc26`  
		Last Modified: Sat, 12 Nov 2022 11:30:32 GMT  
		Size: 11.3 KB (11295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cf5c4a5c5408e30aa38cc30b22c9d22699130f32b2537db3e4ef7316ad003`  
		Last Modified: Sat, 12 Nov 2022 11:30:32 GMT  
		Size: 820.1 KB (820068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf5fa079d29a8020c2f30554dec49ebf6b4f476258dfcd337a6dd3d7e982384`  
		Last Modified: Sat, 12 Nov 2022 11:30:35 GMT  
		Size: 10.2 MB (10245542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb67916d3b1901c83a83ccb9331653fbf4d6268ce3c82876baf2e13086295d9`  
		Last Modified: Mon, 28 Nov 2022 14:44:16 GMT  
		Size: 84.6 MB (84561536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae764393985df742400b2956fd2b1b7fb1c7a91801e7207fa865b915e5e2cfb`  
		Last Modified: Mon, 28 Nov 2022 14:44:00 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:0fb083185cbeb06c6a5a1745f7d2a60ddd5758f2aca950a1e977cdf3961f426a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142191453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab35cdbf962cac0091ed8c7ccd5a6cc6573dd115ed45ff465cb98db7ea0066f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 10:49:14 GMT
ENV NODE_VERSION=14.21.1
# Sat, 12 Nov 2022 11:23:46 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="0fc7c18a1fa7aa6b39ac7b11ba2e56fa12ab1c4d3b4bb32f9c4ac3f7178d613c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 12 Nov 2022 11:23:48 GMT
ENV YARN_VERSION=1.22.19
# Sat, 12 Nov 2022 11:23:54 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 12 Nov 2022 11:23:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 12 Nov 2022 11:23:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 11:23:55 GMT
CMD ["node"]
# Sat, 12 Nov 2022 14:15:57 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 14:15:58 GMT
RUN apk add --no-cache 		bash
# Sat, 12 Nov 2022 14:15:58 GMT
ENV NODE_ENV=production
# Sat, 12 Nov 2022 14:15:58 GMT
ENV GHOST_CLI_VERSION=1.23.1
# Sat, 12 Nov 2022 14:16:35 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 12 Nov 2022 14:16:36 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 12 Nov 2022 14:16:36 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 28 Nov 2022 14:45:31 GMT
ENV GHOST_VERSION=4.48.9
# Mon, 28 Nov 2022 14:51:21 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 28 Nov 2022 14:51:27 GMT
WORKDIR /var/lib/ghost
# Mon, 28 Nov 2022 14:51:27 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 28 Nov 2022 14:51:27 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 28 Nov 2022 14:51:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Nov 2022 14:51:27 GMT
EXPOSE 2368
# Mon, 28 Nov 2022 14:51:27 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2013ca6af2177095883e23da431551e40beacbe9b328bd9a64b101c7afb7af44`  
		Last Modified: Sat, 12 Nov 2022 11:29:32 GMT  
		Size: 36.7 MB (36749486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206761edc1c09db4001f2e6e0ec7451ce3e09df10209b08330620e64ac1a5ba4`  
		Last Modified: Sat, 12 Nov 2022 11:29:25 GMT  
		Size: 2.4 MB (2417570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b20dd6b1b095cad4cf131f991c687c89721cc3b787ad3f134c76b75472b8d9`  
		Last Modified: Sat, 12 Nov 2022 11:29:24 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0af623f089836b4d1c0948bdf9f60e6d9b0cb1cb213e3b91310aabc839fd16`  
		Last Modified: Sat, 12 Nov 2022 14:23:48 GMT  
		Size: 11.0 KB (10992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f949fa7d5d18587a9c4c5bd0ecf584329557957f7f2c2ef1a8c2a292e8112a72`  
		Last Modified: Sat, 12 Nov 2022 14:23:49 GMT  
		Size: 772.0 KB (771958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ddc36407495dd1762664fbc5aa936ce3a4ab1dd65adebc12a2a166c5e01a64`  
		Last Modified: Sat, 12 Nov 2022 14:23:53 GMT  
		Size: 10.2 MB (10245693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b819129eb3c53f0923d42a7c8189e92e9a798b45985cd932be78991412a8866`  
		Last Modified: Mon, 28 Nov 2022 14:53:20 GMT  
		Size: 89.4 MB (89379652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54227c25877b4e9a92a6ca6e7b6400980fed8ccacd1927e94be8149b9f2efee`  
		Last Modified: Mon, 28 Nov 2022 14:52:52 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:ac66c421d4484af7f1194d2b39f838a6ff747fff2183c38572b73c1c65db6514
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140908855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fce3175314fe8fee631e15e60ebaa94c9680d92d9b97cb3cd2bfa1cadb8e523`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 12:29:08 GMT
ENV NODE_VERSION=14.21.1
# Sat, 12 Nov 2022 12:49:23 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="0fc7c18a1fa7aa6b39ac7b11ba2e56fa12ab1c4d3b4bb32f9c4ac3f7178d613c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 12 Nov 2022 12:49:24 GMT
ENV YARN_VERSION=1.22.19
# Sat, 12 Nov 2022 12:49:28 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 12 Nov 2022 12:49:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 12 Nov 2022 12:49:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 12:49:29 GMT
CMD ["node"]
# Sat, 12 Nov 2022 19:10:25 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 19:10:26 GMT
RUN apk add --no-cache 		bash
# Sat, 12 Nov 2022 19:10:26 GMT
ENV NODE_ENV=production
# Sat, 12 Nov 2022 19:10:26 GMT
ENV GHOST_CLI_VERSION=1.23.1
# Sat, 12 Nov 2022 19:10:53 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 12 Nov 2022 19:10:53 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 12 Nov 2022 19:10:53 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 28 Nov 2022 14:53:33 GMT
ENV GHOST_VERSION=4.48.9
# Mon, 28 Nov 2022 14:57:58 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 28 Nov 2022 14:58:03 GMT
WORKDIR /var/lib/ghost
# Mon, 28 Nov 2022 14:58:03 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 28 Nov 2022 14:58:03 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 28 Nov 2022 14:58:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Nov 2022 14:58:03 GMT
EXPOSE 2368
# Mon, 28 Nov 2022 14:58:03 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b251d39d15356abea2c79230cf242fab87ea74bcd05dd281e6f94fe97e36e4`  
		Last Modified: Sat, 12 Nov 2022 13:00:48 GMT  
		Size: 36.7 MB (36669594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a1a3e393e3b1bfc92d8653ae53a13c82581b6e927af79f7fa56cd75be265ee`  
		Last Modified: Sat, 12 Nov 2022 13:00:42 GMT  
		Size: 2.4 MB (2417705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cc7093a86ad8a89189e7286dfaaf1a732af19710a95ccc4e194c4e27fe80d8`  
		Last Modified: Sat, 12 Nov 2022 13:00:41 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eee7557e1106e8660cb2248f22e7a56393c67a6af0267619d9d0947e1dd68bd`  
		Last Modified: Sat, 12 Nov 2022 19:17:07 GMT  
		Size: 10.8 KB (10800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77eda6ad1a4963332eab5f01c258f2803d646f5c4b51d4831d3f396881e27e3`  
		Last Modified: Sat, 12 Nov 2022 19:17:07 GMT  
		Size: 704.7 KB (704668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837f04ca0a1d999700ebaa7f545e48615c0e834cc567695bca2b323052456127`  
		Last Modified: Sat, 12 Nov 2022 19:17:11 GMT  
		Size: 10.2 MB (10245678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b120a91da2ad7be2d8c5262e7b94f404ff7540cfc70ddb8fdf643aacc5934874`  
		Last Modified: Mon, 28 Nov 2022 15:01:36 GMT  
		Size: 88.4 MB (88440626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbb119675bebfc988a4d9574029865ec3845b31ef97c760329542a1aa6fecda`  
		Last Modified: Mon, 28 Nov 2022 15:01:09 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:4-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:05c961287b35d129e1e732e54ee63c4263643a980772bb6ab239049c9c76a0e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135469130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9f67bab252eda285e7e4daf190ed51691eb4bbac42a3f5e3ccd58a0dac0c1ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:56:53 GMT
ENV NODE_VERSION=14.21.1
# Sat, 12 Nov 2022 08:11:05 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="0fc7c18a1fa7aa6b39ac7b11ba2e56fa12ab1c4d3b4bb32f9c4ac3f7178d613c"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 12 Nov 2022 08:11:06 GMT
ENV YARN_VERSION=1.22.19
# Sat, 12 Nov 2022 08:11:11 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 12 Nov 2022 08:11:11 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:11:11 GMT
CMD ["node"]
# Sat, 12 Nov 2022 11:33:50 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 12 Nov 2022 11:33:51 GMT
RUN apk add --no-cache 		bash
# Sat, 12 Nov 2022 11:33:51 GMT
ENV NODE_ENV=production
# Sat, 12 Nov 2022 11:33:51 GMT
ENV GHOST_CLI_VERSION=1.23.1
# Sat, 12 Nov 2022 11:34:11 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 12 Nov 2022 11:34:12 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 12 Nov 2022 11:34:12 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 28 Nov 2022 14:45:16 GMT
ENV GHOST_VERSION=4.48.9
# Mon, 28 Nov 2022 14:46:39 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	sqlite3Version="$(node -p 'require("./package.json").optionalDependencies["sqlite3"]')"; 	[ -n "$sqlite3Version" ]; 	[ "$sqlite3Version" != 'undefined' ]; 	if ! su-exec node yarn add "sqlite3@$sqlite3Version" --force; then 		apk add --no-cache --virtual .build-deps g++ gcc libc-dev make python3 vips-dev; 				su-exec node yarn add "sqlite3@$sqlite3Version" --force --build-from-source; 				apk del --no-network .build-deps; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 28 Nov 2022 14:46:44 GMT
WORKDIR /var/lib/ghost
# Mon, 28 Nov 2022 14:46:44 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 28 Nov 2022 14:46:44 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 28 Nov 2022 14:46:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 28 Nov 2022 14:46:44 GMT
EXPOSE 2368
# Mon, 28 Nov 2022 14:46:44 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd3f8016cbc63b3b13a298021c1681bf77749b18a9aeaf756c4d57fee9c1c72`  
		Last Modified: Sat, 12 Nov 2022 08:16:07 GMT  
		Size: 37.6 MB (37552542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789bf1647f9802940b12385260daf689771a255e5c7508874b89e3f92abd4bb`  
		Last Modified: Sat, 12 Nov 2022 08:16:03 GMT  
		Size: 2.4 MB (2425934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9f9da8b41400f1fccb3ce147e7508de0fcba2852569735aa225e7b75c98926`  
		Last Modified: Sat, 12 Nov 2022 08:16:02 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ccbb9dc2c54dcdda274ba33cfbe3fc7919c007ab182ebe828f4a45537812cba`  
		Last Modified: Sat, 12 Nov 2022 11:36:32 GMT  
		Size: 11.1 KB (11106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b609e2bb235cf901848338bf5a92bc34385f1449e2c7391d125aa348f68f121d`  
		Last Modified: Sat, 12 Nov 2022 11:36:33 GMT  
		Size: 826.3 KB (826327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b1bf97318ed9deb56c6e49a57b09ea59ad67b9bbdbba05607f8e1e348a6a2`  
		Last Modified: Sat, 12 Nov 2022 11:36:35 GMT  
		Size: 10.2 MB (10245237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f54bda74b3c3dbbfdd6d633ae49129bee21ca19da4f462e420c21df0698c4c`  
		Last Modified: Mon, 28 Nov 2022 14:48:42 GMT  
		Size: 81.7 MB (81699233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9af94f2a43e28d4b83c7084e94263416fd3ba835036d06442b8a632479efa`  
		Last Modified: Mon, 28 Nov 2022 14:48:30 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
