## `ghost:5-alpine`

```console
$ docker pull ghost@sha256:7023d159f35250e85ea67727b3aee1c4de4a0d96c4eb96cc87ff24cf8657e735
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:5-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:68a3196cae6554fe56f005c89ab90e915514e6ed63867fbd71064c1443a1f1f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133645350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bec00e537978f2e3435248b67397702014201266bee29ddfec8849b5d1991c9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:22:08 GMT
ENV NODE_VERSION=16.20.0
# Sun, 04 Jun 2023 17:48:40 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="b3f80fe7d0f1af6fe25ffedc7237ca519965d08fc800eab29cf45cd5b90cdb26"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && export GNUPGHOME="$(mktemp -d)"     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sun, 04 Jun 2023 17:48:40 GMT
ENV YARN_VERSION=1.22.19
# Sun, 04 Jun 2023 17:48:44 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && export GNUPGHOME="$(mktemp -d)"   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sun, 04 Jun 2023 17:48:44 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sun, 04 Jun 2023 17:48:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 04 Jun 2023 17:48:44 GMT
CMD ["node"]
# Tue, 13 Jun 2023 02:45:59 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 13 Jun 2023 02:46:00 GMT
RUN apk add --no-cache 		bash
# Tue, 13 Jun 2023 02:46:00 GMT
ENV NODE_ENV=production
# Tue, 13 Jun 2023 02:46:01 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Tue, 13 Jun 2023 02:46:14 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 13 Jun 2023 02:46:15 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 13 Jun 2023 02:46:15 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 13 Jun 2023 02:46:15 GMT
ENV GHOST_VERSION=5.51.0
# Tue, 13 Jun 2023 02:47:30 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 13 Jun 2023 02:47:32 GMT
WORKDIR /var/lib/ghost
# Tue, 13 Jun 2023 02:47:32 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 13 Jun 2023 02:47:32 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 13 Jun 2023 02:47:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 02:47:32 GMT
EXPOSE 2368
# Tue, 13 Jun 2023 02:47:32 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e9712c615f1168b9fc215cc97a91c7c63e2ec432fab006f78bf3e78770b1ea`  
		Last Modified: Sun, 04 Jun 2023 17:52:51 GMT  
		Size: 36.6 MB (36627878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9369075e452c97fe488a12010b6791e6f008181992397f40a502fc7e2f9172a1`  
		Last Modified: Sun, 04 Jun 2023 17:52:46 GMT  
		Size: 2.3 MB (2338997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5f54542006a7e4763672407d46e0a89e37613b78a4f5bbc55d8d462e10d3ba`  
		Last Modified: Sun, 04 Jun 2023 17:52:46 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3e2d902203285b8b0bfde3571b1d7b4ed0152365633e057967d743c7457eab`  
		Last Modified: Tue, 13 Jun 2023 02:48:13 GMT  
		Size: 11.3 KB (11310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0cfea090726e400ca1e87402e0a050c8a3a791b5c594aa9ef29e8da3194b429`  
		Last Modified: Tue, 13 Jun 2023 02:48:13 GMT  
		Size: 857.7 KB (857729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1a24e82f5404557649f54e2f2f00084cf7dbc92cc1d3723d3519a8f75c24ca`  
		Last Modified: Tue, 13 Jun 2023 02:48:16 GMT  
		Size: 10.3 MB (10280568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00587308baa69f5cd7ae0ae9ec2b6a8425dee1d35f395f00aba3c92a35cd823d`  
		Last Modified: Tue, 13 Jun 2023 02:48:27 GMT  
		Size: 80.2 MB (80153307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d327132c5eb945e272548d435c2240c530ac4bcb782ca3dfdec9a2f0c1cd85`  
		Last Modified: Tue, 13 Jun 2023 02:48:13 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:4a2f057a265fa140a0b55b8d10c150f1acd8a47968f859fd8f6af826867741c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128013135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b78dcc6ea5de7ed2054c19dcf4492ac5a5d44db8d0b7932db38c2e4793a5deb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:17:59 GMT
ENV NODE_VERSION=16.20.0
# Sat, 03 Jun 2023 04:50:46 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="b3f80fe7d0f1af6fe25ffedc7237ca519965d08fc800eab29cf45cd5b90cdb26"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && export GNUPGHOME="$(mktemp -d)"     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 03 Jun 2023 04:50:46 GMT
ENV YARN_VERSION=1.22.19
# Sat, 03 Jun 2023 04:50:51 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && export GNUPGHOME="$(mktemp -d)"   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 03 Jun 2023 04:50:52 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 03 Jun 2023 04:50:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Jun 2023 04:50:52 GMT
CMD ["node"]
# Mon, 12 Jun 2023 22:49:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 12 Jun 2023 22:49:14 GMT
RUN apk add --no-cache 		bash
# Mon, 12 Jun 2023 22:49:14 GMT
ENV NODE_ENV=production
# Mon, 12 Jun 2023 22:49:15 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Mon, 12 Jun 2023 22:49:48 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Mon, 12 Jun 2023 22:49:49 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Mon, 12 Jun 2023 22:49:49 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 12 Jun 2023 22:49:49 GMT
ENV GHOST_VERSION=5.51.0
# Mon, 12 Jun 2023 22:57:52 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 12 Jun 2023 22:57:56 GMT
WORKDIR /var/lib/ghost
# Mon, 12 Jun 2023 22:57:56 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 12 Jun 2023 22:57:56 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 12 Jun 2023 22:57:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jun 2023 22:57:56 GMT
EXPOSE 2368
# Mon, 12 Jun 2023 22:57:57 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ccfbcc05d314ae70f0b8daf2e6888dcf962dbc441f4414bd43806cc8b21fc0`  
		Last Modified: Sat, 03 Jun 2023 05:15:37 GMT  
		Size: 35.9 MB (35855324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aededbba24dd5c70f4002c5dbdd49ed582ca47e5c5e6a6cd0bbc857edb31ba0`  
		Last Modified: Sat, 03 Jun 2023 05:15:32 GMT  
		Size: 2.3 MB (2329785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8e268f9c73b12c7fb952957c9e6ff7d530735f5b28858bc14776c1ba6b9717`  
		Last Modified: Sat, 03 Jun 2023 05:15:31 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc6d381a17fa0d625c109937180702c9af1d19f6dad36c7e9df496872ee846b`  
		Last Modified: Mon, 12 Jun 2023 22:58:11 GMT  
		Size: 11.5 KB (11505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a5d9c99d06f97207597bdef22641d17a89c4f04b451785dd7e338551406565`  
		Last Modified: Mon, 12 Jun 2023 22:58:11 GMT  
		Size: 852.1 KB (852101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceba81a43bb716d53ff58be1ac9c1b49297a6b73d2e98042ef3425c7e5edbde8`  
		Last Modified: Mon, 12 Jun 2023 22:58:15 GMT  
		Size: 10.3 MB (10284615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74986150ee3995f1d6457501b19a69023c893bcdc94bc218e29ad2d33763ce2c`  
		Last Modified: Mon, 12 Jun 2023 22:58:31 GMT  
		Size: 75.6 MB (75568005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b89f320f258989fc707306f4510e799dede67050e3119486e2dd31bed87db6`  
		Last Modified: Mon, 12 Jun 2023 22:58:11 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:3ae6fd52d98bb1965704ecbffe81318b9df18e1f334c2501e390ad345042526f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (126972295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a353aa932fd3863069463019694112608831415bce42efe3f26feaf017e2ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 08:28:40 GMT
ENV NODE_VERSION=16.20.0
# Sat, 03 Jun 2023 04:14:25 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="b3f80fe7d0f1af6fe25ffedc7237ca519965d08fc800eab29cf45cd5b90cdb26"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && export GNUPGHOME="$(mktemp -d)"     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 03 Jun 2023 04:14:25 GMT
ENV YARN_VERSION=1.22.19
# Sat, 03 Jun 2023 04:14:29 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && export GNUPGHOME="$(mktemp -d)"   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 03 Jun 2023 04:14:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 03 Jun 2023 04:14:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Jun 2023 04:14:30 GMT
CMD ["node"]
# Mon, 12 Jun 2023 23:02:17 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Mon, 12 Jun 2023 23:02:18 GMT
RUN apk add --no-cache 		bash
# Mon, 12 Jun 2023 23:02:18 GMT
ENV NODE_ENV=production
# Mon, 12 Jun 2023 23:02:18 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Mon, 12 Jun 2023 23:02:33 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Mon, 12 Jun 2023 23:02:34 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Mon, 12 Jun 2023 23:02:34 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Mon, 12 Jun 2023 23:02:34 GMT
ENV GHOST_VERSION=5.51.0
# Mon, 12 Jun 2023 23:08:33 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Mon, 12 Jun 2023 23:08:36 GMT
WORKDIR /var/lib/ghost
# Mon, 12 Jun 2023 23:08:36 GMT
VOLUME [/var/lib/ghost/content]
# Mon, 12 Jun 2023 23:08:36 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Mon, 12 Jun 2023 23:08:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jun 2023 23:08:36 GMT
EXPOSE 2368
# Mon, 12 Jun 2023 23:08:36 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97634c24989fb297386c547ffc01689ee8b91b4051e218fcf72345fc8189d6df`  
		Last Modified: Sat, 03 Jun 2023 04:55:40 GMT  
		Size: 35.4 MB (35387252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d77ab2ab80b1609b70da046f1d97b3c18e3a936a0efeb0abb3c8a66392d5cb`  
		Last Modified: Sat, 03 Jun 2023 04:55:34 GMT  
		Size: 2.3 MB (2329647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6255d0bdabe00d79fd09af04fc1ae2de2ac7d0e0b868ccc793003487b98532b3`  
		Last Modified: Sat, 03 Jun 2023 04:55:33 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a311a964b7f3f2a5995e345ddd6998a2e36176e4249615563a113d257d22a1`  
		Last Modified: Mon, 12 Jun 2023 23:09:22 GMT  
		Size: 11.3 KB (11311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a4e21e788d5228d151fdbabf5d198f8543922ccb888b4ea8c85d49cdad5fac`  
		Last Modified: Mon, 12 Jun 2023 23:09:22 GMT  
		Size: 781.9 KB (781888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23f3e42a8a11eb2e1dd500345a5e9cf8f63d37a71a149b389d99ad264ed9481`  
		Last Modified: Mon, 12 Jun 2023 23:09:25 GMT  
		Size: 10.3 MB (10280520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9615e58772a782df9f530d9c3a5171c97e64a488cf67dc069e7d8ae7dd402c`  
		Last Modified: Mon, 12 Jun 2023 23:09:41 GMT  
		Size: 75.3 MB (75312165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15bea9e72cee3b10dd41198095df70cab409e618bbca344760f58778de5bfeac`  
		Last Modified: Mon, 12 Jun 2023 23:09:21 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:4430630ec7786c928c13b1e07c3dbfdbd9c812e247e10929464d92dfd0fef5f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.0 MB (141022131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ebc9a0ff286f127d6b404230b2a2b769cb5f84f337d8f254e19b6fe10ef5246`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 08:19:47 GMT
ENV NODE_VERSION=16.20.0
# Sat, 03 Jun 2023 02:27:01 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="b3f80fe7d0f1af6fe25ffedc7237ca519965d08fc800eab29cf45cd5b90cdb26"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && export GNUPGHOME="$(mktemp -d)"     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       DD792F5973C6DE52C432CBDAC77ABFA00DDBF2B7       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && gpgconf --kill all     && rm -rf "$GNUPGHOME"     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 03 Jun 2023 02:27:01 GMT
ENV YARN_VERSION=1.22.19
# Sat, 03 Jun 2023 02:27:06 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && export GNUPGHOME="$(mktemp -d)"   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && gpgconf --kill all   && rm -rf "$GNUPGHOME"   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 03 Jun 2023 02:27:06 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 03 Jun 2023 02:27:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 03 Jun 2023 02:27:06 GMT
CMD ["node"]
# Tue, 13 Jun 2023 02:15:00 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 13 Jun 2023 02:15:01 GMT
RUN apk add --no-cache 		bash
# Tue, 13 Jun 2023 02:15:01 GMT
ENV NODE_ENV=production
# Tue, 13 Jun 2023 02:15:01 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Tue, 13 Jun 2023 02:15:13 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 13 Jun 2023 02:15:14 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 13 Jun 2023 02:15:14 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Tue, 13 Jun 2023 02:15:14 GMT
ENV GHOST_VERSION=5.51.0
# Tue, 13 Jun 2023 02:18:49 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Tue, 13 Jun 2023 02:18:54 GMT
WORKDIR /var/lib/ghost
# Tue, 13 Jun 2023 02:18:54 GMT
VOLUME [/var/lib/ghost/content]
# Tue, 13 Jun 2023 02:18:54 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Tue, 13 Jun 2023 02:18:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Jun 2023 02:18:54 GMT
EXPOSE 2368
# Tue, 13 Jun 2023 02:18:54 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89417138b4716ae68d35883e0ea94457b769193b81b202ad41125d00b232361`  
		Last Modified: Sat, 03 Jun 2023 02:48:39 GMT  
		Size: 36.9 MB (36854860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0195fdd52282a266be9dcb5a16d73d9fe54ec25cb88a6bebc199764617b2f2`  
		Last Modified: Sat, 03 Jun 2023 02:48:37 GMT  
		Size: 2.3 MB (2339109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a41b50fd48ec27b9ddff95d86cf5dbf4077000b95452123da9a16657e6460e`  
		Last Modified: Sat, 03 Jun 2023 02:48:37 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba871a2f15ad40a2e7f122b8bb16c57b6274bb475453a410b49efca764c7794`  
		Last Modified: Tue, 13 Jun 2023 02:19:40 GMT  
		Size: 11.6 KB (11563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6ae8d4627d843009ad0c12190c8f7d1bef0e13115214190236b71b258ccdb1`  
		Last Modified: Tue, 13 Jun 2023 02:19:41 GMT  
		Size: 901.8 KB (901773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1db4affd7a6d3a46638987d8754f5f2f1be97e69279d0924e5b78cf132a6508`  
		Last Modified: Tue, 13 Jun 2023 02:19:43 GMT  
		Size: 10.3 MB (10279852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4074041a7a761853d965725e8c2e5973c2facf6ef32e9f6f18969144e727fc`  
		Last Modified: Tue, 13 Jun 2023 02:19:53 GMT  
		Size: 87.4 MB (87372124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0415becb9b35ffb1cc19ccf42fe004f4e613587727f238bd7a7ac99ee9d701`  
		Last Modified: Tue, 13 Jun 2023 02:19:40 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
