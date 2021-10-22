<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mongo-express`

-	[`mongo-express:0.54`](#mongo-express054)
-	[`mongo-express:0.54.0`](#mongo-express0540)
-	[`mongo-express:1.0.0-alpha`](#mongo-express100-alpha)
-	[`mongo-express:1.0.0-alpha.4`](#mongo-express100-alpha4)
-	[`mongo-express:latest`](#mongo-expresslatest)

## `mongo-express:0.54`

```console
$ docker pull mongo-express@sha256:6bc39d97568da612e43a677983fa570eb3e7f9babd00e41d904308ba4bd13fc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo-express:0.54` - linux; amd64

```console
$ docker pull mongo-express@sha256:bc61c0514e94db622895f1e6a01ef58cf363a49b83b043eab8ee3b34a7b02310
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46828129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05378e191d137d018b2c3764d89f87382afec32b233c342b6b448de77cb3299d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 05:52:55 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 05:53:02 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 05:53:03 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 05:53:08 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 18:56:01 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:56:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 18:56:02 GMT
CMD ["node"]
# Fri, 22 Oct 2021 21:11:01 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 21:11:01 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 21:11:34 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 21:11:34 GMT
ENV MONGO_EXPRESS=0.54.0
# Fri, 22 Oct 2021 21:11:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 21:11:51 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Fri, 22 Oct 2021 21:11:51 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 21:11:52 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 21:11:52 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 21:11:52 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b1fb32259e200075a4ab04b243ecca4272739858745adf943e84d2024b6170`  
		Last Modified: Wed, 13 Oct 2021 06:10:47 GMT  
		Size: 24.6 MB (24620753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40888f2a0a1fdca1cf006d687ff6ef2222922433392055ecf12d883b76a65eab`  
		Last Modified: Wed, 13 Oct 2021 06:10:43 GMT  
		Size: 2.2 MB (2243338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3cc9ce09beb3d44f7dda5da4e79e24ee472be9ffdef7d78680eae65e1aa14f`  
		Last Modified: Fri, 22 Oct 2021 19:10:18 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa1898f3899414a4fb10f0a24782ecf8d425123a687c17593f0cbe18960544f`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 789.3 KB (789328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f39ba6bb39ce45b40f26685ce32feb864423cc66211f684bbfca490a298f0`  
		Last Modified: Fri, 22 Oct 2021 21:12:24 GMT  
		Size: 16.4 MB (16353143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9e7ae54dffa50e9beac930462a74ca8e1ddb7be40cab9d7ff2233242f3d431`  
		Last Modified: Fri, 22 Oct 2021 21:12:22 GMT  
		Size: 655.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a82e57a7f1e655b0f0b32464028624f49e2683fbb81faa4adaca4b702bbde7`  
		Last Modified: Fri, 22 Oct 2021 21:12:23 GMT  
		Size: 3.1 KB (3148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo-express:0.54` - linux; arm64 variant v8

```console
$ docker pull mongo-express@sha256:5bf035faae450d68247fb4364dda361bde60f89de185c179a6eda14e2aa731dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46949203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafad2e5c9548089bf13ccc7fde1af79af169e0e4b7ecc88e113dc12aecd4294`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 04:05:26 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 04:20:56 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 04:20:57 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 04:21:02 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 17:48:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 17:48:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 17:48:30 GMT
CMD ["node"]
# Fri, 22 Oct 2021 19:43:50 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 19:43:51 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 19:44:21 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 19:44:22 GMT
ENV MONGO_EXPRESS=0.54.0
# Fri, 22 Oct 2021 19:44:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 19:44:39 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Fri, 22 Oct 2021 19:44:39 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 19:44:41 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 19:44:41 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 19:44:42 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b3197201b08e68ff95dbc19e91cf430255395077a579d2395824ef5559bb36`  
		Last Modified: Wed, 13 Oct 2021 05:29:42 GMT  
		Size: 24.8 MB (24760702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a38f0f0caa10058f29b20a5f53a372c5b18924b09813e5517a322d8abd39987`  
		Last Modified: Wed, 13 Oct 2021 05:29:38 GMT  
		Size: 2.3 MB (2302269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2283aa6432d7a569a24831fb68000c3f62ac6517814dc2da8978cb573dd197a`  
		Last Modified: Fri, 22 Oct 2021 18:06:47 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf010fd053cf713df6acde05c58dc86bae2a94465cdbcf4e1b5d7d01f6a935c`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 799.9 KB (799898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27da46c3d32725647447223d310af317dc428ade25d30b77d8fe47ffab3a2f44`  
		Last Modified: Fri, 22 Oct 2021 19:45:19 GMT  
		Size: 16.4 MB (16353672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159e3cddb5c8a76bd187db43946146dbe2037c9a202cc546ddcee658972a087f`  
		Last Modified: Fri, 22 Oct 2021 19:45:17 GMT  
		Size: 656.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e05bfec3ffafc03cd15c8ef8cbd385f2e008762fa8bc1a91f8d19d8f997db4`  
		Last Modified: Fri, 22 Oct 2021 19:45:16 GMT  
		Size: 3.1 KB (3150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo-express:0.54.0`

```console
$ docker pull mongo-express@sha256:6bc39d97568da612e43a677983fa570eb3e7f9babd00e41d904308ba4bd13fc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo-express:0.54.0` - linux; amd64

```console
$ docker pull mongo-express@sha256:bc61c0514e94db622895f1e6a01ef58cf363a49b83b043eab8ee3b34a7b02310
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46828129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05378e191d137d018b2c3764d89f87382afec32b233c342b6b448de77cb3299d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 05:52:55 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 05:53:02 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 05:53:03 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 05:53:08 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 18:56:01 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:56:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 18:56:02 GMT
CMD ["node"]
# Fri, 22 Oct 2021 21:11:01 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 21:11:01 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 21:11:34 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 21:11:34 GMT
ENV MONGO_EXPRESS=0.54.0
# Fri, 22 Oct 2021 21:11:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 21:11:51 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Fri, 22 Oct 2021 21:11:51 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 21:11:52 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 21:11:52 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 21:11:52 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b1fb32259e200075a4ab04b243ecca4272739858745adf943e84d2024b6170`  
		Last Modified: Wed, 13 Oct 2021 06:10:47 GMT  
		Size: 24.6 MB (24620753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40888f2a0a1fdca1cf006d687ff6ef2222922433392055ecf12d883b76a65eab`  
		Last Modified: Wed, 13 Oct 2021 06:10:43 GMT  
		Size: 2.2 MB (2243338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3cc9ce09beb3d44f7dda5da4e79e24ee472be9ffdef7d78680eae65e1aa14f`  
		Last Modified: Fri, 22 Oct 2021 19:10:18 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa1898f3899414a4fb10f0a24782ecf8d425123a687c17593f0cbe18960544f`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 789.3 KB (789328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f39ba6bb39ce45b40f26685ce32feb864423cc66211f684bbfca490a298f0`  
		Last Modified: Fri, 22 Oct 2021 21:12:24 GMT  
		Size: 16.4 MB (16353143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9e7ae54dffa50e9beac930462a74ca8e1ddb7be40cab9d7ff2233242f3d431`  
		Last Modified: Fri, 22 Oct 2021 21:12:22 GMT  
		Size: 655.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a82e57a7f1e655b0f0b32464028624f49e2683fbb81faa4adaca4b702bbde7`  
		Last Modified: Fri, 22 Oct 2021 21:12:23 GMT  
		Size: 3.1 KB (3148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo-express:0.54.0` - linux; arm64 variant v8

```console
$ docker pull mongo-express@sha256:5bf035faae450d68247fb4364dda361bde60f89de185c179a6eda14e2aa731dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46949203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafad2e5c9548089bf13ccc7fde1af79af169e0e4b7ecc88e113dc12aecd4294`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 04:05:26 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 04:20:56 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 04:20:57 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 04:21:02 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 17:48:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 17:48:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 17:48:30 GMT
CMD ["node"]
# Fri, 22 Oct 2021 19:43:50 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 19:43:51 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 19:44:21 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 19:44:22 GMT
ENV MONGO_EXPRESS=0.54.0
# Fri, 22 Oct 2021 19:44:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 19:44:39 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Fri, 22 Oct 2021 19:44:39 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 19:44:41 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 19:44:41 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 19:44:42 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b3197201b08e68ff95dbc19e91cf430255395077a579d2395824ef5559bb36`  
		Last Modified: Wed, 13 Oct 2021 05:29:42 GMT  
		Size: 24.8 MB (24760702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a38f0f0caa10058f29b20a5f53a372c5b18924b09813e5517a322d8abd39987`  
		Last Modified: Wed, 13 Oct 2021 05:29:38 GMT  
		Size: 2.3 MB (2302269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2283aa6432d7a569a24831fb68000c3f62ac6517814dc2da8978cb573dd197a`  
		Last Modified: Fri, 22 Oct 2021 18:06:47 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf010fd053cf713df6acde05c58dc86bae2a94465cdbcf4e1b5d7d01f6a935c`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 799.9 KB (799898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27da46c3d32725647447223d310af317dc428ade25d30b77d8fe47ffab3a2f44`  
		Last Modified: Fri, 22 Oct 2021 19:45:19 GMT  
		Size: 16.4 MB (16353672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159e3cddb5c8a76bd187db43946146dbe2037c9a202cc546ddcee658972a087f`  
		Last Modified: Fri, 22 Oct 2021 19:45:17 GMT  
		Size: 656.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e05bfec3ffafc03cd15c8ef8cbd385f2e008762fa8bc1a91f8d19d8f997db4`  
		Last Modified: Fri, 22 Oct 2021 19:45:16 GMT  
		Size: 3.1 KB (3150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo-express:1.0.0-alpha`

```console
$ docker pull mongo-express@sha256:2a25aafdf23296823b06bc9a0a2af2656971262041b8dbf11b40444804fdc104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo-express:1.0.0-alpha` - linux; amd64

```console
$ docker pull mongo-express@sha256:d5cee110909938c99cf8800b9379494c190d8fecaec70a4ce3886facdee6ef8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49229094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2fb2cabc8fa6b894bd7c82158dd7a9dd5815d240f75a93db0d853f008cfd20`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 05:52:55 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 05:53:02 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 05:53:03 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 05:53:08 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 18:56:01 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:56:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 18:56:02 GMT
CMD ["node"]
# Fri, 22 Oct 2021 21:11:01 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 21:11:01 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 21:11:02 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_URL=mongodb://mongo:27017 ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 21:11:02 GMT
ENV MONGO_EXPRESS=1.0.0-alpha.4
# Fri, 22 Oct 2021 21:11:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 21:11:29 GMT
COPY file:4835df10525ec6f18e6339ce0c331b087391dd3279d964040c96a41ba7bf90b7 in / 
# Fri, 22 Oct 2021 21:11:29 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 21:11:30 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 21:11:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 21:11:30 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b1fb32259e200075a4ab04b243ecca4272739858745adf943e84d2024b6170`  
		Last Modified: Wed, 13 Oct 2021 06:10:47 GMT  
		Size: 24.6 MB (24620753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40888f2a0a1fdca1cf006d687ff6ef2222922433392055ecf12d883b76a65eab`  
		Last Modified: Wed, 13 Oct 2021 06:10:43 GMT  
		Size: 2.2 MB (2243338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3cc9ce09beb3d44f7dda5da4e79e24ee472be9ffdef7d78680eae65e1aa14f`  
		Last Modified: Fri, 22 Oct 2021 19:10:18 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa1898f3899414a4fb10f0a24782ecf8d425123a687c17593f0cbe18960544f`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 789.3 KB (789328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4078090382b279408fc5dea2aa5c2684848edf89522cf0d5fc7838aefbfadc`  
		Last Modified: Fri, 22 Oct 2021 21:12:10 GMT  
		Size: 18.8 MB (18753877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae780a42c79ec4c2a8ff24a55d4f621578b787578ce612d6bcd829bfd32663af`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60224d64a049691e21a377295171e15645f999cc04636702e1c18767eb896d1`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 3.3 KB (3303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo-express:1.0.0-alpha` - linux; arm64 variant v8

```console
$ docker pull mongo-express@sha256:9d9120f8308b6d5b47b6b400497a48313d06e15660ced6f87665b50b2fc2ba42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49348435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce615669da5e083c892bcf62fab55dcb6484b42c54ce11de2a3f301e7dc232e4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 04:05:26 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 04:20:56 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 04:20:57 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 04:21:02 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 17:48:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 17:48:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 17:48:30 GMT
CMD ["node"]
# Fri, 22 Oct 2021 19:43:50 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 19:43:51 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 19:43:52 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_URL=mongodb://mongo:27017 ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 19:43:53 GMT
ENV MONGO_EXPRESS=1.0.0-alpha.4
# Fri, 22 Oct 2021 19:44:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 19:44:12 GMT
COPY file:4835df10525ec6f18e6339ce0c331b087391dd3279d964040c96a41ba7bf90b7 in / 
# Fri, 22 Oct 2021 19:44:12 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 19:44:14 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 19:44:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 19:44:15 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b3197201b08e68ff95dbc19e91cf430255395077a579d2395824ef5559bb36`  
		Last Modified: Wed, 13 Oct 2021 05:29:42 GMT  
		Size: 24.8 MB (24760702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a38f0f0caa10058f29b20a5f53a372c5b18924b09813e5517a322d8abd39987`  
		Last Modified: Wed, 13 Oct 2021 05:29:38 GMT  
		Size: 2.3 MB (2302269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2283aa6432d7a569a24831fb68000c3f62ac6517814dc2da8978cb573dd197a`  
		Last Modified: Fri, 22 Oct 2021 18:06:47 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf010fd053cf713df6acde05c58dc86bae2a94465cdbcf4e1b5d7d01f6a935c`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 799.9 KB (799898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a545528b1fec43de49f88b7a27e615796d2a3b9e0a599cedd2af70d35a13bc94`  
		Last Modified: Fri, 22 Oct 2021 19:45:03 GMT  
		Size: 18.8 MB (18752679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fa5610e3594ffa65054f586e287584ac84f3183a31cce7fc47fe95c448f25d`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56780d66f8c3e1060dff7b92ac29efc0b2546d1fc562ca0ac61b568f3f536718`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 3.3 KB (3300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo-express:1.0.0-alpha.4`

```console
$ docker pull mongo-express@sha256:2a25aafdf23296823b06bc9a0a2af2656971262041b8dbf11b40444804fdc104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo-express:1.0.0-alpha.4` - linux; amd64

```console
$ docker pull mongo-express@sha256:d5cee110909938c99cf8800b9379494c190d8fecaec70a4ce3886facdee6ef8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49229094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2fb2cabc8fa6b894bd7c82158dd7a9dd5815d240f75a93db0d853f008cfd20`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 05:52:55 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 05:53:02 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 05:53:03 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 05:53:08 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 18:56:01 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:56:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 18:56:02 GMT
CMD ["node"]
# Fri, 22 Oct 2021 21:11:01 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 21:11:01 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 21:11:02 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_URL=mongodb://mongo:27017 ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 21:11:02 GMT
ENV MONGO_EXPRESS=1.0.0-alpha.4
# Fri, 22 Oct 2021 21:11:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 21:11:29 GMT
COPY file:4835df10525ec6f18e6339ce0c331b087391dd3279d964040c96a41ba7bf90b7 in / 
# Fri, 22 Oct 2021 21:11:29 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 21:11:30 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 21:11:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 21:11:30 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b1fb32259e200075a4ab04b243ecca4272739858745adf943e84d2024b6170`  
		Last Modified: Wed, 13 Oct 2021 06:10:47 GMT  
		Size: 24.6 MB (24620753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40888f2a0a1fdca1cf006d687ff6ef2222922433392055ecf12d883b76a65eab`  
		Last Modified: Wed, 13 Oct 2021 06:10:43 GMT  
		Size: 2.2 MB (2243338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3cc9ce09beb3d44f7dda5da4e79e24ee472be9ffdef7d78680eae65e1aa14f`  
		Last Modified: Fri, 22 Oct 2021 19:10:18 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa1898f3899414a4fb10f0a24782ecf8d425123a687c17593f0cbe18960544f`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 789.3 KB (789328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4078090382b279408fc5dea2aa5c2684848edf89522cf0d5fc7838aefbfadc`  
		Last Modified: Fri, 22 Oct 2021 21:12:10 GMT  
		Size: 18.8 MB (18753877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae780a42c79ec4c2a8ff24a55d4f621578b787578ce612d6bcd829bfd32663af`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60224d64a049691e21a377295171e15645f999cc04636702e1c18767eb896d1`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 3.3 KB (3303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo-express:1.0.0-alpha.4` - linux; arm64 variant v8

```console
$ docker pull mongo-express@sha256:9d9120f8308b6d5b47b6b400497a48313d06e15660ced6f87665b50b2fc2ba42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49348435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce615669da5e083c892bcf62fab55dcb6484b42c54ce11de2a3f301e7dc232e4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 04:05:26 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 04:20:56 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 04:20:57 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 04:21:02 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 17:48:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 17:48:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 17:48:30 GMT
CMD ["node"]
# Fri, 22 Oct 2021 19:43:50 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 19:43:51 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 19:43:52 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_URL=mongodb://mongo:27017 ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 19:43:53 GMT
ENV MONGO_EXPRESS=1.0.0-alpha.4
# Fri, 22 Oct 2021 19:44:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 19:44:12 GMT
COPY file:4835df10525ec6f18e6339ce0c331b087391dd3279d964040c96a41ba7bf90b7 in / 
# Fri, 22 Oct 2021 19:44:12 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 19:44:14 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 19:44:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 19:44:15 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b3197201b08e68ff95dbc19e91cf430255395077a579d2395824ef5559bb36`  
		Last Modified: Wed, 13 Oct 2021 05:29:42 GMT  
		Size: 24.8 MB (24760702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a38f0f0caa10058f29b20a5f53a372c5b18924b09813e5517a322d8abd39987`  
		Last Modified: Wed, 13 Oct 2021 05:29:38 GMT  
		Size: 2.3 MB (2302269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2283aa6432d7a569a24831fb68000c3f62ac6517814dc2da8978cb573dd197a`  
		Last Modified: Fri, 22 Oct 2021 18:06:47 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf010fd053cf713df6acde05c58dc86bae2a94465cdbcf4e1b5d7d01f6a935c`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 799.9 KB (799898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a545528b1fec43de49f88b7a27e615796d2a3b9e0a599cedd2af70d35a13bc94`  
		Last Modified: Fri, 22 Oct 2021 19:45:03 GMT  
		Size: 18.8 MB (18752679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fa5610e3594ffa65054f586e287584ac84f3183a31cce7fc47fe95c448f25d`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56780d66f8c3e1060dff7b92ac29efc0b2546d1fc562ca0ac61b568f3f536718`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 3.3 KB (3300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mongo-express:latest`

```console
$ docker pull mongo-express@sha256:2a25aafdf23296823b06bc9a0a2af2656971262041b8dbf11b40444804fdc104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo-express:latest` - linux; amd64

```console
$ docker pull mongo-express@sha256:d5cee110909938c99cf8800b9379494c190d8fecaec70a4ce3886facdee6ef8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49229094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2fb2cabc8fa6b894bd7c82158dd7a9dd5815d240f75a93db0d853f008cfd20`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 05:52:55 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 05:53:02 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 05:53:03 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 05:53:08 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 18:56:01 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:56:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 18:56:02 GMT
CMD ["node"]
# Fri, 22 Oct 2021 21:11:01 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 21:11:01 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 21:11:02 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_URL=mongodb://mongo:27017 ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 21:11:02 GMT
ENV MONGO_EXPRESS=1.0.0-alpha.4
# Fri, 22 Oct 2021 21:11:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 21:11:29 GMT
COPY file:4835df10525ec6f18e6339ce0c331b087391dd3279d964040c96a41ba7bf90b7 in / 
# Fri, 22 Oct 2021 21:11:29 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 21:11:30 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 21:11:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 21:11:30 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b1fb32259e200075a4ab04b243ecca4272739858745adf943e84d2024b6170`  
		Last Modified: Wed, 13 Oct 2021 06:10:47 GMT  
		Size: 24.6 MB (24620753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40888f2a0a1fdca1cf006d687ff6ef2222922433392055ecf12d883b76a65eab`  
		Last Modified: Wed, 13 Oct 2021 06:10:43 GMT  
		Size: 2.2 MB (2243338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3cc9ce09beb3d44f7dda5da4e79e24ee472be9ffdef7d78680eae65e1aa14f`  
		Last Modified: Fri, 22 Oct 2021 19:10:18 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa1898f3899414a4fb10f0a24782ecf8d425123a687c17593f0cbe18960544f`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 789.3 KB (789328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4078090382b279408fc5dea2aa5c2684848edf89522cf0d5fc7838aefbfadc`  
		Last Modified: Fri, 22 Oct 2021 21:12:10 GMT  
		Size: 18.8 MB (18753877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae780a42c79ec4c2a8ff24a55d4f621578b787578ce612d6bcd829bfd32663af`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60224d64a049691e21a377295171e15645f999cc04636702e1c18767eb896d1`  
		Last Modified: Fri, 22 Oct 2021 21:12:07 GMT  
		Size: 3.3 KB (3303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo-express:latest` - linux; arm64 variant v8

```console
$ docker pull mongo-express@sha256:9d9120f8308b6d5b47b6b400497a48313d06e15660ced6f87665b50b2fc2ba42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49348435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce615669da5e083c892bcf62fab55dcb6484b42c54ce11de2a3f301e7dc232e4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:59 GMT
ADD file:da6c0ac7cb9f819998546d88fb489b746004eb2ad6da64a39210696ef0e66e54 in / 
# Wed, 01 Sep 2021 02:50:59 GMT
CMD ["/bin/sh"]
# Wed, 13 Oct 2021 04:05:26 GMT
ENV NODE_VERSION=12.22.7
# Wed, 13 Oct 2021 04:20:56 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 13 Oct 2021 04:20:57 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 04:21:02 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 22 Oct 2021 17:48:29 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 17:48:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 17:48:30 GMT
CMD ["node"]
# Fri, 22 Oct 2021 19:43:50 GMT
RUN apk add --no-cache bash tini
# Fri, 22 Oct 2021 19:43:51 GMT
EXPOSE 8081
# Fri, 22 Oct 2021 19:43:52 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_URL=mongodb://mongo:27017 ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 22 Oct 2021 19:43:53 GMT
ENV MONGO_EXPRESS=1.0.0-alpha.4
# Fri, 22 Oct 2021 19:44:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 22 Oct 2021 19:44:12 GMT
COPY file:4835df10525ec6f18e6339ce0c331b087391dd3279d964040c96a41ba7bf90b7 in / 
# Fri, 22 Oct 2021 19:44:12 GMT
WORKDIR /node_modules/mongo-express
# Fri, 22 Oct 2021 19:44:14 GMT
RUN cp config.default.js config.js
# Fri, 22 Oct 2021 19:44:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 19:44:15 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:07d756952c5cd45726cf9e8a292a3e05ca67eee5da176df7d632be8c5bb0ad04`  
		Last Modified: Wed, 01 Sep 2021 02:52:00 GMT  
		Size: 2.7 MB (2728407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b3197201b08e68ff95dbc19e91cf430255395077a579d2395824ef5559bb36`  
		Last Modified: Wed, 13 Oct 2021 05:29:42 GMT  
		Size: 24.8 MB (24760702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a38f0f0caa10058f29b20a5f53a372c5b18924b09813e5517a322d8abd39987`  
		Last Modified: Wed, 13 Oct 2021 05:29:38 GMT  
		Size: 2.3 MB (2302269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2283aa6432d7a569a24831fb68000c3f62ac6517814dc2da8978cb573dd197a`  
		Last Modified: Fri, 22 Oct 2021 18:06:47 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf010fd053cf713df6acde05c58dc86bae2a94465cdbcf4e1b5d7d01f6a935c`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 799.9 KB (799898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a545528b1fec43de49f88b7a27e615796d2a3b9e0a599cedd2af70d35a13bc94`  
		Last Modified: Fri, 22 Oct 2021 19:45:03 GMT  
		Size: 18.8 MB (18752679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fa5610e3594ffa65054f586e287584ac84f3183a31cce7fc47fe95c448f25d`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56780d66f8c3e1060dff7b92ac29efc0b2546d1fc562ca0ac61b568f3f536718`  
		Last Modified: Fri, 22 Oct 2021 19:45:00 GMT  
		Size: 3.3 KB (3300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
