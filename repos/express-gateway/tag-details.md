<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `express-gateway`

-	[`express-gateway:1.16.11`](#express-gateway11611)
-	[`express-gateway:1.16.x`](#express-gateway116x)
-	[`express-gateway:1.x`](#express-gateway1x)
-	[`express-gateway:latest`](#express-gatewaylatest)

## `express-gateway:1.16.11`

```console
$ docker pull express-gateway@sha256:30fefcd985a841fb1f0f5eaef659cadca137dcf5a341307e8b5336db23cd1934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `express-gateway:1.16.11` - linux; amd64

```console
$ docker pull express-gateway@sha256:9fdb12a4f04ea0d0ded3a4183f279993a20df1e387b345e5541c263729caa8ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40177423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19671d273209ca1a7ebe3b9a0c66f26677c9a9676e3d0eb44e0c1c0aba532ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 21:54:38 GMT
ENV NODE_VERSION=12.22.11
# Fri, 18 Mar 2022 21:54:50 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 21:54:50 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:54:56 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 21:54:56 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:54:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:54:56 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:10:40 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 19 Mar 2022 00:10:40 GMT
ARG EG_VERSION=1.16.11
# Sat, 19 Mar 2022 00:11:04 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 19 Mar 2022 00:11:05 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:11:05 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 19 Mar 2022 00:11:05 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 19 Mar 2022 00:11:05 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 19 Mar 2022 00:11:05 GMT
VOLUME [/var/lib/eg]
# Sat, 19 Mar 2022 00:11:05 GMT
EXPOSE 8080 9876
# Sat, 19 Mar 2022 00:11:06 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:11:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:11:06 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4df20eca50beea3c4188568910712f5683e5d0497ba399c818213b73180e273`  
		Last Modified: Fri, 18 Mar 2022 22:17:11 GMT  
		Size: 24.9 MB (24907620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb8006bb2b0d1233915059f504c0e715fd8f43c409ef20878acafb279c5a785`  
		Last Modified: Fri, 18 Mar 2022 22:17:06 GMT  
		Size: 2.4 MB (2357895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f64245aee5e460a1afa73858263e95c471cde81f3bb6ebdf6a3d4eda0012fb`  
		Last Modified: Fri, 18 Mar 2022 22:17:05 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cc5e35bdccf9b4518dd259bc7e3dc9f5a52644e2c4bce27d94b9c584e9ba74`  
		Last Modified: Sat, 19 Mar 2022 00:11:22 GMT  
		Size: 10.1 MB (10098321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9169b1660824e9f509de7cb767b624f42b9cd6771f692b4a34b52f00d3ba5b9`  
		Last Modified: Sat, 19 Mar 2022 00:11:19 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.11` - linux; arm64 variant v8

```console
$ docker pull express-gateway@sha256:8420121d1d31ca646480565f8e735646200f903502c5b325df4b78d3321406f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40060865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26d80065dd102c820850bf947f35e459416a10edae8f4ab3665c420e1c61f723`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:13:22 GMT
ENV NODE_VERSION=12.22.11
# Sat, 19 Mar 2022 00:31:55 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 19 Mar 2022 00:31:56 GMT
ENV YARN_VERSION=1.22.17
# Sat, 19 Mar 2022 00:32:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 19 Mar 2022 00:32:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:32:06 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:52:35 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 19 Mar 2022 17:52:35 GMT
ARG EG_VERSION=1.16.11
# Sat, 19 Mar 2022 17:53:00 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 19 Mar 2022 17:53:01 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:53:02 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 19 Mar 2022 17:53:03 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 19 Mar 2022 17:53:04 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 19 Mar 2022 17:53:05 GMT
VOLUME [/var/lib/eg]
# Sat, 19 Mar 2022 17:53:06 GMT
EXPOSE 8080 9876
# Sat, 19 Mar 2022 17:53:08 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 19 Mar 2022 17:53:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:53:09 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4804b7fb3c60c6fd6d87ca3cea8f51583c5fa4e023d214248111e38ed597f`  
		Last Modified: Sat, 19 Mar 2022 00:56:50 GMT  
		Size: 24.8 MB (24803893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aa9e6c8534e79c8ff44bec0a6845088d5b1fe5cbb9a4f3657cbd24d84edee8`  
		Last Modified: Sat, 19 Mar 2022 00:56:46 GMT  
		Size: 2.4 MB (2438217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91d150c92f25556d9b1bdce6869f06d0ac18f645b941beaf980ccf0610fc4a8`  
		Last Modified: Sat, 19 Mar 2022 00:56:45 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16240801f297dcde4abf0883a71ef9c4b20e54595525acfb587f577a745cd968`  
		Last Modified: Sat, 19 Mar 2022 17:53:32 GMT  
		Size: 10.1 MB (10103002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625c6593e1c334a62aaa85ab9a088f4f929d723c13e761ce33ce5bceac2e7c1f`  
		Last Modified: Sat, 19 Mar 2022 17:53:29 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.11` - linux; ppc64le

```console
$ docker pull express-gateway@sha256:26d4baad39231541adfce1bb6ecab7f45fe52d81695fcad5db4f49cc0ee136f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42523175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a057efda589b92876538c5d5f75653fafb897c037d7580ff004e50db6c3e22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 11:14:04 GMT
ADD file:ddc94e1e084c05807db26adcc95b47a137fa47fb391e75998b338ada65e00c1c in / 
# Thu, 17 Mar 2022 11:14:09 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 23:44:23 GMT
ENV NODE_VERSION=12.22.11
# Sat, 19 Mar 2022 00:04:36 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 19 Mar 2022 00:04:47 GMT
ENV YARN_VERSION=1.22.17
# Sat, 19 Mar 2022 00:05:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 19 Mar 2022 00:05:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:05:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:05:12 GMT
CMD ["node"]
# Sun, 20 Mar 2022 02:26:13 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sun, 20 Mar 2022 02:26:16 GMT
ARG EG_VERSION=1.16.11
# Sun, 20 Mar 2022 02:27:11 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sun, 20 Mar 2022 02:27:16 GMT
ENV NODE_ENV=production
# Sun, 20 Mar 2022 02:27:19 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sun, 20 Mar 2022 02:27:22 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sun, 20 Mar 2022 02:27:25 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sun, 20 Mar 2022 02:27:29 GMT
VOLUME [/var/lib/eg]
# Sun, 20 Mar 2022 02:27:31 GMT
EXPOSE 8080 9876
# Sun, 20 Mar 2022 02:27:34 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sun, 20 Mar 2022 02:27:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 02:27:40 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:eef85fcc847498263d979ef7ec75680d05e90815eb83a9ec4db135b990c0d8b8`  
		Last Modified: Thu, 17 Mar 2022 11:15:15 GMT  
		Size: 2.8 MB (2814051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520f8182ba461712aeb72b3184ad1ab550f0da9aac8b041e3d128bd5081ef25`  
		Last Modified: Sat, 19 Mar 2022 02:17:11 GMT  
		Size: 27.1 MB (27136542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2b8da92dd97b67e17b234dec546b6585e21ba0d0042599f5679b16af964ebf`  
		Last Modified: Sat, 19 Mar 2022 02:17:07 GMT  
		Size: 2.4 MB (2438373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fdb16adbd7fbe1d7ec85d6a222900e9ce2313cd9b63a1bb8dad84d75d43a66`  
		Last Modified: Sat, 19 Mar 2022 02:17:06 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec81d857a561a987e15c89297b8275e3f386a9e87d9c0edd2729c63ba7da477`  
		Last Modified: Sun, 20 Mar 2022 02:28:09 GMT  
		Size: 10.1 MB (10133259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b41adb5d74866605ffef0cba06c0cfd1196e97b14395547321c3b827a4eb08`  
		Last Modified: Sun, 20 Mar 2022 02:28:06 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.11` - linux; s390x

```console
$ docker pull express-gateway@sha256:5477d675e36dc9ffe5bf4feb73731848dc5ceaeb3394264de1f53eebfdc14ee7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39943968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e75c9ba837f5d9b352a127b02bea42dedde22cd405d2336407ee3b88593fdc0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 22:37:27 GMT
ENV NODE_VERSION=12.22.11
# Fri, 18 Mar 2022 22:57:09 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 22:57:10 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:57:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 22:57:14 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:57:14 GMT
CMD ["node"]
# Fri, 18 Mar 2022 23:12:34 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Fri, 18 Mar 2022 23:12:34 GMT
ARG EG_VERSION=1.16.11
# Fri, 18 Mar 2022 23:12:53 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Fri, 18 Mar 2022 23:12:55 GMT
ENV NODE_ENV=production
# Fri, 18 Mar 2022 23:12:56 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Fri, 18 Mar 2022 23:12:56 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Fri, 18 Mar 2022 23:12:56 GMT
ENV CHOKIDAR_USEPOLLING=true
# Fri, 18 Mar 2022 23:12:56 GMT
VOLUME [/var/lib/eg]
# Fri, 18 Mar 2022 23:12:56 GMT
EXPOSE 8080 9876
# Fri, 18 Mar 2022 23:12:56 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:12:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:12:56 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc7615e0810b845e7a7a67083a6fe5e8f87b1a58b6097a02a34bc03be25367`  
		Last Modified: Fri, 18 Mar 2022 23:11:09 GMT  
		Size: 24.8 MB (24802008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa5357697f7e0751e355eafc575990ac0869a5e684f10b8baee5a1ed80d6d8a`  
		Last Modified: Fri, 18 Mar 2022 23:11:05 GMT  
		Size: 2.4 MB (2440644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58972249e28a7f4674026b4d9d987ee90c90e9a8c3ef62722da31f781c74ab32`  
		Last Modified: Fri, 18 Mar 2022 23:11:05 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a46cee6202c0abe148ea21a1e7645a8aa3de118ebe01fca5ee1f57747ff833`  
		Last Modified: Fri, 18 Mar 2022 23:13:19 GMT  
		Size: 10.1 MB (10098658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466d9746795cef0cf0d6ad6e38cef1507bd55e7da3614926bcf9c1941f5a234b`  
		Last Modified: Fri, 18 Mar 2022 23:13:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `express-gateway:1.16.x`

```console
$ docker pull express-gateway@sha256:30fefcd985a841fb1f0f5eaef659cadca137dcf5a341307e8b5336db23cd1934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `express-gateway:1.16.x` - linux; amd64

```console
$ docker pull express-gateway@sha256:9fdb12a4f04ea0d0ded3a4183f279993a20df1e387b345e5541c263729caa8ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40177423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19671d273209ca1a7ebe3b9a0c66f26677c9a9676e3d0eb44e0c1c0aba532ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 21:54:38 GMT
ENV NODE_VERSION=12.22.11
# Fri, 18 Mar 2022 21:54:50 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 21:54:50 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:54:56 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 21:54:56 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:54:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:54:56 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:10:40 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 19 Mar 2022 00:10:40 GMT
ARG EG_VERSION=1.16.11
# Sat, 19 Mar 2022 00:11:04 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 19 Mar 2022 00:11:05 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:11:05 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 19 Mar 2022 00:11:05 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 19 Mar 2022 00:11:05 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 19 Mar 2022 00:11:05 GMT
VOLUME [/var/lib/eg]
# Sat, 19 Mar 2022 00:11:05 GMT
EXPOSE 8080 9876
# Sat, 19 Mar 2022 00:11:06 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:11:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:11:06 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4df20eca50beea3c4188568910712f5683e5d0497ba399c818213b73180e273`  
		Last Modified: Fri, 18 Mar 2022 22:17:11 GMT  
		Size: 24.9 MB (24907620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb8006bb2b0d1233915059f504c0e715fd8f43c409ef20878acafb279c5a785`  
		Last Modified: Fri, 18 Mar 2022 22:17:06 GMT  
		Size: 2.4 MB (2357895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f64245aee5e460a1afa73858263e95c471cde81f3bb6ebdf6a3d4eda0012fb`  
		Last Modified: Fri, 18 Mar 2022 22:17:05 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cc5e35bdccf9b4518dd259bc7e3dc9f5a52644e2c4bce27d94b9c584e9ba74`  
		Last Modified: Sat, 19 Mar 2022 00:11:22 GMT  
		Size: 10.1 MB (10098321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9169b1660824e9f509de7cb767b624f42b9cd6771f692b4a34b52f00d3ba5b9`  
		Last Modified: Sat, 19 Mar 2022 00:11:19 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.x` - linux; arm64 variant v8

```console
$ docker pull express-gateway@sha256:8420121d1d31ca646480565f8e735646200f903502c5b325df4b78d3321406f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40060865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26d80065dd102c820850bf947f35e459416a10edae8f4ab3665c420e1c61f723`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:13:22 GMT
ENV NODE_VERSION=12.22.11
# Sat, 19 Mar 2022 00:31:55 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 19 Mar 2022 00:31:56 GMT
ENV YARN_VERSION=1.22.17
# Sat, 19 Mar 2022 00:32:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 19 Mar 2022 00:32:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:32:06 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:52:35 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 19 Mar 2022 17:52:35 GMT
ARG EG_VERSION=1.16.11
# Sat, 19 Mar 2022 17:53:00 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 19 Mar 2022 17:53:01 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:53:02 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 19 Mar 2022 17:53:03 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 19 Mar 2022 17:53:04 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 19 Mar 2022 17:53:05 GMT
VOLUME [/var/lib/eg]
# Sat, 19 Mar 2022 17:53:06 GMT
EXPOSE 8080 9876
# Sat, 19 Mar 2022 17:53:08 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 19 Mar 2022 17:53:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:53:09 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4804b7fb3c60c6fd6d87ca3cea8f51583c5fa4e023d214248111e38ed597f`  
		Last Modified: Sat, 19 Mar 2022 00:56:50 GMT  
		Size: 24.8 MB (24803893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aa9e6c8534e79c8ff44bec0a6845088d5b1fe5cbb9a4f3657cbd24d84edee8`  
		Last Modified: Sat, 19 Mar 2022 00:56:46 GMT  
		Size: 2.4 MB (2438217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91d150c92f25556d9b1bdce6869f06d0ac18f645b941beaf980ccf0610fc4a8`  
		Last Modified: Sat, 19 Mar 2022 00:56:45 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16240801f297dcde4abf0883a71ef9c4b20e54595525acfb587f577a745cd968`  
		Last Modified: Sat, 19 Mar 2022 17:53:32 GMT  
		Size: 10.1 MB (10103002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625c6593e1c334a62aaa85ab9a088f4f929d723c13e761ce33ce5bceac2e7c1f`  
		Last Modified: Sat, 19 Mar 2022 17:53:29 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.x` - linux; ppc64le

```console
$ docker pull express-gateway@sha256:26d4baad39231541adfce1bb6ecab7f45fe52d81695fcad5db4f49cc0ee136f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42523175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a057efda589b92876538c5d5f75653fafb897c037d7580ff004e50db6c3e22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 11:14:04 GMT
ADD file:ddc94e1e084c05807db26adcc95b47a137fa47fb391e75998b338ada65e00c1c in / 
# Thu, 17 Mar 2022 11:14:09 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 23:44:23 GMT
ENV NODE_VERSION=12.22.11
# Sat, 19 Mar 2022 00:04:36 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 19 Mar 2022 00:04:47 GMT
ENV YARN_VERSION=1.22.17
# Sat, 19 Mar 2022 00:05:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 19 Mar 2022 00:05:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:05:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:05:12 GMT
CMD ["node"]
# Sun, 20 Mar 2022 02:26:13 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sun, 20 Mar 2022 02:26:16 GMT
ARG EG_VERSION=1.16.11
# Sun, 20 Mar 2022 02:27:11 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sun, 20 Mar 2022 02:27:16 GMT
ENV NODE_ENV=production
# Sun, 20 Mar 2022 02:27:19 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sun, 20 Mar 2022 02:27:22 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sun, 20 Mar 2022 02:27:25 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sun, 20 Mar 2022 02:27:29 GMT
VOLUME [/var/lib/eg]
# Sun, 20 Mar 2022 02:27:31 GMT
EXPOSE 8080 9876
# Sun, 20 Mar 2022 02:27:34 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sun, 20 Mar 2022 02:27:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 02:27:40 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:eef85fcc847498263d979ef7ec75680d05e90815eb83a9ec4db135b990c0d8b8`  
		Last Modified: Thu, 17 Mar 2022 11:15:15 GMT  
		Size: 2.8 MB (2814051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520f8182ba461712aeb72b3184ad1ab550f0da9aac8b041e3d128bd5081ef25`  
		Last Modified: Sat, 19 Mar 2022 02:17:11 GMT  
		Size: 27.1 MB (27136542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2b8da92dd97b67e17b234dec546b6585e21ba0d0042599f5679b16af964ebf`  
		Last Modified: Sat, 19 Mar 2022 02:17:07 GMT  
		Size: 2.4 MB (2438373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fdb16adbd7fbe1d7ec85d6a222900e9ce2313cd9b63a1bb8dad84d75d43a66`  
		Last Modified: Sat, 19 Mar 2022 02:17:06 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec81d857a561a987e15c89297b8275e3f386a9e87d9c0edd2729c63ba7da477`  
		Last Modified: Sun, 20 Mar 2022 02:28:09 GMT  
		Size: 10.1 MB (10133259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b41adb5d74866605ffef0cba06c0cfd1196e97b14395547321c3b827a4eb08`  
		Last Modified: Sun, 20 Mar 2022 02:28:06 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.16.x` - linux; s390x

```console
$ docker pull express-gateway@sha256:5477d675e36dc9ffe5bf4feb73731848dc5ceaeb3394264de1f53eebfdc14ee7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39943968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e75c9ba837f5d9b352a127b02bea42dedde22cd405d2336407ee3b88593fdc0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 22:37:27 GMT
ENV NODE_VERSION=12.22.11
# Fri, 18 Mar 2022 22:57:09 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 22:57:10 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:57:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 22:57:14 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:57:14 GMT
CMD ["node"]
# Fri, 18 Mar 2022 23:12:34 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Fri, 18 Mar 2022 23:12:34 GMT
ARG EG_VERSION=1.16.11
# Fri, 18 Mar 2022 23:12:53 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Fri, 18 Mar 2022 23:12:55 GMT
ENV NODE_ENV=production
# Fri, 18 Mar 2022 23:12:56 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Fri, 18 Mar 2022 23:12:56 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Fri, 18 Mar 2022 23:12:56 GMT
ENV CHOKIDAR_USEPOLLING=true
# Fri, 18 Mar 2022 23:12:56 GMT
VOLUME [/var/lib/eg]
# Fri, 18 Mar 2022 23:12:56 GMT
EXPOSE 8080 9876
# Fri, 18 Mar 2022 23:12:56 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:12:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:12:56 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc7615e0810b845e7a7a67083a6fe5e8f87b1a58b6097a02a34bc03be25367`  
		Last Modified: Fri, 18 Mar 2022 23:11:09 GMT  
		Size: 24.8 MB (24802008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa5357697f7e0751e355eafc575990ac0869a5e684f10b8baee5a1ed80d6d8a`  
		Last Modified: Fri, 18 Mar 2022 23:11:05 GMT  
		Size: 2.4 MB (2440644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58972249e28a7f4674026b4d9d987ee90c90e9a8c3ef62722da31f781c74ab32`  
		Last Modified: Fri, 18 Mar 2022 23:11:05 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a46cee6202c0abe148ea21a1e7645a8aa3de118ebe01fca5ee1f57747ff833`  
		Last Modified: Fri, 18 Mar 2022 23:13:19 GMT  
		Size: 10.1 MB (10098658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466d9746795cef0cf0d6ad6e38cef1507bd55e7da3614926bcf9c1941f5a234b`  
		Last Modified: Fri, 18 Mar 2022 23:13:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `express-gateway:1.x`

```console
$ docker pull express-gateway@sha256:30fefcd985a841fb1f0f5eaef659cadca137dcf5a341307e8b5336db23cd1934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `express-gateway:1.x` - linux; amd64

```console
$ docker pull express-gateway@sha256:9fdb12a4f04ea0d0ded3a4183f279993a20df1e387b345e5541c263729caa8ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40177423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19671d273209ca1a7ebe3b9a0c66f26677c9a9676e3d0eb44e0c1c0aba532ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 21:54:38 GMT
ENV NODE_VERSION=12.22.11
# Fri, 18 Mar 2022 21:54:50 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 21:54:50 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:54:56 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 21:54:56 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:54:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:54:56 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:10:40 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 19 Mar 2022 00:10:40 GMT
ARG EG_VERSION=1.16.11
# Sat, 19 Mar 2022 00:11:04 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 19 Mar 2022 00:11:05 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:11:05 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 19 Mar 2022 00:11:05 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 19 Mar 2022 00:11:05 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 19 Mar 2022 00:11:05 GMT
VOLUME [/var/lib/eg]
# Sat, 19 Mar 2022 00:11:05 GMT
EXPOSE 8080 9876
# Sat, 19 Mar 2022 00:11:06 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:11:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:11:06 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4df20eca50beea3c4188568910712f5683e5d0497ba399c818213b73180e273`  
		Last Modified: Fri, 18 Mar 2022 22:17:11 GMT  
		Size: 24.9 MB (24907620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb8006bb2b0d1233915059f504c0e715fd8f43c409ef20878acafb279c5a785`  
		Last Modified: Fri, 18 Mar 2022 22:17:06 GMT  
		Size: 2.4 MB (2357895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f64245aee5e460a1afa73858263e95c471cde81f3bb6ebdf6a3d4eda0012fb`  
		Last Modified: Fri, 18 Mar 2022 22:17:05 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cc5e35bdccf9b4518dd259bc7e3dc9f5a52644e2c4bce27d94b9c584e9ba74`  
		Last Modified: Sat, 19 Mar 2022 00:11:22 GMT  
		Size: 10.1 MB (10098321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9169b1660824e9f509de7cb767b624f42b9cd6771f692b4a34b52f00d3ba5b9`  
		Last Modified: Sat, 19 Mar 2022 00:11:19 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.x` - linux; arm64 variant v8

```console
$ docker pull express-gateway@sha256:8420121d1d31ca646480565f8e735646200f903502c5b325df4b78d3321406f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40060865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26d80065dd102c820850bf947f35e459416a10edae8f4ab3665c420e1c61f723`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:13:22 GMT
ENV NODE_VERSION=12.22.11
# Sat, 19 Mar 2022 00:31:55 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 19 Mar 2022 00:31:56 GMT
ENV YARN_VERSION=1.22.17
# Sat, 19 Mar 2022 00:32:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 19 Mar 2022 00:32:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:32:06 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:52:35 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 19 Mar 2022 17:52:35 GMT
ARG EG_VERSION=1.16.11
# Sat, 19 Mar 2022 17:53:00 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 19 Mar 2022 17:53:01 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:53:02 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 19 Mar 2022 17:53:03 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 19 Mar 2022 17:53:04 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 19 Mar 2022 17:53:05 GMT
VOLUME [/var/lib/eg]
# Sat, 19 Mar 2022 17:53:06 GMT
EXPOSE 8080 9876
# Sat, 19 Mar 2022 17:53:08 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 19 Mar 2022 17:53:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:53:09 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4804b7fb3c60c6fd6d87ca3cea8f51583c5fa4e023d214248111e38ed597f`  
		Last Modified: Sat, 19 Mar 2022 00:56:50 GMT  
		Size: 24.8 MB (24803893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aa9e6c8534e79c8ff44bec0a6845088d5b1fe5cbb9a4f3657cbd24d84edee8`  
		Last Modified: Sat, 19 Mar 2022 00:56:46 GMT  
		Size: 2.4 MB (2438217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91d150c92f25556d9b1bdce6869f06d0ac18f645b941beaf980ccf0610fc4a8`  
		Last Modified: Sat, 19 Mar 2022 00:56:45 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16240801f297dcde4abf0883a71ef9c4b20e54595525acfb587f577a745cd968`  
		Last Modified: Sat, 19 Mar 2022 17:53:32 GMT  
		Size: 10.1 MB (10103002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625c6593e1c334a62aaa85ab9a088f4f929d723c13e761ce33ce5bceac2e7c1f`  
		Last Modified: Sat, 19 Mar 2022 17:53:29 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.x` - linux; ppc64le

```console
$ docker pull express-gateway@sha256:26d4baad39231541adfce1bb6ecab7f45fe52d81695fcad5db4f49cc0ee136f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42523175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a057efda589b92876538c5d5f75653fafb897c037d7580ff004e50db6c3e22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 11:14:04 GMT
ADD file:ddc94e1e084c05807db26adcc95b47a137fa47fb391e75998b338ada65e00c1c in / 
# Thu, 17 Mar 2022 11:14:09 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 23:44:23 GMT
ENV NODE_VERSION=12.22.11
# Sat, 19 Mar 2022 00:04:36 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 19 Mar 2022 00:04:47 GMT
ENV YARN_VERSION=1.22.17
# Sat, 19 Mar 2022 00:05:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 19 Mar 2022 00:05:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:05:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:05:12 GMT
CMD ["node"]
# Sun, 20 Mar 2022 02:26:13 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sun, 20 Mar 2022 02:26:16 GMT
ARG EG_VERSION=1.16.11
# Sun, 20 Mar 2022 02:27:11 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sun, 20 Mar 2022 02:27:16 GMT
ENV NODE_ENV=production
# Sun, 20 Mar 2022 02:27:19 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sun, 20 Mar 2022 02:27:22 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sun, 20 Mar 2022 02:27:25 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sun, 20 Mar 2022 02:27:29 GMT
VOLUME [/var/lib/eg]
# Sun, 20 Mar 2022 02:27:31 GMT
EXPOSE 8080 9876
# Sun, 20 Mar 2022 02:27:34 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sun, 20 Mar 2022 02:27:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 02:27:40 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:eef85fcc847498263d979ef7ec75680d05e90815eb83a9ec4db135b990c0d8b8`  
		Last Modified: Thu, 17 Mar 2022 11:15:15 GMT  
		Size: 2.8 MB (2814051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520f8182ba461712aeb72b3184ad1ab550f0da9aac8b041e3d128bd5081ef25`  
		Last Modified: Sat, 19 Mar 2022 02:17:11 GMT  
		Size: 27.1 MB (27136542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2b8da92dd97b67e17b234dec546b6585e21ba0d0042599f5679b16af964ebf`  
		Last Modified: Sat, 19 Mar 2022 02:17:07 GMT  
		Size: 2.4 MB (2438373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fdb16adbd7fbe1d7ec85d6a222900e9ce2313cd9b63a1bb8dad84d75d43a66`  
		Last Modified: Sat, 19 Mar 2022 02:17:06 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec81d857a561a987e15c89297b8275e3f386a9e87d9c0edd2729c63ba7da477`  
		Last Modified: Sun, 20 Mar 2022 02:28:09 GMT  
		Size: 10.1 MB (10133259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b41adb5d74866605ffef0cba06c0cfd1196e97b14395547321c3b827a4eb08`  
		Last Modified: Sun, 20 Mar 2022 02:28:06 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:1.x` - linux; s390x

```console
$ docker pull express-gateway@sha256:5477d675e36dc9ffe5bf4feb73731848dc5ceaeb3394264de1f53eebfdc14ee7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39943968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e75c9ba837f5d9b352a127b02bea42dedde22cd405d2336407ee3b88593fdc0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 22:37:27 GMT
ENV NODE_VERSION=12.22.11
# Fri, 18 Mar 2022 22:57:09 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 22:57:10 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:57:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 22:57:14 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:57:14 GMT
CMD ["node"]
# Fri, 18 Mar 2022 23:12:34 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Fri, 18 Mar 2022 23:12:34 GMT
ARG EG_VERSION=1.16.11
# Fri, 18 Mar 2022 23:12:53 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Fri, 18 Mar 2022 23:12:55 GMT
ENV NODE_ENV=production
# Fri, 18 Mar 2022 23:12:56 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Fri, 18 Mar 2022 23:12:56 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Fri, 18 Mar 2022 23:12:56 GMT
ENV CHOKIDAR_USEPOLLING=true
# Fri, 18 Mar 2022 23:12:56 GMT
VOLUME [/var/lib/eg]
# Fri, 18 Mar 2022 23:12:56 GMT
EXPOSE 8080 9876
# Fri, 18 Mar 2022 23:12:56 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:12:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:12:56 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc7615e0810b845e7a7a67083a6fe5e8f87b1a58b6097a02a34bc03be25367`  
		Last Modified: Fri, 18 Mar 2022 23:11:09 GMT  
		Size: 24.8 MB (24802008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa5357697f7e0751e355eafc575990ac0869a5e684f10b8baee5a1ed80d6d8a`  
		Last Modified: Fri, 18 Mar 2022 23:11:05 GMT  
		Size: 2.4 MB (2440644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58972249e28a7f4674026b4d9d987ee90c90e9a8c3ef62722da31f781c74ab32`  
		Last Modified: Fri, 18 Mar 2022 23:11:05 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a46cee6202c0abe148ea21a1e7645a8aa3de118ebe01fca5ee1f57747ff833`  
		Last Modified: Fri, 18 Mar 2022 23:13:19 GMT  
		Size: 10.1 MB (10098658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466d9746795cef0cf0d6ad6e38cef1507bd55e7da3614926bcf9c1941f5a234b`  
		Last Modified: Fri, 18 Mar 2022 23:13:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `express-gateway:latest`

```console
$ docker pull express-gateway@sha256:30fefcd985a841fb1f0f5eaef659cadca137dcf5a341307e8b5336db23cd1934
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `express-gateway:latest` - linux; amd64

```console
$ docker pull express-gateway@sha256:9fdb12a4f04ea0d0ded3a4183f279993a20df1e387b345e5541c263729caa8ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40177423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b19671d273209ca1a7ebe3b9a0c66f26677c9a9676e3d0eb44e0c1c0aba532ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 21:54:38 GMT
ENV NODE_VERSION=12.22.11
# Fri, 18 Mar 2022 21:54:50 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 21:54:50 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:54:56 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 21:54:56 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:54:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:54:56 GMT
CMD ["node"]
# Sat, 19 Mar 2022 00:10:40 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 19 Mar 2022 00:10:40 GMT
ARG EG_VERSION=1.16.11
# Sat, 19 Mar 2022 00:11:04 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 19 Mar 2022 00:11:05 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 00:11:05 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 19 Mar 2022 00:11:05 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 19 Mar 2022 00:11:05 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 19 Mar 2022 00:11:05 GMT
VOLUME [/var/lib/eg]
# Sat, 19 Mar 2022 00:11:05 GMT
EXPOSE 8080 9876
# Sat, 19 Mar 2022 00:11:06 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:11:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:11:06 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4df20eca50beea3c4188568910712f5683e5d0497ba399c818213b73180e273`  
		Last Modified: Fri, 18 Mar 2022 22:17:11 GMT  
		Size: 24.9 MB (24907620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb8006bb2b0d1233915059f504c0e715fd8f43c409ef20878acafb279c5a785`  
		Last Modified: Fri, 18 Mar 2022 22:17:06 GMT  
		Size: 2.4 MB (2357895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f64245aee5e460a1afa73858263e95c471cde81f3bb6ebdf6a3d4eda0012fb`  
		Last Modified: Fri, 18 Mar 2022 22:17:05 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cc5e35bdccf9b4518dd259bc7e3dc9f5a52644e2c4bce27d94b9c584e9ba74`  
		Last Modified: Sat, 19 Mar 2022 00:11:22 GMT  
		Size: 10.1 MB (10098321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9169b1660824e9f509de7cb767b624f42b9cd6771f692b4a34b52f00d3ba5b9`  
		Last Modified: Sat, 19 Mar 2022 00:11:19 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:latest` - linux; arm64 variant v8

```console
$ docker pull express-gateway@sha256:8420121d1d31ca646480565f8e735646200f903502c5b325df4b78d3321406f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40060865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26d80065dd102c820850bf947f35e459416a10edae8f4ab3665c420e1c61f723`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 00:13:22 GMT
ENV NODE_VERSION=12.22.11
# Sat, 19 Mar 2022 00:31:55 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 19 Mar 2022 00:31:56 GMT
ENV YARN_VERSION=1.22.17
# Sat, 19 Mar 2022 00:32:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 19 Mar 2022 00:32:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:32:06 GMT
CMD ["node"]
# Sat, 19 Mar 2022 17:52:35 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 19 Mar 2022 17:52:35 GMT
ARG EG_VERSION=1.16.11
# Sat, 19 Mar 2022 17:53:00 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 19 Mar 2022 17:53:01 GMT
ENV NODE_ENV=production
# Sat, 19 Mar 2022 17:53:02 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 19 Mar 2022 17:53:03 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 19 Mar 2022 17:53:04 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 19 Mar 2022 17:53:05 GMT
VOLUME [/var/lib/eg]
# Sat, 19 Mar 2022 17:53:06 GMT
EXPOSE 8080 9876
# Sat, 19 Mar 2022 17:53:08 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 19 Mar 2022 17:53:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 17:53:09 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4804b7fb3c60c6fd6d87ca3cea8f51583c5fa4e023d214248111e38ed597f`  
		Last Modified: Sat, 19 Mar 2022 00:56:50 GMT  
		Size: 24.8 MB (24803893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aa9e6c8534e79c8ff44bec0a6845088d5b1fe5cbb9a4f3657cbd24d84edee8`  
		Last Modified: Sat, 19 Mar 2022 00:56:46 GMT  
		Size: 2.4 MB (2438217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91d150c92f25556d9b1bdce6869f06d0ac18f645b941beaf980ccf0610fc4a8`  
		Last Modified: Sat, 19 Mar 2022 00:56:45 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16240801f297dcde4abf0883a71ef9c4b20e54595525acfb587f577a745cd968`  
		Last Modified: Sat, 19 Mar 2022 17:53:32 GMT  
		Size: 10.1 MB (10103002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625c6593e1c334a62aaa85ab9a088f4f929d723c13e761ce33ce5bceac2e7c1f`  
		Last Modified: Sat, 19 Mar 2022 17:53:29 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:latest` - linux; ppc64le

```console
$ docker pull express-gateway@sha256:26d4baad39231541adfce1bb6ecab7f45fe52d81695fcad5db4f49cc0ee136f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42523175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a057efda589b92876538c5d5f75653fafb897c037d7580ff004e50db6c3e22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 11:14:04 GMT
ADD file:ddc94e1e084c05807db26adcc95b47a137fa47fb391e75998b338ada65e00c1c in / 
# Thu, 17 Mar 2022 11:14:09 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 23:44:23 GMT
ENV NODE_VERSION=12.22.11
# Sat, 19 Mar 2022 00:04:36 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 19 Mar 2022 00:04:47 GMT
ENV YARN_VERSION=1.22.17
# Sat, 19 Mar 2022 00:05:03 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 19 Mar 2022 00:05:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 19 Mar 2022 00:05:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 00:05:12 GMT
CMD ["node"]
# Sun, 20 Mar 2022 02:26:13 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sun, 20 Mar 2022 02:26:16 GMT
ARG EG_VERSION=1.16.11
# Sun, 20 Mar 2022 02:27:11 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sun, 20 Mar 2022 02:27:16 GMT
ENV NODE_ENV=production
# Sun, 20 Mar 2022 02:27:19 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sun, 20 Mar 2022 02:27:22 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sun, 20 Mar 2022 02:27:25 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sun, 20 Mar 2022 02:27:29 GMT
VOLUME [/var/lib/eg]
# Sun, 20 Mar 2022 02:27:31 GMT
EXPOSE 8080 9876
# Sun, 20 Mar 2022 02:27:34 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sun, 20 Mar 2022 02:27:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 20 Mar 2022 02:27:40 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:eef85fcc847498263d979ef7ec75680d05e90815eb83a9ec4db135b990c0d8b8`  
		Last Modified: Thu, 17 Mar 2022 11:15:15 GMT  
		Size: 2.8 MB (2814051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520f8182ba461712aeb72b3184ad1ab550f0da9aac8b041e3d128bd5081ef25`  
		Last Modified: Sat, 19 Mar 2022 02:17:11 GMT  
		Size: 27.1 MB (27136542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2b8da92dd97b67e17b234dec546b6585e21ba0d0042599f5679b16af964ebf`  
		Last Modified: Sat, 19 Mar 2022 02:17:07 GMT  
		Size: 2.4 MB (2438373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fdb16adbd7fbe1d7ec85d6a222900e9ce2313cd9b63a1bb8dad84d75d43a66`  
		Last Modified: Sat, 19 Mar 2022 02:17:06 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec81d857a561a987e15c89297b8275e3f386a9e87d9c0edd2729c63ba7da477`  
		Last Modified: Sun, 20 Mar 2022 02:28:09 GMT  
		Size: 10.1 MB (10133259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b41adb5d74866605ffef0cba06c0cfd1196e97b14395547321c3b827a4eb08`  
		Last Modified: Sun, 20 Mar 2022 02:28:06 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:latest` - linux; s390x

```console
$ docker pull express-gateway@sha256:5477d675e36dc9ffe5bf4feb73731848dc5ceaeb3394264de1f53eebfdc14ee7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39943968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e75c9ba837f5d9b352a127b02bea42dedde22cd405d2336407ee3b88593fdc0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 22:37:27 GMT
ENV NODE_VERSION=12.22.11
# Fri, 18 Mar 2022 22:57:09 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 22:57:10 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 22:57:14 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 22:57:14 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 22:57:14 GMT
CMD ["node"]
# Fri, 18 Mar 2022 23:12:34 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Fri, 18 Mar 2022 23:12:34 GMT
ARG EG_VERSION=1.16.11
# Fri, 18 Mar 2022 23:12:53 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Fri, 18 Mar 2022 23:12:55 GMT
ENV NODE_ENV=production
# Fri, 18 Mar 2022 23:12:56 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Fri, 18 Mar 2022 23:12:56 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Fri, 18 Mar 2022 23:12:56 GMT
ENV CHOKIDAR_USEPOLLING=true
# Fri, 18 Mar 2022 23:12:56 GMT
VOLUME [/var/lib/eg]
# Fri, 18 Mar 2022 23:12:56 GMT
EXPOSE 8080 9876
# Fri, 18 Mar 2022 23:12:56 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Fri, 18 Mar 2022 23:12:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 23:12:56 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dc7615e0810b845e7a7a67083a6fe5e8f87b1a58b6097a02a34bc03be25367`  
		Last Modified: Fri, 18 Mar 2022 23:11:09 GMT  
		Size: 24.8 MB (24802008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fa5357697f7e0751e355eafc575990ac0869a5e684f10b8baee5a1ed80d6d8a`  
		Last Modified: Fri, 18 Mar 2022 23:11:05 GMT  
		Size: 2.4 MB (2440644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58972249e28a7f4674026b4d9d987ee90c90e9a8c3ef62722da31f781c74ab32`  
		Last Modified: Fri, 18 Mar 2022 23:11:05 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a46cee6202c0abe148ea21a1e7645a8aa3de118ebe01fca5ee1f57747ff833`  
		Last Modified: Fri, 18 Mar 2022 23:13:19 GMT  
		Size: 10.1 MB (10098658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466d9746795cef0cf0d6ad6e38cef1507bd55e7da3614926bcf9c1941f5a234b`  
		Last Modified: Fri, 18 Mar 2022 23:13:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
