## `ghost:alpine`

```console
$ docker pull ghost@sha256:d43e395b085f85888b8e627a71a3568003048b4822bcad07f6fd528fa3b354fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `ghost:alpine` - linux; amd64

```console
$ docker pull ghost@sha256:b775ac089de16624ccfe426a8b62730612fcadc52f927e1e1dc6c813d91cb50f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.6 MB (143608185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993d30c3e21c74dcfdf543be7b6955e6881e37b79c86685e0b675c4167b34e0c`
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
# Sat, 25 Mar 2023 00:47:44 GMT
ENV GHOST_VERSION=5.40.1
# Sat, 25 Mar 2023 00:49:24 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 25 Mar 2023 00:49:28 GMT
WORKDIR /var/lib/ghost
# Sat, 25 Mar 2023 00:49:28 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 25 Mar 2023 00:49:28 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 25 Mar 2023 00:49:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:49:28 GMT
EXPOSE 2368
# Sat, 25 Mar 2023 00:49:28 GMT
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
	-	`sha256:67d1ebaa654adf48d9c1f072ea0ee4c6277180808bfe95c1f7e3985a3b0cfac1`  
		Last Modified: Sat, 25 Mar 2023 00:50:39 GMT  
		Size: 90.9 MB (90885778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c56e52fa0df7d22a42e08c1899f5dea82414567c25de39086f07d47a0028fda`  
		Last Modified: Sat, 25 Mar 2023 00:50:22 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v6

```console
$ docker pull ghost@sha256:23cf100b808f5c6b996139e9b31b09f9564c05e76790d7705342f95f69e66516
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.9 MB (142887444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4f3adcee57932cdd452e3ff5d026fed11de62b3644a5aff494eef20f7d1e2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 19:31:52 GMT
ENV NODE_VERSION=16.19.1
# Mon, 13 Mar 2023 19:55:37 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="f701dbe93da8be3198d3b6a2ba0044c2f5d142b3acabefb7a3ffeb31245b88df"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Mon, 13 Mar 2023 19:55:38 GMT
ENV YARN_VERSION=1.22.19
# Mon, 13 Mar 2023 19:55:44 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Mon, 13 Mar 2023 19:55:44 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Mon, 13 Mar 2023 19:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Mar 2023 19:55:44 GMT
CMD ["node"]
# Tue, 14 Mar 2023 01:51:45 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Tue, 14 Mar 2023 01:51:46 GMT
RUN apk add --no-cache 		bash
# Tue, 14 Mar 2023 01:51:46 GMT
ENV NODE_ENV=production
# Tue, 14 Mar 2023 01:51:46 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Tue, 14 Mar 2023 01:52:19 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Tue, 14 Mar 2023 01:52:19 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Tue, 14 Mar 2023 01:52:19 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 25 Mar 2023 02:18:06 GMT
ENV GHOST_VERSION=5.40.1
# Sat, 25 Mar 2023 02:28:12 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 25 Mar 2023 02:28:16 GMT
WORKDIR /var/lib/ghost
# Sat, 25 Mar 2023 02:28:16 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 25 Mar 2023 02:28:17 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 25 Mar 2023 02:28:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Mar 2023 02:28:17 GMT
EXPOSE 2368
# Sat, 25 Mar 2023 02:28:17 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4e53885b26440a752bfdba2636b88d5809ff27fb16644111a296ebb4513e99`  
		Last Modified: Mon, 13 Mar 2023 20:52:36 GMT  
		Size: 35.4 MB (35444013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f01079626421c0cf60800fdfe9120052540f6639cb57fe8cb37383141ae080`  
		Last Modified: Mon, 13 Mar 2023 20:52:30 GMT  
		Size: 2.4 MB (2401340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c38784fe5e951049cf96c9b1b53b42779f4ead277404e2be0e8f09625fcda1`  
		Last Modified: Mon, 13 Mar 2023 20:52:30 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7747d342d624f1bfcf793adae14344f44db78c5378dfa2140159e0b7cfb33a57`  
		Last Modified: Tue, 14 Mar 2023 02:09:26 GMT  
		Size: 11.0 KB (10996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761483b8dfbfcab986eb8bbe8ae2fa78904ab8d678ef0e6820cff116a608e3aa`  
		Last Modified: Tue, 14 Mar 2023 02:09:26 GMT  
		Size: 772.0 KB (772027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45238a9c6662da4e79caaa07ae842108f9d02ecfd50b0be0e5ae75447dc0d1c8`  
		Last Modified: Tue, 14 Mar 2023 02:09:31 GMT  
		Size: 10.3 MB (10252808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1900ce64c22d345002acb64a3e0811b2c138e1961f7649c6a62be099a1fad7d`  
		Last Modified: Sat, 25 Mar 2023 02:30:25 GMT  
		Size: 91.4 MB (91388486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5873a3e1d0f69775bd04f8fa8b1c0bc3052af548aab78cb2e8c6088fa92b755`  
		Last Modified: Sat, 25 Mar 2023 02:30:01 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm variant v7

```console
$ docker pull ghost@sha256:1134332de3fb3da792d426e9e394d2bea6b82f1e12fe8f5f05f1fda54f5f54fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141609941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a92ca9d715959ff031db3805c00ff8388dfcec10738897649bf0b8438dc6c752`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","current\/index.js"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 19:24:37 GMT
ENV NODE_VERSION=16.19.1
# Wed, 01 Mar 2023 19:48:01 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="f701dbe93da8be3198d3b6a2ba0044c2f5d142b3acabefb7a3ffeb31245b88df"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python3     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       74F12602B6F1C4E913FAA37AD3A89613643B6201       61FC681DFB92A079F1685E77973F295594EC4689       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       890C08DB8579162FEE0DF9DB8BEAB4DFCF555EF4       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       108F52B48DB57BB0CC439B2997B01419BD92F80A     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 01 Mar 2023 19:48:02 GMT
ENV YARN_VERSION=1.22.19
# Wed, 01 Mar 2023 19:48:07 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 01 Mar 2023 19:48:07 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 01 Mar 2023 19:48:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 19:48:07 GMT
CMD ["node"]
# Thu, 02 Mar 2023 06:26:50 GMT
RUN apk add --no-cache 'su-exec>=0.2'
# Thu, 02 Mar 2023 06:26:51 GMT
RUN apk add --no-cache 		bash
# Thu, 02 Mar 2023 06:26:51 GMT
ENV NODE_ENV=production
# Thu, 02 Mar 2023 06:26:51 GMT
ENV GHOST_CLI_VERSION=1.24.0
# Thu, 02 Mar 2023 06:27:06 GMT
RUN set -eux; 	npm install -g "ghost-cli@$GHOST_CLI_VERSION"; 	npm cache clean --force
# Thu, 02 Mar 2023 06:27:06 GMT
ENV GHOST_INSTALL=/var/lib/ghost
# Thu, 02 Mar 2023 06:27:06 GMT
ENV GHOST_CONTENT=/var/lib/ghost/content
# Sat, 25 Mar 2023 05:46:46 GMT
ENV GHOST_VERSION=5.40.1
# Sat, 25 Mar 2023 05:54:21 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 25 Mar 2023 05:54:25 GMT
WORKDIR /var/lib/ghost
# Sat, 25 Mar 2023 05:54:26 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 25 Mar 2023 05:54:26 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 25 Mar 2023 05:54:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Mar 2023 05:54:26 GMT
EXPOSE 2368
# Sat, 25 Mar 2023 05:54:26 GMT
CMD ["node" "current/index.js"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f11fe3e54c5e2768c2dd1dc0efb44258fe82c5882e69e433a82bbe2897d5ba`  
		Last Modified: Wed, 01 Mar 2023 20:53:48 GMT  
		Size: 35.0 MB (34983292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f586ee1450c37a484a9318164b2361ab1fbbe31e063cd63286b8dd19359833b1`  
		Last Modified: Wed, 01 Mar 2023 20:53:42 GMT  
		Size: 2.4 MB (2399972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267d903c7e1832e8e79a8bfb9f009abcedcd7d470392750b24578401a0a95c43`  
		Last Modified: Wed, 01 Mar 2023 20:53:42 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2df68d2fd77199820c8d074508f7b491d2ae326627017a28f09cd414668bf1`  
		Last Modified: Thu, 02 Mar 2023 06:45:20 GMT  
		Size: 10.8 KB (10777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2261c9e63d51620149d35175db87a1d4589a96f82e89c8e30f33dadaa423f0`  
		Last Modified: Thu, 02 Mar 2023 06:45:20 GMT  
		Size: 704.7 KB (704689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92b8230fc5cecfcdb8e2e9cbb5953f111fedff2f9c4f64c6a13e225095b7b6d`  
		Last Modified: Thu, 02 Mar 2023 06:45:26 GMT  
		Size: 10.2 MB (10244072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9116bf64f2ebb93dba7de6ea010a848a9c3eed8dfafeee3fef89f0edf73b3d26`  
		Last Modified: Sat, 25 Mar 2023 05:56:01 GMT  
		Size: 90.8 MB (90845649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5c0af7640b10797c2a84dc9248a6a673fb8b3595b0b67b479ff0ddf757a969`  
		Last Modified: Sat, 25 Mar 2023 05:55:38 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ghost:alpine` - linux; arm64 variant v8

```console
$ docker pull ghost@sha256:cdbe4378e500f26abda29e1ca6bbc5223bba9a4cf17bbb7c4bf20b1d7e0bb683
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.7 MB (150667278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5489bf7e57c93694769372bf20b77c40d8cddb1a717ba447f0d6988e23b4ba1`
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
# Sat, 25 Mar 2023 01:14:27 GMT
ENV GHOST_VERSION=5.40.1
# Sat, 25 Mar 2023 01:18:57 GMT
RUN set -eux; 	mkdir -p "$GHOST_INSTALL"; 	chown node:node "$GHOST_INSTALL"; 		apkDel=; 		installCmd='su-exec node ghost install "$GHOST_VERSION" --db mysql --dbhost mysql --no-prompt --no-stack --no-setup --dir "$GHOST_INSTALL"'; 	if ! eval "$installCmd"; then 		virtual='.build-deps-ghost'; 		apkDel="$apkDel $virtual"; 		apk add --no-cache --virtual "$virtual" g++ make python3; 		eval "$installCmd"; 	fi; 		cd "$GHOST_INSTALL"; 	su-exec node ghost config --no-prompt --ip '::' --port 2368 --url 'http://localhost:2368'; 	su-exec node ghost config paths.contentPath "$GHOST_CONTENT"; 		su-exec node ln -s config.production.json "$GHOST_INSTALL/config.development.json"; 	readlink -f "$GHOST_INSTALL/config.development.json"; 		mv "$GHOST_CONTENT" "$GHOST_INSTALL/content.orig"; 	mkdir -p "$GHOST_CONTENT"; 	chown node:node "$GHOST_CONTENT"; 	chmod 1777 "$GHOST_CONTENT"; 		cd "$GHOST_INSTALL/current"; 	packages="$(node -p ' 		var ghost = require("./package.json"); 		var transform = require("./node_modules/@tryghost/image-transform/package.json"); 		[ 			"sharp@" + transform.optionalDependencies["sharp"], 			"sqlite3@" + ghost.optionalDependencies["sqlite3"], 		].join(" ") 	')"; 	if echo "$packages" | grep 'undefined'; then exit 1; fi; 	for package in $packages; do 		installCmd='su-exec node yarn add "$package" --force'; 		if ! eval "$installCmd"; then 			virtualPackages='g++ make python3'; 			case "$package" in 				sharp@*) echo >&2 "sorry: libvips 8.12.1 in Alpine 3.15 is not new enough (8.12.2+) for sharp 0.30 😞"; continue ;; 			esac; 			virtual=".build-deps-${package%%@*}"; 			apkDel="$apkDel $virtual"; 			apk add --no-cache --virtual "$virtual" $virtualPackages; 						eval "$installCmd --build-from-source"; 		fi; 	done; 		if [ -n "$apkDel" ]; then 		apk del --no-network $apkDel; 	fi; 		su-exec node yarn cache clean; 	su-exec node npm cache clean --force; 	npm cache clean --force; 	rm -rv /tmp/yarn* /tmp/v8*
# Sat, 25 Mar 2023 01:19:03 GMT
WORKDIR /var/lib/ghost
# Sat, 25 Mar 2023 01:19:04 GMT
VOLUME [/var/lib/ghost/content]
# Sat, 25 Mar 2023 01:19:04 GMT
COPY file:87209c4c75826f5d839c2f3270a782740f42eecf4bc96b2f6dbae79b08c17e21 in /usr/local/bin 
# Sat, 25 Mar 2023 01:19:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Mar 2023 01:19:04 GMT
EXPOSE 2368
# Sat, 25 Mar 2023 01:19:04 GMT
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
	-	`sha256:c205a53069f074cfc15eda9124d023edd7c457acd8e137f512eb735b94dbbff8`  
		Last Modified: Sat, 25 Mar 2023 01:20:15 GMT  
		Size: 98.1 MB (98108463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b048c4c441b3342b97c79834ee50e6445720c3bd93e567ed2e7d274292534c6e`  
		Last Modified: Sat, 25 Mar 2023 01:20:01 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
