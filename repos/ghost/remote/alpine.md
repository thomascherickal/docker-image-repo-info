## `ghost:alpine`

```console
$ docker pull ghost@sha256:819fa2d2688e51d23a4bcf820304ca02049ad78e89f9e7c0f4b1242b790dfb85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:alpine` - linux; amd64

```console
$ docker pull ghost@sha256:ff34882f16f729b7d96661e72f96333ede565a8d93fc57a9eff9d6cf7fb3e4dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119355639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0211ecd816614d1109edf12ac969151971c4c83a7367f0f1cf572713d75b72c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:38:12 GMT
ENV NODE_VERSION=16.16.0
# Mon, 18 Jul 2022 23:38:19 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2b74f0baaaa931ffc46573874a7d7435b642d28f1f283104ac297499fba99f0a"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Mon, 18 Jul 2022 23:38:20 GMT
ENV YARN_VERSION=1.22.19
# Mon, 18 Jul 2022 23:38:24 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Mon, 18 Jul 2022 23:38:24 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Mon, 18 Jul 2022 23:38:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Jul 2022 23:38:24 GMT
CMD ["node"]
# Thu, 21 Jul 2022 00:10:37 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 21 Jul 2022 00:10:38 GMT
RUN apk add --no-cache 		bash
# Thu, 21 Jul 2022 00:10:38 GMT
ENV NODE_ENV=production
# Thu, 21 Jul 2022 00:10:38 GMT
ENV GHOST_CLI_VERSION=1.21.0
# Thu, 21 Jul 2022 00:11:01 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Thu, 21 Jul 2022 00:11:01 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Thu, 21 Jul 2022 00:11:02 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 21 Jul 2022 00:11:02 GMT
ENV GHOST_VERSION=5.4.1
# Thu, 21 Jul 2022 00:12:09 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 21 Jul 2022 00:12:10 GMT
WORKDIR /var/lib/ghost
# Thu, 21 Jul 2022 00:12:10 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 21 Jul 2022 00:12:11 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 21 Jul 2022 00:12:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jul 2022 00:12:11 GMT
EXPOSE 2368
# Thu, 21 Jul 2022 00:12:11 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ca4541bf43fa13f7c3ef511d8b0f1a156a738645582a3c7e27a7b3fdebf4e3`  
		Last Modified: Mon, 18 Jul 2022 23:41:53 GMT  
		Size: 35.7 MB (35680407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b831dd745300d07e75a46ae8805ad39a4164cf888686f4a45ed782a26fd0d50c`  
		Last Modified: Mon, 18 Jul 2022 23:41:48 GMT  
		Size: 2.3 MB (2342258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86937321b535acf01ac5d7f108ead204d1c6a71f9a1c4402e8317ece72d1f6c8`  
		Last Modified: Mon, 18 Jul 2022 23:41:47 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0592e73d6339c74418c4cd0dea38b3bb902de35e88e9efc25bea4f6a9099ab`  
		Last Modified: Thu, 21 Jul 2022 00:14:52 GMT  
		Size: 11.3 KB (11267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14249c905b1e66dd9a402ec7e12cd656f11280264f95df28d707b14e5080ecc0`  
		Last Modified: Thu, 21 Jul 2022 00:14:53 GMT  
		Size: 820.0 KB (820018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25efc1c96c74b0e8bbf3bb20de3a4f5a914a53d9bc04331565fde6e51546753`  
		Last Modified: Thu, 21 Jul 2022 00:14:56 GMT  
		Size: 10.6 MB (10551079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37534ac356524ddbd46a317babc1c4d360d08c4b2978a96002a86d9470ea1dff`  
		Last Modified: Thu, 21 Jul 2022 00:15:05 GMT  
		Size: 67.2 MB (67150803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d669cf821c038c65960ef43afa327bdfca48c9a2d317fce1a73f779bae4854fc`  
		Last Modified: Thu, 21 Jul 2022 00:14:52 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:9eb81db7aae6db7a4ca527c41ceb6295fd7e3c3eb3744efded5f36cdc2e7ea70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113548977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f6423687061b8b00de0d1aaa04598d64570293b8a0f86681c489db3754d0b2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 02:09:21 GMT
ENV NODE_VERSION=16.16.0
# Tue, 19 Jul 2022 02:30:54 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2b74f0baaaa931ffc46573874a7d7435b642d28f1f283104ac297499fba99f0a"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 19 Jul 2022 02:30:55 GMT
ENV YARN_VERSION=1.22.19
# Tue, 19 Jul 2022 02:31:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 19 Jul 2022 02:31:03 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 19 Jul 2022 02:31:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 02:31:04 GMT
CMD ["node"]
# Thu, 21 Jul 2022 00:35:00 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 21 Jul 2022 00:35:03 GMT
RUN apk add --no-cache 		bash
# Thu, 21 Jul 2022 00:35:03 GMT
ENV NODE_ENV=production
# Thu, 21 Jul 2022 00:35:04 GMT
ENV GHOST_CLI_VERSION=1.21.0
# Thu, 21 Jul 2022 00:36:54 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Thu, 21 Jul 2022 00:36:55 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Thu, 21 Jul 2022 00:36:56 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 21 Jul 2022 00:36:56 GMT
ENV GHOST_VERSION=5.4.1
# Thu, 21 Jul 2022 00:55:33 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 21 Jul 2022 00:55:36 GMT
WORKDIR /var/lib/ghost
# Thu, 21 Jul 2022 00:55:36 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 21 Jul 2022 00:55:37 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 21 Jul 2022 00:55:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jul 2022 00:55:38 GMT
EXPOSE 2368
# Thu, 21 Jul 2022 00:55:38 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6ddbf2a6697cb4cbf18a1ff99fd7ffdbd6b04259757aaa018b4451ed046a4d`  
		Last Modified: Tue, 19 Jul 2022 02:52:05 GMT  
		Size: 34.7 MB (34685508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415b0bfb324792ccaf7a06f374eac7e58d62a27b965bdd9b171a5b21defcf0f0`  
		Last Modified: Tue, 19 Jul 2022 02:51:45 GMT  
		Size: 2.4 MB (2422616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1b3d9e9bb6638038ac630c8bbb2ad62df46e59b7ff76bb1091718361fb89d6`  
		Last Modified: Tue, 19 Jul 2022 02:51:43 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec1cb6e78851d865871c3bcd097c4f11aa05ed8fcd9bfdc35a57092ae535e65`  
		Last Modified: Thu, 21 Jul 2022 01:08:24 GMT  
		Size: 11.0 KB (10960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39ca8d08b5426f44a24f87badcf55453c7db3243a22cb47c922a7bcbcee2a2f`  
		Last Modified: Thu, 21 Jul 2022 01:08:25 GMT  
		Size: 772.0 KB (771978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f81697ec96f1795cfc8480ce65ced2a27c81b1d693f443e4807b433361956f`  
		Last Modified: Thu, 21 Jul 2022 01:08:40 GMT  
		Size: 10.6 MB (10560834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c81e0b88abd873f004717b992f6b1cd235aca0e921d6fc25c68fa3b5261228`  
		Last Modified: Thu, 21 Jul 2022 01:09:32 GMT  
		Size: 62.5 MB (62489651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff5fa8149276747ffa4f99f7c038fb1e28bd46810975768551fcbde769672f0`  
		Last Modified: Thu, 21 Jul 2022 01:08:24 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:9379c61737b48677d3ea156d224622eb27594e04d9326ed7dced2bd5801e743b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112704939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0896eb3e4e5a9cfe842a92483948e9754e46abf03692aa0f26b68257a8a044`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Tue, 19 Jul 2022 22:57:50 GMT
ADD file:eb9518889a2987adfe1dfbeb786888817d6b767409b0102155094508f88b8798 in / 
# Tue, 19 Jul 2022 22:57:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 01:28:40 GMT
ENV NODE_VERSION=16.16.0
# Wed, 20 Jul 2022 01:56:57 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2b74f0baaaa931ffc46573874a7d7435b642d28f1f283104ac297499fba99f0a"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 20 Jul 2022 01:56:58 GMT
ENV YARN_VERSION=1.22.19
# Wed, 20 Jul 2022 01:57:09 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 20 Jul 2022 01:57:10 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 20 Jul 2022 01:57:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 01:57:12 GMT
CMD ["node"]
# Wed, 20 Jul 2022 10:47:14 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 20 Jul 2022 10:47:16 GMT
RUN apk add --no-cache 		bash
# Wed, 20 Jul 2022 10:47:17 GMT
ENV NODE_ENV=production
# Wed, 20 Jul 2022 10:47:17 GMT
ENV GHOST_CLI_VERSION=1.21.0
# Wed, 20 Jul 2022 10:48:07 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 20 Jul 2022 10:48:08 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 20 Jul 2022 10:48:09 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 20 Jul 2022 10:48:09 GMT
ENV GHOST_VERSION=5.3.1
# Wed, 20 Jul 2022 11:01:25 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 20 Jul 2022 11:01:28 GMT
WORKDIR /var/lib/ghost
# Wed, 20 Jul 2022 11:01:29 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 20 Jul 2022 11:01:29 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 20 Jul 2022 11:01:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 11:01:30 GMT
EXPOSE 2368
# Wed, 20 Jul 2022 11:01:30 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:4a43ec7a7388a66102a4ef9408174101a21dd2260a6deb956929f7eda8cde610`  
		Last Modified: Tue, 19 Jul 2022 22:59:36 GMT  
		Size: 2.4 MB (2424551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82802d9789e49b0eb4ed0f24c57598c90819c1c456b549e5ded65ce7d0a295c2`  
		Last Modified: Wed, 20 Jul 2022 02:28:02 GMT  
		Size: 34.2 MB (34156119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef950a69282a153519b64d6ad7037f890c160d7e92a34387dff4449d0945a0c`  
		Last Modified: Wed, 20 Jul 2022 02:27:42 GMT  
		Size: 2.4 MB (2422680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef43d3a0b5bcf0efca778ac8083173101fe94c64c2fbf1fb9d34c9dcaef2e129`  
		Last Modified: Wed, 20 Jul 2022 02:27:40 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bfe915614b1de2208eb3f45c9ee491c3c41d6f01f58ffe55d76357bdd25337`  
		Last Modified: Wed, 20 Jul 2022 11:11:40 GMT  
		Size: 10.8 KB (10789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca58d839a2c480db2210bbcbd57695d1378b33e689f8411d97876b7ce4099814`  
		Last Modified: Wed, 20 Jul 2022 11:11:40 GMT  
		Size: 705.0 KB (704980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c735179d354bc34a6884546e87a4e97d1b7e3c13a6a82b26d03468cdca2181d`  
		Last Modified: Wed, 20 Jul 2022 11:11:56 GMT  
		Size: 10.6 MB (10555403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4a7822e9dc4c3b9b27bfa711a2841428ea64435d2f9c8baaf958d4094771bd`  
		Last Modified: Wed, 20 Jul 2022 11:12:49 GMT  
		Size: 62.4 MB (62429422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c63ab3dd8ad51e44178be8081002ea8eeff46dc45a03a418e797e29c46b66f5`  
		Last Modified: Wed, 20 Jul 2022 11:11:40 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:f353d299174fd824900239784eafe731ff9bfec7f31f6a0a36fb40f6313f6eb4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126434795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3115e512c914a18a1261dec259c7d5bcd466fa67bc7b4e3f6472cb6c5da0e59b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:27:31 GMT
ENV NODE_VERSION=16.16.0
# Tue, 19 Jul 2022 00:57:44 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2b74f0baaaa931ffc46573874a7d7435b642d28f1f283104ac297499fba99f0a"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 19 Jul 2022 00:57:44 GMT
ENV YARN_VERSION=1.22.19
# Tue, 19 Jul 2022 00:57:51 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 19 Jul 2022 00:57:52 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 19 Jul 2022 00:57:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 00:57:53 GMT
CMD ["node"]
# Thu, 21 Jul 2022 01:00:32 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 21 Jul 2022 01:00:33 GMT
RUN apk add --no-cache 		bash
# Thu, 21 Jul 2022 01:00:33 GMT
ENV NODE_ENV=production
# Thu, 21 Jul 2022 01:00:34 GMT
ENV GHOST_CLI_VERSION=1.21.0
# Thu, 21 Jul 2022 01:00:57 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Thu, 21 Jul 2022 01:00:59 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Thu, 21 Jul 2022 01:00:59 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Thu, 21 Jul 2022 01:01:00 GMT
ENV GHOST_VERSION=5.4.1
# Thu, 21 Jul 2022 01:05:46 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db sqlite3 --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --ip '::' --port 2368 --no-prompt --db sqlite3 --url http://localhost:2368 --dbpath "$GHOST_CONTENT/data/ghost.db"; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Thu, 21 Jul 2022 01:05:50 GMT
WORKDIR /var/lib/ghost
# Thu, 21 Jul 2022 01:05:52 GMT
VOLUME [/var/lib/ghost/content]
# Thu, 21 Jul 2022 01:05:54 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Thu, 21 Jul 2022 01:05:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jul 2022 01:05:59 GMT
EXPOSE 2368
# Thu, 21 Jul 2022 01:06:02 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a0afc8369f735ffbdf898b1b4a7e3daaedf809448620eb8c4fd8cda53fd0f7`  
		Last Modified: Tue, 19 Jul 2022 01:24:32 GMT  
		Size: 35.6 MB (35609524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33bf715aa7027abf029587f99133f7d86d5cfb965b7e5270523a32b1aa66f95`  
		Last Modified: Tue, 19 Jul 2022 01:24:27 GMT  
		Size: 2.4 MB (2430026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197c33cbfa1ca36647b64839f4434532bcaee094c6a23949d8edc49ceadfd07a`  
		Last Modified: Tue, 19 Jul 2022 01:24:26 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ac713e99d42e74d1b5c27db8386164513493dedde4a58c1878b5d3b08a7e7d`  
		Last Modified: Thu, 21 Jul 2022 01:09:31 GMT  
		Size: 11.0 KB (10987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aaf0b42af78fecf7af819e4937c93e69a82a7a595595425df22fd61f1a8b76f`  
		Last Modified: Thu, 21 Jul 2022 01:09:31 GMT  
		Size: 826.1 KB (826074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a2026619c72abe7eeb006a3cb6332ac048acb799e06316b98167b2cf0ea8fe`  
		Last Modified: Thu, 21 Jul 2022 01:09:34 GMT  
		Size: 10.5 MB (10548011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c4d2fce880019c989298076bd83553f384f698b4f333a68974364ebcabb38`  
		Last Modified: Thu, 21 Jul 2022 01:09:45 GMT  
		Size: 74.3 MB (74314455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41e3f8cafb9bfcf1c3cd44d75ee3efc02b40f793ee80c031ebfb841d0efe163`  
		Last Modified: Thu, 21 Jul 2022 01:09:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
