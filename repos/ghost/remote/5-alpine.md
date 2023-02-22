## `ghost:5-alpine`

```console
$ docker pull ghost@sha256:59bb6dfb8d51e7e1a874d238e341c1d7de1c32b9dd40b9f5ca2ab7e54e0c80b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:5-alpine` - linux; amd64

```console
$ docker pull ghost@sha256:0dddf8b6a34693ff35459f3c808de938b9939b2c63cb09b59363496c8c13b5d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140119019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f43dbced0b845febf564d1b7197da1d14aa8fb1d2881b83391c46d3d0226f44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Fri, 17 Feb 2023 18:25:42 GMT
ENV NODE_VERSION=16.19.1
# Tue, 21 Feb 2023 22:13:33 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="f701dbe93da8be3198d3b6a2ba0044c2f5d142b3acabefb7a3ffeb31245b88df"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 21 Feb 2023 22:13:33 GMT
ENV YARN_VERSION=1.22.19
# Tue, 21 Feb 2023 22:13:38 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 21 Feb 2023 22:13:38 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 21 Feb 2023 22:13:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Feb 2023 22:13:38 GMT
CMD ["node"]
# Tue, 21 Feb 2023 22:34:13 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 21 Feb 2023 22:34:14 GMT
RUN apk add --no-cache 		bash
# Tue, 21 Feb 2023 22:34:14 GMT
ENV NODE_ENV=production
# Tue, 21 Feb 2023 22:34:14 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Tue, 21 Feb 2023 22:34:28 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 21 Feb 2023 22:34:28 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 21 Feb 2023 22:34:29 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 22 Feb 2023 01:25:53 GMT
ENV GHOST_VERSION=5.35.1
# Wed, 22 Feb 2023 01:27:34 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 22 Feb 2023 01:27:38 GMT
WORKDIR /var/lib/ghost
# Wed, 22 Feb 2023 01:27:38 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 22 Feb 2023 01:27:38 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 22 Feb 2023 01:27:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 01:27:38 GMT
EXPOSE 2368
# Wed, 22 Feb 2023 01:27:38 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60192c892f5335138788064bbf95055259110306c6e7633eed5b68d6128fcb23`  
		Last Modified: Tue, 21 Feb 2023 22:17:46 GMT  
		Size: 36.5 MB (36505387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6dfec7e39fb14821c67873311ab85ba8a7cf6053907af8c53d8da91e560761c`  
		Last Modified: Tue, 21 Feb 2023 22:17:41 GMT  
		Size: 2.4 MB (2351132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08a1a042cb99aa66f9cbf34819582d4925b14e1ed8b85b6af7a86327eb5d2dd`  
		Last Modified: Tue, 21 Feb 2023 22:17:41 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3acec299f3bb9cdc9c9fef18398314d73f733bc6f7f08573f29cfb6a6ff983`  
		Last Modified: Tue, 21 Feb 2023 22:36:39 GMT  
		Size: 11.3 KB (11296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa9632467283cc6dc574b96c11260b01cae3986a120fdf40aa0b5f6884fc05b`  
		Last Modified: Tue, 21 Feb 2023 22:36:40 GMT  
		Size: 820.1 KB (820063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9d58f71c0669a95d7c71ff6fac7e2a74f26afabb30566b2a76e115234cd22f`  
		Last Modified: Tue, 21 Feb 2023 22:36:42 GMT  
		Size: 10.2 MB (10225768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231bcedb7fa2f5160a972a0cb86f4ce960cbc46466afd83067037d720668f343`  
		Last Modified: Wed, 22 Feb 2023 01:28:54 GMT  
		Size: 87.4 MB (87396616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258bbcc43bfb5998eaed274f2424976318af50ead6c5c7e1565f4ae3b8a0f0eb`  
		Last Modified: Wed, 22 Feb 2023 01:28:36 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5-alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:0a241d0fc8b3fea9a9bc27e6a27a2962b6b64af1b850a6fe2348a357b572889c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.2 MB (134234590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a62c13f2716ca1f984363c08b01e349dff3897064f3d16c2a4df810533ca820`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Fri, 17 Feb 2023 23:04:55 GMT
ENV NODE_VERSION=16.19.1
# Tue, 21 Feb 2023 23:19:38 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="f701dbe93da8be3198d3b6a2ba0044c2f5d142b3acabefb7a3ffeb31245b88df"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 21 Feb 2023 23:19:39 GMT
ENV YARN_VERSION=1.22.19
# Tue, 21 Feb 2023 23:19:44 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 21 Feb 2023 23:19:45 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 21 Feb 2023 23:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Feb 2023 23:19:45 GMT
CMD ["node"]
# Wed, 22 Feb 2023 00:13:28 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Wed, 22 Feb 2023 00:13:29 GMT
RUN apk add --no-cache 		bash
# Wed, 22 Feb 2023 00:13:30 GMT
ENV NODE_ENV=production
# Wed, 22 Feb 2023 00:13:30 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Wed, 22 Feb 2023 00:14:13 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Wed, 22 Feb 2023 00:14:14 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Wed, 22 Feb 2023 00:14:14 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 22 Feb 2023 01:49:32 GMT
ENV GHOST_VERSION=5.35.1
# Wed, 22 Feb 2023 02:01:36 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 22 Feb 2023 02:01:40 GMT
WORKDIR /var/lib/ghost
# Wed, 22 Feb 2023 02:01:40 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 22 Feb 2023 02:01:41 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 22 Feb 2023 02:01:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 02:01:42 GMT
EXPOSE 2368
# Wed, 22 Feb 2023 02:01:42 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871903e765d7cc7e62ceb51e0aea219a4e007458cc9cc2bf13e35503fc97be5e`  
		Last Modified: Tue, 21 Feb 2023 23:57:05 GMT  
		Size: 35.4 MB (35431987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3245edf4a9750306064f5c16f260b59036d6fec4bb046a5ea650e81bab6eec`  
		Last Modified: Tue, 21 Feb 2023 23:56:58 GMT  
		Size: 2.4 MB (2399867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553320185b75107d46f7669d37fe4a990f84b6810604b975b449c030830d0fab`  
		Last Modified: Tue, 21 Feb 2023 23:56:58 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be81989faf7aa2c489231dd741c70025e57e7acb6ae439c50e05706df06c114d`  
		Last Modified: Wed, 22 Feb 2023 00:27:11 GMT  
		Size: 11.0 KB (10995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf2fc83c63dc96abe7e61302f07241ee7cb2cf4f9767e74b5858a03eed95111`  
		Last Modified: Wed, 22 Feb 2023 00:27:12 GMT  
		Size: 772.0 KB (771957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac986a1fee9e4684f1ac27e07c2e38cad7b10dec4b226b7c595617ec3d249bb4`  
		Last Modified: Wed, 22 Feb 2023 00:27:17 GMT  
		Size: 10.2 MB (10239169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567be68942fc07349699e1acad78578c6ec124a13a635ea4df898ee272c52bc4`  
		Last Modified: Wed, 22 Feb 2023 02:02:49 GMT  
		Size: 82.8 MB (82762844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8250b85bfcb15f70a1113f573f219aa259bbc4de9e49ac733c60cb6f547d01f5`  
		Last Modified: Wed, 22 Feb 2023 02:02:19 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5-alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:a0600cdb0a365a4375c49a5d48a242ae9ba0361cdc5c6b03872e7894660dc967
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.3 MB (133253290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f18eea9bb027781a0eca722b561cb9bc4aa06b7039a2932519cd8954ae5e52d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 17 Feb 2023 21:19:53 GMT
ENV NODE_VERSION=16.19.1
# Fri, 17 Feb 2023 22:17:33 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="8f14f84b7011f468e06affe9102b57140452078510c43f86feb2b7266b516b28"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 17 Feb 2023 22:17:34 GMT
ENV YARN_VERSION=1.22.19
# Fri, 17 Feb 2023 22:17:40 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 17 Feb 2023 22:17:40 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 17 Feb 2023 22:17:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Feb 2023 22:17:41 GMT
CMD ["node"]
# Sat, 18 Feb 2023 01:09:16 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Sat, 18 Feb 2023 01:09:18 GMT
RUN apk add --no-cache 		bash
# Sat, 18 Feb 2023 01:09:18 GMT
ENV NODE_ENV=production
# Sat, 18 Feb 2023 01:09:19 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Sat, 18 Feb 2023 01:09:45 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Sat, 18 Feb 2023 01:09:47 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Sat, 18 Feb 2023 01:09:47 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 18 Feb 2023 01:09:47 GMT
ENV GHOST_VERSION=5.35.0
# Sat, 18 Feb 2023 01:18:40 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 18 Feb 2023 01:18:45 GMT
WORKDIR /var/lib/ghost
# Sat, 18 Feb 2023 01:18:45 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 18 Feb 2023 01:18:45 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 18 Feb 2023 01:18:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Feb 2023 01:18:45 GMT
EXPOSE 2368
# Sat, 18 Feb 2023 01:18:46 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cd4db2335cc4146c69b432639b0bd8d08200588bc20c4d37efab28f42f4001`  
		Last Modified: Sat, 18 Feb 2023 00:31:49 GMT  
		Size: 35.0 MB (34976283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5fa161d4678a898676b050ba4bde3a0713611193dc042c8b5a3ec620e4a906`  
		Last Modified: Sat, 18 Feb 2023 00:31:42 GMT  
		Size: 2.4 MB (2399843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf365dc814386c09b9935229b2c7c04ffd944715fca6a2c4991bc50a8d042231`  
		Last Modified: Sat, 18 Feb 2023 00:31:41 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2ebb5c01d7825a031e30491128816f58130cceefe1715cedd0f5941b766a00`  
		Last Modified: Sat, 18 Feb 2023 01:31:15 GMT  
		Size: 10.8 KB (10769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f9bf4c1bf5504ebee8ecd947371a5be2956d003f5667d22853ba3789e05b1d`  
		Last Modified: Sat, 18 Feb 2023 01:31:15 GMT  
		Size: 704.6 KB (704635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f75ed8446bebb56d2fd6c5c2f7c52924636ce5e33aacb5e02f90773890f524`  
		Last Modified: Sat, 18 Feb 2023 01:31:19 GMT  
		Size: 10.2 MB (10231428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f72a2750ca7bb11a872fd7cb639067c9d8be773ebcb1b9065b2928e7f862f0`  
		Last Modified: Sat, 18 Feb 2023 01:31:43 GMT  
		Size: 82.5 MB (82508841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189346697253629f8f8c38b579cfc011760d51d468a4f01bed42e5cd925cb03f`  
		Last Modified: Sat, 18 Feb 2023 01:31:15 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:5-alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:62f561904877fdebfc7750631770a0a205dcbe3c3a4633995fc1d942d58f1e6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.2 MB (147183398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02787ba72ee631eb36b23b9408ab65360967a710cf9936674ceda074e42402f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 17 Feb 2023 20:31:17 GMT
ENV NODE_VERSION=16.19.1
# Tue, 21 Feb 2023 22:46:53 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="f701dbe93da8be3198d3b6a2ba0044c2f5d142b3acabefb7a3ffeb31245b88df"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 21 Feb 2023 22:46:53 GMT
ENV YARN_VERSION=1.22.19
# Tue, 21 Feb 2023 22:46:58 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 21 Feb 2023 22:46:58 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 21 Feb 2023 22:46:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Feb 2023 22:46:58 GMT
CMD ["node"]
# Tue, 21 Feb 2023 23:26:00 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 21 Feb 2023 23:26:01 GMT
RUN apk add --no-cache 		bash
# Tue, 21 Feb 2023 23:26:01 GMT
ENV NODE_ENV=production
# Tue, 21 Feb 2023 23:26:01 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Tue, 21 Feb 2023 23:26:13 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 21 Feb 2023 23:26:14 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 21 Feb 2023 23:26:14 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Wed, 22 Feb 2023 01:47:00 GMT
ENV GHOST_VERSION=5.35.1
# Wed, 22 Feb 2023 01:51:31 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Wed, 22 Feb 2023 01:51:37 GMT
WORKDIR /var/lib/ghost
# Wed, 22 Feb 2023 01:51:37 GMT
VOLUME [/var/lib/ghost/content]
# Wed, 22 Feb 2023 01:51:37 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Wed, 22 Feb 2023 01:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 01:51:38 GMT
EXPOSE 2368
# Wed, 22 Feb 2023 01:51:38 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49019cb02c310e8315ffee66fc0e8bb235558c4edfa0e733d48111ef9080b329`  
		Last Modified: Tue, 21 Feb 2023 23:09:44 GMT  
		Size: 36.4 MB (36376745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b2d160ac03ee059cb95627f3bcdc635dc3a1fd5bac316c4d1c4778b6d886f4`  
		Last Modified: Tue, 21 Feb 2023 23:09:40 GMT  
		Size: 2.4 MB (2409364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08119d77b2643327eae47f8761f42acb81c1a792987b258550766f870f182d1`  
		Last Modified: Tue, 21 Feb 2023 23:09:39 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7aca67d05887bd656f12755191ca7d3e5e8b403ec864c42de139260f68e1e7`  
		Last Modified: Tue, 21 Feb 2023 23:31:28 GMT  
		Size: 11.1 KB (11107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7206be427dc6bbba71f39a1c8f198343b09110e78232b2f4bd9525ea915b0d`  
		Last Modified: Tue, 21 Feb 2023 23:31:28 GMT  
		Size: 826.3 KB (826341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca8df833722573334a3485fa809f6c112a3955f3702616e6ab800c7b66f4ab21`  
		Last Modified: Tue, 21 Feb 2023 23:31:30 GMT  
		Size: 10.2 MB (10224759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10198d262c988ab800397b959db6c72d4eb34be03d738b23c165dd76bb92b669`  
		Last Modified: Wed, 22 Feb 2023 01:52:58 GMT  
		Size: 94.6 MB (94624589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04cc50f4938ac6490c1e6d8f008b96e253fe5701757c245aaa3d17e4dda7a4`  
		Last Modified: Wed, 22 Feb 2023 01:52:43 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
