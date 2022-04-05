<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `express-gateway`

-	[`express-gateway:1.16.11`](#express-gateway11611)
-	[`express-gateway:1.16.x`](#express-gateway116x)
-	[`express-gateway:1.x`](#express-gateway1x)
-	[`express-gateway:latest`](#express-gatewaylatest)

## `express-gateway:1.16.11`

```console
$ docker pull express-gateway@sha256:60c3deaace65bf95f64666f2c4e2c0a0804170f337498d149be7f2ffcef9d4d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `express-gateway:1.16.11` - linux; amd64

```console
$ docker pull express-gateway@sha256:8f28f56f9d07df13dfdfaa777c6730fa5e587dd1a3afd526ee1da6f87737b4f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40220686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29c0a1f79c50c1821da7a745c413eae5a4c69f4a976579ac26630d7426279a1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:12:24 GMT
ENV NODE_VERSION=12.22.11
# Tue, 05 Apr 2022 10:12:33 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 05 Apr 2022 10:12:33 GMT
ENV YARN_VERSION=1.22.17
# Tue, 05 Apr 2022 10:12:37 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 05 Apr 2022 10:12:37 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:12:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:12:37 GMT
CMD ["node"]
# Tue, 05 Apr 2022 15:53:33 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Tue, 05 Apr 2022 15:53:33 GMT
ARG EG_VERSION=1.16.11
# Tue, 05 Apr 2022 15:53:51 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Tue, 05 Apr 2022 15:53:52 GMT
ENV NODE_ENV=production
# Tue, 05 Apr 2022 15:53:52 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Tue, 05 Apr 2022 15:53:52 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Tue, 05 Apr 2022 15:53:52 GMT
ENV CHOKIDAR_USEPOLLING=true
# Tue, 05 Apr 2022 15:53:52 GMT
VOLUME [/var/lib/eg]
# Tue, 05 Apr 2022 15:53:52 GMT
EXPOSE 8080 9876
# Tue, 05 Apr 2022 15:53:52 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:53:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:53:53 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531844641126be05299dabbf98c669da74090d29770e1fb5ea8d84730fec5b3b`  
		Last Modified: Tue, 05 Apr 2022 10:19:26 GMT  
		Size: 24.9 MB (24908154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433587b2f2e8ca21cbb938472fdd992ea693c8e812327ac84e23e63f995d0697`  
		Last Modified: Tue, 05 Apr 2022 10:19:22 GMT  
		Size: 2.4 MB (2357893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8c7a0941626ad6a8c89ef9c288344005231e3c11fa2beb9b69ed9084438919`  
		Last Modified: Tue, 05 Apr 2022 10:19:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21e218ece3ade1d88ad6cde6d8e817b9fcaeb9dd6526828575ea15f19ed7d9d`  
		Last Modified: Tue, 05 Apr 2022 15:54:08 GMT  
		Size: 10.1 MB (10139127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af1afe42cfcb948b68365b8f898176b8d32ed257796b820479ba3c3757fcfd8`  
		Last Modified: Tue, 05 Apr 2022 15:54:06 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.11` - linux; arm64 variant v8

```console
$ docker pull express-gateway@sha256:0555de03db833c98e9e84a29aee86cbf488093ddf2750e818580cc10063f9dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40095883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dea3df4b8ae38632c4fe6e8fb57734270b06591876c5654aa5556828d4b18ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 23:51:51 GMT
ENV NODE_VERSION=12.22.11
# Wed, 30 Mar 2022 00:16:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 30 Mar 2022 00:16:05 GMT
ENV YARN_VERSION=1.22.17
# Wed, 30 Mar 2022 00:16:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 30 Mar 2022 00:16:13 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 30 Mar 2022 00:16:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 00:16:14 GMT
CMD ["node"]
# Wed, 30 Mar 2022 21:52:51 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Wed, 30 Mar 2022 21:52:51 GMT
ARG EG_VERSION=1.16.11
# Wed, 30 Mar 2022 21:53:17 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Wed, 30 Mar 2022 21:53:18 GMT
ENV NODE_ENV=production
# Wed, 30 Mar 2022 21:53:19 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Wed, 30 Mar 2022 21:53:20 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Wed, 30 Mar 2022 21:53:21 GMT
ENV CHOKIDAR_USEPOLLING=true
# Wed, 30 Mar 2022 21:53:22 GMT
VOLUME [/var/lib/eg]
# Wed, 30 Mar 2022 21:53:23 GMT
EXPOSE 8080 9876
# Wed, 30 Mar 2022 21:53:25 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Wed, 30 Mar 2022 21:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 21:53:26 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26de282d29a8a25d910aa7fd63640165b9877c3870e8b67d444f1a65155c9198`  
		Last Modified: Wed, 30 Mar 2022 00:34:22 GMT  
		Size: 24.8 MB (24803672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d62aadc49d18bd6705fbd2ff01febe5ef479625c0e9fbcf9ea515c8c5371a`  
		Last Modified: Wed, 30 Mar 2022 00:34:18 GMT  
		Size: 2.4 MB (2438209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2328a5ff8b0351af8616231117a13ccdeb3e72da702c38209d3f878d2404e368`  
		Last Modified: Wed, 30 Mar 2022 00:34:18 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab3b99e2bb98c55a6df3223d412d0d38f8c81e2bc7ae0efc4eedbb6f2647889`  
		Last Modified: Wed, 30 Mar 2022 21:53:49 GMT  
		Size: 10.1 MB (10136705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66a57a627bb400110a61827a566afd0529abb2abbbf273726d85af77eda045b`  
		Last Modified: Wed, 30 Mar 2022 21:53:47 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.11` - linux; ppc64le

```console
$ docker pull express-gateway@sha256:92d9e20d80718625b88b5e4cf52d87cbf3068e425c3fb8440aefba65c25900a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42522076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0673b556cc4a7e9b607730a939741ccdd57b192cd777985a9da250167a53da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:58:17 GMT
ENV NODE_VERSION=12.22.11
# Tue, 29 Mar 2022 12:17:32 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 29 Mar 2022 12:17:38 GMT
ENV YARN_VERSION=1.22.17
# Tue, 29 Mar 2022 12:17:52 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 29 Mar 2022 12:17:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:18:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:18:03 GMT
CMD ["node"]
# Thu, 31 Mar 2022 01:55:19 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Thu, 31 Mar 2022 01:55:25 GMT
ARG EG_VERSION=1.16.11
# Thu, 31 Mar 2022 01:56:17 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Thu, 31 Mar 2022 01:56:23 GMT
ENV NODE_ENV=production
# Thu, 31 Mar 2022 01:56:26 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Thu, 31 Mar 2022 01:56:34 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Thu, 31 Mar 2022 01:56:37 GMT
ENV CHOKIDAR_USEPOLLING=true
# Thu, 31 Mar 2022 01:56:41 GMT
VOLUME [/var/lib/eg]
# Thu, 31 Mar 2022 01:56:46 GMT
EXPOSE 8080 9876
# Thu, 31 Mar 2022 01:56:47 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Thu, 31 Mar 2022 01:56:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 31 Mar 2022 01:56:57 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9667107f92b05a88c0ab857080019b5d447c33c02d85335ef7d647d19586e6`  
		Last Modified: Tue, 29 Mar 2022 12:39:12 GMT  
		Size: 27.1 MB (27136316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d3a1ba50ab2b72dc936e422f4dac4f17adee0cf9e95664177bf541e41e5e4f`  
		Last Modified: Tue, 29 Mar 2022 12:39:07 GMT  
		Size: 2.4 MB (2438247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc68635dbf2fcebc4f8e6c6366d87940ac261f6b9d4a40bc7f571245e4ba03af`  
		Last Modified: Tue, 29 Mar 2022 12:39:06 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f5bce043faf23f853a689a23df0fdfed81ffcac68548988999ba977c7b4e`  
		Last Modified: Thu, 31 Mar 2022 01:57:28 GMT  
		Size: 10.1 MB (10135558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889073f0902baee3b79cfc8380a7aa08757a91acb5be0dd104434ebb772ff700`  
		Last Modified: Thu, 31 Mar 2022 01:57:24 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.11` - linux; s390x

```console
$ docker pull express-gateway@sha256:d79d2081a09a37dbfa3202ccafa240a8dcf790a6dae477b149d55d7f94400886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39983485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:146c879398b4dfe43d43c8ec1ca653accb3a66b428f98b58d798a05fa3443af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:10 GMT
ENV NODE_VERSION=12.22.11
# Tue, 05 Apr 2022 11:09:35 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 05 Apr 2022 11:09:37 GMT
ENV YARN_VERSION=1.22.17
# Tue, 05 Apr 2022 11:09:40 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 05 Apr 2022 11:09:41 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:09:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:09:41 GMT
CMD ["node"]
# Tue, 05 Apr 2022 14:03:38 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Tue, 05 Apr 2022 14:03:38 GMT
ARG EG_VERSION=1.16.11
# Tue, 05 Apr 2022 14:03:56 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Tue, 05 Apr 2022 14:03:57 GMT
ENV NODE_ENV=production
# Tue, 05 Apr 2022 14:03:58 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Tue, 05 Apr 2022 14:03:58 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Tue, 05 Apr 2022 14:03:58 GMT
ENV CHOKIDAR_USEPOLLING=true
# Tue, 05 Apr 2022 14:03:58 GMT
VOLUME [/var/lib/eg]
# Tue, 05 Apr 2022 14:03:58 GMT
EXPOSE 8080 9876
# Tue, 05 Apr 2022 14:03:58 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:03:59 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18178392e9afb2211641a91b1519a64daefa9b91077d38da82ed04aafc72ae10`  
		Last Modified: Tue, 05 Apr 2022 11:18:03 GMT  
		Size: 24.8 MB (24802252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef15af4b0e35b008f982d9b9c9285a9a0b4bb72bfb85d43abb107afd1d1f4f28`  
		Last Modified: Tue, 05 Apr 2022 11:18:00 GMT  
		Size: 2.4 MB (2440715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7dabc9fdb78338c5632b86f133973b0a28c230a8bb54d9bf27a6a738b027d4`  
		Last Modified: Tue, 05 Apr 2022 11:18:00 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfaa9c669c53b9056e6d39b839631ca67a750ae0bfe4119c4dbff8485cbe594`  
		Last Modified: Tue, 05 Apr 2022 14:04:20 GMT  
		Size: 10.1 MB (10139195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16833b391b4cfa63195065eac5674ad382b8d613a3b55147e2f718e9b98d14e2`  
		Last Modified: Tue, 05 Apr 2022 14:04:18 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `express-gateway:1.16.x`

```console
$ docker pull express-gateway@sha256:60c3deaace65bf95f64666f2c4e2c0a0804170f337498d149be7f2ffcef9d4d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `express-gateway:1.16.x` - linux; amd64

```console
$ docker pull express-gateway@sha256:8f28f56f9d07df13dfdfaa777c6730fa5e587dd1a3afd526ee1da6f87737b4f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40220686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29c0a1f79c50c1821da7a745c413eae5a4c69f4a976579ac26630d7426279a1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:12:24 GMT
ENV NODE_VERSION=12.22.11
# Tue, 05 Apr 2022 10:12:33 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 05 Apr 2022 10:12:33 GMT
ENV YARN_VERSION=1.22.17
# Tue, 05 Apr 2022 10:12:37 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 05 Apr 2022 10:12:37 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:12:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:12:37 GMT
CMD ["node"]
# Tue, 05 Apr 2022 15:53:33 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Tue, 05 Apr 2022 15:53:33 GMT
ARG EG_VERSION=1.16.11
# Tue, 05 Apr 2022 15:53:51 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Tue, 05 Apr 2022 15:53:52 GMT
ENV NODE_ENV=production
# Tue, 05 Apr 2022 15:53:52 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Tue, 05 Apr 2022 15:53:52 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Tue, 05 Apr 2022 15:53:52 GMT
ENV CHOKIDAR_USEPOLLING=true
# Tue, 05 Apr 2022 15:53:52 GMT
VOLUME [/var/lib/eg]
# Tue, 05 Apr 2022 15:53:52 GMT
EXPOSE 8080 9876
# Tue, 05 Apr 2022 15:53:52 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:53:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:53:53 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531844641126be05299dabbf98c669da74090d29770e1fb5ea8d84730fec5b3b`  
		Last Modified: Tue, 05 Apr 2022 10:19:26 GMT  
		Size: 24.9 MB (24908154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433587b2f2e8ca21cbb938472fdd992ea693c8e812327ac84e23e63f995d0697`  
		Last Modified: Tue, 05 Apr 2022 10:19:22 GMT  
		Size: 2.4 MB (2357893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8c7a0941626ad6a8c89ef9c288344005231e3c11fa2beb9b69ed9084438919`  
		Last Modified: Tue, 05 Apr 2022 10:19:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21e218ece3ade1d88ad6cde6d8e817b9fcaeb9dd6526828575ea15f19ed7d9d`  
		Last Modified: Tue, 05 Apr 2022 15:54:08 GMT  
		Size: 10.1 MB (10139127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af1afe42cfcb948b68365b8f898176b8d32ed257796b820479ba3c3757fcfd8`  
		Last Modified: Tue, 05 Apr 2022 15:54:06 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.x` - linux; arm64 variant v8

```console
$ docker pull express-gateway@sha256:0555de03db833c98e9e84a29aee86cbf488093ddf2750e818580cc10063f9dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40095883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dea3df4b8ae38632c4fe6e8fb57734270b06591876c5654aa5556828d4b18ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 23:51:51 GMT
ENV NODE_VERSION=12.22.11
# Wed, 30 Mar 2022 00:16:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 30 Mar 2022 00:16:05 GMT
ENV YARN_VERSION=1.22.17
# Wed, 30 Mar 2022 00:16:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 30 Mar 2022 00:16:13 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 30 Mar 2022 00:16:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 00:16:14 GMT
CMD ["node"]
# Wed, 30 Mar 2022 21:52:51 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Wed, 30 Mar 2022 21:52:51 GMT
ARG EG_VERSION=1.16.11
# Wed, 30 Mar 2022 21:53:17 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Wed, 30 Mar 2022 21:53:18 GMT
ENV NODE_ENV=production
# Wed, 30 Mar 2022 21:53:19 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Wed, 30 Mar 2022 21:53:20 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Wed, 30 Mar 2022 21:53:21 GMT
ENV CHOKIDAR_USEPOLLING=true
# Wed, 30 Mar 2022 21:53:22 GMT
VOLUME [/var/lib/eg]
# Wed, 30 Mar 2022 21:53:23 GMT
EXPOSE 8080 9876
# Wed, 30 Mar 2022 21:53:25 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Wed, 30 Mar 2022 21:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 21:53:26 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26de282d29a8a25d910aa7fd63640165b9877c3870e8b67d444f1a65155c9198`  
		Last Modified: Wed, 30 Mar 2022 00:34:22 GMT  
		Size: 24.8 MB (24803672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d62aadc49d18bd6705fbd2ff01febe5ef479625c0e9fbcf9ea515c8c5371a`  
		Last Modified: Wed, 30 Mar 2022 00:34:18 GMT  
		Size: 2.4 MB (2438209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2328a5ff8b0351af8616231117a13ccdeb3e72da702c38209d3f878d2404e368`  
		Last Modified: Wed, 30 Mar 2022 00:34:18 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab3b99e2bb98c55a6df3223d412d0d38f8c81e2bc7ae0efc4eedbb6f2647889`  
		Last Modified: Wed, 30 Mar 2022 21:53:49 GMT  
		Size: 10.1 MB (10136705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66a57a627bb400110a61827a566afd0529abb2abbbf273726d85af77eda045b`  
		Last Modified: Wed, 30 Mar 2022 21:53:47 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.x` - linux; ppc64le

```console
$ docker pull express-gateway@sha256:92d9e20d80718625b88b5e4cf52d87cbf3068e425c3fb8440aefba65c25900a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42522076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0673b556cc4a7e9b607730a939741ccdd57b192cd777985a9da250167a53da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:58:17 GMT
ENV NODE_VERSION=12.22.11
# Tue, 29 Mar 2022 12:17:32 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 29 Mar 2022 12:17:38 GMT
ENV YARN_VERSION=1.22.17
# Tue, 29 Mar 2022 12:17:52 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 29 Mar 2022 12:17:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:18:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:18:03 GMT
CMD ["node"]
# Thu, 31 Mar 2022 01:55:19 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Thu, 31 Mar 2022 01:55:25 GMT
ARG EG_VERSION=1.16.11
# Thu, 31 Mar 2022 01:56:17 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Thu, 31 Mar 2022 01:56:23 GMT
ENV NODE_ENV=production
# Thu, 31 Mar 2022 01:56:26 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Thu, 31 Mar 2022 01:56:34 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Thu, 31 Mar 2022 01:56:37 GMT
ENV CHOKIDAR_USEPOLLING=true
# Thu, 31 Mar 2022 01:56:41 GMT
VOLUME [/var/lib/eg]
# Thu, 31 Mar 2022 01:56:46 GMT
EXPOSE 8080 9876
# Thu, 31 Mar 2022 01:56:47 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Thu, 31 Mar 2022 01:56:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 31 Mar 2022 01:56:57 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9667107f92b05a88c0ab857080019b5d447c33c02d85335ef7d647d19586e6`  
		Last Modified: Tue, 29 Mar 2022 12:39:12 GMT  
		Size: 27.1 MB (27136316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d3a1ba50ab2b72dc936e422f4dac4f17adee0cf9e95664177bf541e41e5e4f`  
		Last Modified: Tue, 29 Mar 2022 12:39:07 GMT  
		Size: 2.4 MB (2438247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc68635dbf2fcebc4f8e6c6366d87940ac261f6b9d4a40bc7f571245e4ba03af`  
		Last Modified: Tue, 29 Mar 2022 12:39:06 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f5bce043faf23f853a689a23df0fdfed81ffcac68548988999ba977c7b4e`  
		Last Modified: Thu, 31 Mar 2022 01:57:28 GMT  
		Size: 10.1 MB (10135558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889073f0902baee3b79cfc8380a7aa08757a91acb5be0dd104434ebb772ff700`  
		Last Modified: Thu, 31 Mar 2022 01:57:24 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.x` - linux; s390x

```console
$ docker pull express-gateway@sha256:d79d2081a09a37dbfa3202ccafa240a8dcf790a6dae477b149d55d7f94400886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39983485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:146c879398b4dfe43d43c8ec1ca653accb3a66b428f98b58d798a05fa3443af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:10 GMT
ENV NODE_VERSION=12.22.11
# Tue, 05 Apr 2022 11:09:35 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 05 Apr 2022 11:09:37 GMT
ENV YARN_VERSION=1.22.17
# Tue, 05 Apr 2022 11:09:40 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 05 Apr 2022 11:09:41 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:09:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:09:41 GMT
CMD ["node"]
# Tue, 05 Apr 2022 14:03:38 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Tue, 05 Apr 2022 14:03:38 GMT
ARG EG_VERSION=1.16.11
# Tue, 05 Apr 2022 14:03:56 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Tue, 05 Apr 2022 14:03:57 GMT
ENV NODE_ENV=production
# Tue, 05 Apr 2022 14:03:58 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Tue, 05 Apr 2022 14:03:58 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Tue, 05 Apr 2022 14:03:58 GMT
ENV CHOKIDAR_USEPOLLING=true
# Tue, 05 Apr 2022 14:03:58 GMT
VOLUME [/var/lib/eg]
# Tue, 05 Apr 2022 14:03:58 GMT
EXPOSE 8080 9876
# Tue, 05 Apr 2022 14:03:58 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:03:59 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18178392e9afb2211641a91b1519a64daefa9b91077d38da82ed04aafc72ae10`  
		Last Modified: Tue, 05 Apr 2022 11:18:03 GMT  
		Size: 24.8 MB (24802252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef15af4b0e35b008f982d9b9c9285a9a0b4bb72bfb85d43abb107afd1d1f4f28`  
		Last Modified: Tue, 05 Apr 2022 11:18:00 GMT  
		Size: 2.4 MB (2440715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7dabc9fdb78338c5632b86f133973b0a28c230a8bb54d9bf27a6a738b027d4`  
		Last Modified: Tue, 05 Apr 2022 11:18:00 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfaa9c669c53b9056e6d39b839631ca67a750ae0bfe4119c4dbff8485cbe594`  
		Last Modified: Tue, 05 Apr 2022 14:04:20 GMT  
		Size: 10.1 MB (10139195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16833b391b4cfa63195065eac5674ad382b8d613a3b55147e2f718e9b98d14e2`  
		Last Modified: Tue, 05 Apr 2022 14:04:18 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `express-gateway:1.x`

```console
$ docker pull express-gateway@sha256:60c3deaace65bf95f64666f2c4e2c0a0804170f337498d149be7f2ffcef9d4d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `express-gateway:1.x` - linux; amd64

```console
$ docker pull express-gateway@sha256:8f28f56f9d07df13dfdfaa777c6730fa5e587dd1a3afd526ee1da6f87737b4f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40220686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29c0a1f79c50c1821da7a745c413eae5a4c69f4a976579ac26630d7426279a1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:12:24 GMT
ENV NODE_VERSION=12.22.11
# Tue, 05 Apr 2022 10:12:33 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 05 Apr 2022 10:12:33 GMT
ENV YARN_VERSION=1.22.17
# Tue, 05 Apr 2022 10:12:37 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 05 Apr 2022 10:12:37 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:12:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:12:37 GMT
CMD ["node"]
# Tue, 05 Apr 2022 15:53:33 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Tue, 05 Apr 2022 15:53:33 GMT
ARG EG_VERSION=1.16.11
# Tue, 05 Apr 2022 15:53:51 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Tue, 05 Apr 2022 15:53:52 GMT
ENV NODE_ENV=production
# Tue, 05 Apr 2022 15:53:52 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Tue, 05 Apr 2022 15:53:52 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Tue, 05 Apr 2022 15:53:52 GMT
ENV CHOKIDAR_USEPOLLING=true
# Tue, 05 Apr 2022 15:53:52 GMT
VOLUME [/var/lib/eg]
# Tue, 05 Apr 2022 15:53:52 GMT
EXPOSE 8080 9876
# Tue, 05 Apr 2022 15:53:52 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:53:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:53:53 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531844641126be05299dabbf98c669da74090d29770e1fb5ea8d84730fec5b3b`  
		Last Modified: Tue, 05 Apr 2022 10:19:26 GMT  
		Size: 24.9 MB (24908154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433587b2f2e8ca21cbb938472fdd992ea693c8e812327ac84e23e63f995d0697`  
		Last Modified: Tue, 05 Apr 2022 10:19:22 GMT  
		Size: 2.4 MB (2357893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8c7a0941626ad6a8c89ef9c288344005231e3c11fa2beb9b69ed9084438919`  
		Last Modified: Tue, 05 Apr 2022 10:19:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21e218ece3ade1d88ad6cde6d8e817b9fcaeb9dd6526828575ea15f19ed7d9d`  
		Last Modified: Tue, 05 Apr 2022 15:54:08 GMT  
		Size: 10.1 MB (10139127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af1afe42cfcb948b68365b8f898176b8d32ed257796b820479ba3c3757fcfd8`  
		Last Modified: Tue, 05 Apr 2022 15:54:06 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.x` - linux; arm64 variant v8

```console
$ docker pull express-gateway@sha256:0555de03db833c98e9e84a29aee86cbf488093ddf2750e818580cc10063f9dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40095883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dea3df4b8ae38632c4fe6e8fb57734270b06591876c5654aa5556828d4b18ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 23:51:51 GMT
ENV NODE_VERSION=12.22.11
# Wed, 30 Mar 2022 00:16:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 30 Mar 2022 00:16:05 GMT
ENV YARN_VERSION=1.22.17
# Wed, 30 Mar 2022 00:16:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 30 Mar 2022 00:16:13 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 30 Mar 2022 00:16:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 00:16:14 GMT
CMD ["node"]
# Wed, 30 Mar 2022 21:52:51 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Wed, 30 Mar 2022 21:52:51 GMT
ARG EG_VERSION=1.16.11
# Wed, 30 Mar 2022 21:53:17 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Wed, 30 Mar 2022 21:53:18 GMT
ENV NODE_ENV=production
# Wed, 30 Mar 2022 21:53:19 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Wed, 30 Mar 2022 21:53:20 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Wed, 30 Mar 2022 21:53:21 GMT
ENV CHOKIDAR_USEPOLLING=true
# Wed, 30 Mar 2022 21:53:22 GMT
VOLUME [/var/lib/eg]
# Wed, 30 Mar 2022 21:53:23 GMT
EXPOSE 8080 9876
# Wed, 30 Mar 2022 21:53:25 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Wed, 30 Mar 2022 21:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 21:53:26 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26de282d29a8a25d910aa7fd63640165b9877c3870e8b67d444f1a65155c9198`  
		Last Modified: Wed, 30 Mar 2022 00:34:22 GMT  
		Size: 24.8 MB (24803672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d62aadc49d18bd6705fbd2ff01febe5ef479625c0e9fbcf9ea515c8c5371a`  
		Last Modified: Wed, 30 Mar 2022 00:34:18 GMT  
		Size: 2.4 MB (2438209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2328a5ff8b0351af8616231117a13ccdeb3e72da702c38209d3f878d2404e368`  
		Last Modified: Wed, 30 Mar 2022 00:34:18 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab3b99e2bb98c55a6df3223d412d0d38f8c81e2bc7ae0efc4eedbb6f2647889`  
		Last Modified: Wed, 30 Mar 2022 21:53:49 GMT  
		Size: 10.1 MB (10136705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66a57a627bb400110a61827a566afd0529abb2abbbf273726d85af77eda045b`  
		Last Modified: Wed, 30 Mar 2022 21:53:47 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.x` - linux; ppc64le

```console
$ docker pull express-gateway@sha256:92d9e20d80718625b88b5e4cf52d87cbf3068e425c3fb8440aefba65c25900a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42522076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0673b556cc4a7e9b607730a939741ccdd57b192cd777985a9da250167a53da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:58:17 GMT
ENV NODE_VERSION=12.22.11
# Tue, 29 Mar 2022 12:17:32 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 29 Mar 2022 12:17:38 GMT
ENV YARN_VERSION=1.22.17
# Tue, 29 Mar 2022 12:17:52 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 29 Mar 2022 12:17:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:18:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:18:03 GMT
CMD ["node"]
# Thu, 31 Mar 2022 01:55:19 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Thu, 31 Mar 2022 01:55:25 GMT
ARG EG_VERSION=1.16.11
# Thu, 31 Mar 2022 01:56:17 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Thu, 31 Mar 2022 01:56:23 GMT
ENV NODE_ENV=production
# Thu, 31 Mar 2022 01:56:26 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Thu, 31 Mar 2022 01:56:34 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Thu, 31 Mar 2022 01:56:37 GMT
ENV CHOKIDAR_USEPOLLING=true
# Thu, 31 Mar 2022 01:56:41 GMT
VOLUME [/var/lib/eg]
# Thu, 31 Mar 2022 01:56:46 GMT
EXPOSE 8080 9876
# Thu, 31 Mar 2022 01:56:47 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Thu, 31 Mar 2022 01:56:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 31 Mar 2022 01:56:57 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9667107f92b05a88c0ab857080019b5d447c33c02d85335ef7d647d19586e6`  
		Last Modified: Tue, 29 Mar 2022 12:39:12 GMT  
		Size: 27.1 MB (27136316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d3a1ba50ab2b72dc936e422f4dac4f17adee0cf9e95664177bf541e41e5e4f`  
		Last Modified: Tue, 29 Mar 2022 12:39:07 GMT  
		Size: 2.4 MB (2438247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc68635dbf2fcebc4f8e6c6366d87940ac261f6b9d4a40bc7f571245e4ba03af`  
		Last Modified: Tue, 29 Mar 2022 12:39:06 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f5bce043faf23f853a689a23df0fdfed81ffcac68548988999ba977c7b4e`  
		Last Modified: Thu, 31 Mar 2022 01:57:28 GMT  
		Size: 10.1 MB (10135558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889073f0902baee3b79cfc8380a7aa08757a91acb5be0dd104434ebb772ff700`  
		Last Modified: Thu, 31 Mar 2022 01:57:24 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.x` - linux; s390x

```console
$ docker pull express-gateway@sha256:d79d2081a09a37dbfa3202ccafa240a8dcf790a6dae477b149d55d7f94400886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39983485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:146c879398b4dfe43d43c8ec1ca653accb3a66b428f98b58d798a05fa3443af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:10 GMT
ENV NODE_VERSION=12.22.11
# Tue, 05 Apr 2022 11:09:35 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 05 Apr 2022 11:09:37 GMT
ENV YARN_VERSION=1.22.17
# Tue, 05 Apr 2022 11:09:40 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 05 Apr 2022 11:09:41 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:09:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:09:41 GMT
CMD ["node"]
# Tue, 05 Apr 2022 14:03:38 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Tue, 05 Apr 2022 14:03:38 GMT
ARG EG_VERSION=1.16.11
# Tue, 05 Apr 2022 14:03:56 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Tue, 05 Apr 2022 14:03:57 GMT
ENV NODE_ENV=production
# Tue, 05 Apr 2022 14:03:58 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Tue, 05 Apr 2022 14:03:58 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Tue, 05 Apr 2022 14:03:58 GMT
ENV CHOKIDAR_USEPOLLING=true
# Tue, 05 Apr 2022 14:03:58 GMT
VOLUME [/var/lib/eg]
# Tue, 05 Apr 2022 14:03:58 GMT
EXPOSE 8080 9876
# Tue, 05 Apr 2022 14:03:58 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:03:59 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18178392e9afb2211641a91b1519a64daefa9b91077d38da82ed04aafc72ae10`  
		Last Modified: Tue, 05 Apr 2022 11:18:03 GMT  
		Size: 24.8 MB (24802252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef15af4b0e35b008f982d9b9c9285a9a0b4bb72bfb85d43abb107afd1d1f4f28`  
		Last Modified: Tue, 05 Apr 2022 11:18:00 GMT  
		Size: 2.4 MB (2440715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7dabc9fdb78338c5632b86f133973b0a28c230a8bb54d9bf27a6a738b027d4`  
		Last Modified: Tue, 05 Apr 2022 11:18:00 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfaa9c669c53b9056e6d39b839631ca67a750ae0bfe4119c4dbff8485cbe594`  
		Last Modified: Tue, 05 Apr 2022 14:04:20 GMT  
		Size: 10.1 MB (10139195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16833b391b4cfa63195065eac5674ad382b8d613a3b55147e2f718e9b98d14e2`  
		Last Modified: Tue, 05 Apr 2022 14:04:18 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `express-gateway:latest`

```console
$ docker pull express-gateway@sha256:60c3deaace65bf95f64666f2c4e2c0a0804170f337498d149be7f2ffcef9d4d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `express-gateway:latest` - linux; amd64

```console
$ docker pull express-gateway@sha256:8f28f56f9d07df13dfdfaa777c6730fa5e587dd1a3afd526ee1da6f87737b4f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40220686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29c0a1f79c50c1821da7a745c413eae5a4c69f4a976579ac26630d7426279a1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:12:24 GMT
ENV NODE_VERSION=12.22.11
# Tue, 05 Apr 2022 10:12:33 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 05 Apr 2022 10:12:33 GMT
ENV YARN_VERSION=1.22.17
# Tue, 05 Apr 2022 10:12:37 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 05 Apr 2022 10:12:37 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:12:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:12:37 GMT
CMD ["node"]
# Tue, 05 Apr 2022 15:53:33 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Tue, 05 Apr 2022 15:53:33 GMT
ARG EG_VERSION=1.16.11
# Tue, 05 Apr 2022 15:53:51 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Tue, 05 Apr 2022 15:53:52 GMT
ENV NODE_ENV=production
# Tue, 05 Apr 2022 15:53:52 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Tue, 05 Apr 2022 15:53:52 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Tue, 05 Apr 2022 15:53:52 GMT
ENV CHOKIDAR_USEPOLLING=true
# Tue, 05 Apr 2022 15:53:52 GMT
VOLUME [/var/lib/eg]
# Tue, 05 Apr 2022 15:53:52 GMT
EXPOSE 8080 9876
# Tue, 05 Apr 2022 15:53:52 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Tue, 05 Apr 2022 15:53:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 15:53:53 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531844641126be05299dabbf98c669da74090d29770e1fb5ea8d84730fec5b3b`  
		Last Modified: Tue, 05 Apr 2022 10:19:26 GMT  
		Size: 24.9 MB (24908154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433587b2f2e8ca21cbb938472fdd992ea693c8e812327ac84e23e63f995d0697`  
		Last Modified: Tue, 05 Apr 2022 10:19:22 GMT  
		Size: 2.4 MB (2357893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8c7a0941626ad6a8c89ef9c288344005231e3c11fa2beb9b69ed9084438919`  
		Last Modified: Tue, 05 Apr 2022 10:19:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21e218ece3ade1d88ad6cde6d8e817b9fcaeb9dd6526828575ea15f19ed7d9d`  
		Last Modified: Tue, 05 Apr 2022 15:54:08 GMT  
		Size: 10.1 MB (10139127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af1afe42cfcb948b68365b8f898176b8d32ed257796b820479ba3c3757fcfd8`  
		Last Modified: Tue, 05 Apr 2022 15:54:06 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:latest` - linux; arm64 variant v8

```console
$ docker pull express-gateway@sha256:0555de03db833c98e9e84a29aee86cbf488093ddf2750e818580cc10063f9dbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40095883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dea3df4b8ae38632c4fe6e8fb57734270b06591876c5654aa5556828d4b18ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 23:51:51 GMT
ENV NODE_VERSION=12.22.11
# Wed, 30 Mar 2022 00:16:04 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 30 Mar 2022 00:16:05 GMT
ENV YARN_VERSION=1.22.17
# Wed, 30 Mar 2022 00:16:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 30 Mar 2022 00:16:13 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 30 Mar 2022 00:16:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 00:16:14 GMT
CMD ["node"]
# Wed, 30 Mar 2022 21:52:51 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Wed, 30 Mar 2022 21:52:51 GMT
ARG EG_VERSION=1.16.11
# Wed, 30 Mar 2022 21:53:17 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Wed, 30 Mar 2022 21:53:18 GMT
ENV NODE_ENV=production
# Wed, 30 Mar 2022 21:53:19 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Wed, 30 Mar 2022 21:53:20 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Wed, 30 Mar 2022 21:53:21 GMT
ENV CHOKIDAR_USEPOLLING=true
# Wed, 30 Mar 2022 21:53:22 GMT
VOLUME [/var/lib/eg]
# Wed, 30 Mar 2022 21:53:23 GMT
EXPOSE 8080 9876
# Wed, 30 Mar 2022 21:53:25 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Wed, 30 Mar 2022 21:53:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 30 Mar 2022 21:53:26 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26de282d29a8a25d910aa7fd63640165b9877c3870e8b67d444f1a65155c9198`  
		Last Modified: Wed, 30 Mar 2022 00:34:22 GMT  
		Size: 24.8 MB (24803672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7d62aadc49d18bd6705fbd2ff01febe5ef479625c0e9fbcf9ea515c8c5371a`  
		Last Modified: Wed, 30 Mar 2022 00:34:18 GMT  
		Size: 2.4 MB (2438209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2328a5ff8b0351af8616231117a13ccdeb3e72da702c38209d3f878d2404e368`  
		Last Modified: Wed, 30 Mar 2022 00:34:18 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab3b99e2bb98c55a6df3223d412d0d38f8c81e2bc7ae0efc4eedbb6f2647889`  
		Last Modified: Wed, 30 Mar 2022 21:53:49 GMT  
		Size: 10.1 MB (10136705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66a57a627bb400110a61827a566afd0529abb2abbbf273726d85af77eda045b`  
		Last Modified: Wed, 30 Mar 2022 21:53:47 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:latest` - linux; ppc64le

```console
$ docker pull express-gateway@sha256:92d9e20d80718625b88b5e4cf52d87cbf3068e425c3fb8440aefba65c25900a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42522076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0673b556cc4a7e9b607730a939741ccdd57b192cd777985a9da250167a53da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:58:17 GMT
ENV NODE_VERSION=12.22.11
# Tue, 29 Mar 2022 12:17:32 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 29 Mar 2022 12:17:38 GMT
ENV YARN_VERSION=1.22.17
# Tue, 29 Mar 2022 12:17:52 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 29 Mar 2022 12:17:55 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 29 Mar 2022 12:18:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Mar 2022 12:18:03 GMT
CMD ["node"]
# Thu, 31 Mar 2022 01:55:19 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Thu, 31 Mar 2022 01:55:25 GMT
ARG EG_VERSION=1.16.11
# Thu, 31 Mar 2022 01:56:17 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Thu, 31 Mar 2022 01:56:23 GMT
ENV NODE_ENV=production
# Thu, 31 Mar 2022 01:56:26 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Thu, 31 Mar 2022 01:56:34 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Thu, 31 Mar 2022 01:56:37 GMT
ENV CHOKIDAR_USEPOLLING=true
# Thu, 31 Mar 2022 01:56:41 GMT
VOLUME [/var/lib/eg]
# Thu, 31 Mar 2022 01:56:46 GMT
EXPOSE 8080 9876
# Thu, 31 Mar 2022 01:56:47 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Thu, 31 Mar 2022 01:56:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 31 Mar 2022 01:56:57 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9667107f92b05a88c0ab857080019b5d447c33c02d85335ef7d647d19586e6`  
		Last Modified: Tue, 29 Mar 2022 12:39:12 GMT  
		Size: 27.1 MB (27136316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d3a1ba50ab2b72dc936e422f4dac4f17adee0cf9e95664177bf541e41e5e4f`  
		Last Modified: Tue, 29 Mar 2022 12:39:07 GMT  
		Size: 2.4 MB (2438247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc68635dbf2fcebc4f8e6c6366d87940ac261f6b9d4a40bc7f571245e4ba03af`  
		Last Modified: Tue, 29 Mar 2022 12:39:06 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18f5bce043faf23f853a689a23df0fdfed81ffcac68548988999ba977c7b4e`  
		Last Modified: Thu, 31 Mar 2022 01:57:28 GMT  
		Size: 10.1 MB (10135558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889073f0902baee3b79cfc8380a7aa08757a91acb5be0dd104434ebb772ff700`  
		Last Modified: Thu, 31 Mar 2022 01:57:24 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:latest` - linux; s390x

```console
$ docker pull express-gateway@sha256:d79d2081a09a37dbfa3202ccafa240a8dcf790a6dae477b149d55d7f94400886
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39983485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:146c879398b4dfe43d43c8ec1ca653accb3a66b428f98b58d798a05fa3443af1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:50:10 GMT
ENV NODE_VERSION=12.22.11
# Tue, 05 Apr 2022 11:09:35 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 05 Apr 2022 11:09:37 GMT
ENV YARN_VERSION=1.22.17
# Tue, 05 Apr 2022 11:09:40 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 05 Apr 2022 11:09:41 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:09:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:09:41 GMT
CMD ["node"]
# Tue, 05 Apr 2022 14:03:38 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Tue, 05 Apr 2022 14:03:38 GMT
ARG EG_VERSION=1.16.11
# Tue, 05 Apr 2022 14:03:56 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Tue, 05 Apr 2022 14:03:57 GMT
ENV NODE_ENV=production
# Tue, 05 Apr 2022 14:03:58 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Tue, 05 Apr 2022 14:03:58 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Tue, 05 Apr 2022 14:03:58 GMT
ENV CHOKIDAR_USEPOLLING=true
# Tue, 05 Apr 2022 14:03:58 GMT
VOLUME [/var/lib/eg]
# Tue, 05 Apr 2022 14:03:58 GMT
EXPOSE 8080 9876
# Tue, 05 Apr 2022 14:03:58 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Tue, 05 Apr 2022 14:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 14:03:59 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18178392e9afb2211641a91b1519a64daefa9b91077d38da82ed04aafc72ae10`  
		Last Modified: Tue, 05 Apr 2022 11:18:03 GMT  
		Size: 24.8 MB (24802252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef15af4b0e35b008f982d9b9c9285a9a0b4bb72bfb85d43abb107afd1d1f4f28`  
		Last Modified: Tue, 05 Apr 2022 11:18:00 GMT  
		Size: 2.4 MB (2440715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7dabc9fdb78338c5632b86f133973b0a28c230a8bb54d9bf27a6a738b027d4`  
		Last Modified: Tue, 05 Apr 2022 11:18:00 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfaa9c669c53b9056e6d39b839631ca67a750ae0bfe4119c4dbff8485cbe594`  
		Last Modified: Tue, 05 Apr 2022 14:04:20 GMT  
		Size: 10.1 MB (10139195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16833b391b4cfa63195065eac5674ad382b8d613a3b55147e2f718e9b98d14e2`  
		Last Modified: Tue, 05 Apr 2022 14:04:18 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
