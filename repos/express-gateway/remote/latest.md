## `express-gateway:latest`

```console
$ docker pull express-gateway@sha256:ba93881101bb65b0eec447944ae822e35988c488b7f829538f501004fd90ae49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `express-gateway:latest` - linux; amd64

```console
$ docker pull express-gateway@sha256:5950b112c6388e4dfcc158ac7c0e77fcc0e568261e3c62afcb0abb84d0f65365
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40117066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d88e8f9476b6225bfc0db829ddca3222c0df22305030ff42eaab0bedbefa3b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:02:12 GMT
ENV NODE_VERSION=12.22.7
# Sat, 13 Nov 2021 11:02:19 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 13 Nov 2021 11:02:20 GMT
ENV YARN_VERSION=1.22.15
# Sat, 13 Nov 2021 11:02:25 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 13 Nov 2021 11:02:25 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 13 Nov 2021 11:02:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:02:25 GMT
CMD ["node"]
# Sat, 13 Nov 2021 16:05:46 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 13 Nov 2021 16:05:46 GMT
ARG EG_VERSION=1.16.11
# Sat, 13 Nov 2021 16:06:06 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 13 Nov 2021 16:06:06 GMT
ENV NODE_ENV=production
# Sat, 13 Nov 2021 16:06:07 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 13 Nov 2021 16:06:07 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 13 Nov 2021 16:06:07 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 13 Nov 2021 16:06:07 GMT
VOLUME [/var/lib/eg]
# Sat, 13 Nov 2021 16:06:07 GMT
EXPOSE 8080 9876
# Sat, 13 Nov 2021 16:06:08 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 13 Nov 2021 16:06:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 16:06:08 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468000513d90bb27c6602b0b3bb5b7478173e555d9b905e768265694ad5c0192`  
		Last Modified: Sat, 13 Nov 2021 11:11:20 GMT  
		Size: 24.8 MB (24769217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4d2470b55737d054727607cda782e47ae7c2f3bdbf619d888d110943bb9278`  
		Last Modified: Sat, 13 Nov 2021 11:11:16 GMT  
		Size: 2.4 MB (2367572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26993460ce451dc85a494f9cfe75066895482fb4a53b23b40b99289548e96cb4`  
		Last Modified: Sat, 13 Nov 2021 11:11:15 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23840f413f31eb0a9c4b26ae5166854e2196e174490decf230996619ed57024a`  
		Last Modified: Sat, 13 Nov 2021 16:06:24 GMT  
		Size: 10.2 MB (10156349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42bff20007788ded5ed805ae168f73b5d59ebfdf5e355e410b5f76f37d2ffc93`  
		Last Modified: Sat, 13 Nov 2021 16:06:21 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:latest` - linux; arm64 variant v8

```console
$ docker pull express-gateway@sha256:84f2b6f9cd3aa2efb5babbab3db90d81239e244e34abef81a45f5ca778243888
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40112631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8227362ac00dce7d9d5987de0ebe0684a869fcc99eed984b3790341bc8c0cc90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:35:53 GMT
ENV NODE_VERSION=12.22.7
# Sat, 13 Nov 2021 05:57:05 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 13 Nov 2021 05:57:06 GMT
ENV YARN_VERSION=1.22.15
# Sat, 13 Nov 2021 05:57:13 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 13 Nov 2021 05:57:14 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 13 Nov 2021 05:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:57:15 GMT
CMD ["node"]
# Sat, 13 Nov 2021 15:58:14 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 13 Nov 2021 15:58:14 GMT
ARG EG_VERSION=1.16.11
# Sat, 13 Nov 2021 15:59:08 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 13 Nov 2021 15:59:09 GMT
ENV NODE_ENV=production
# Sat, 13 Nov 2021 15:59:09 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 13 Nov 2021 15:59:10 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 13 Nov 2021 15:59:11 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 13 Nov 2021 15:59:12 GMT
VOLUME [/var/lib/eg]
# Sat, 13 Nov 2021 15:59:13 GMT
EXPOSE 8080 9876
# Sat, 13 Nov 2021 15:59:15 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 13 Nov 2021 15:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 15:59:16 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ad98fc9bf3113afdedca24a42bedc69571abab432d27a18add2e6d86265220`  
		Last Modified: Sat, 13 Nov 2021 06:10:30 GMT  
		Size: 24.8 MB (24811831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbb38cbbf28dd8ec02e481d44f7f6cd4ba3dfe3cb08e08b891824e92c4adc48`  
		Last Modified: Sat, 13 Nov 2021 06:10:26 GMT  
		Size: 2.4 MB (2426075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e427954a01874bc5348e69b6cd7035328a29994c74245878a3f26fafdefb582`  
		Last Modified: Sat, 13 Nov 2021 06:10:26 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20674a66469abf23d18695e884621b6684ae827745c747b6b882a83b10521ad`  
		Last Modified: Sat, 13 Nov 2021 15:59:42 GMT  
		Size: 10.2 MB (10156081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4ef0b4439586f9e1af59dca6bcf0a743aee0f1118ad25d80f978fdc03a3ba5`  
		Last Modified: Sat, 13 Nov 2021 15:59:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:latest` - linux; ppc64le

```console
$ docker pull express-gateway@sha256:94c7cce465c1c31abd0ef1ba95a495d839e8f660dff3bf1301e194d4822a4a32
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42548263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb7fec0d5a32d60b8e68d4edcabf1e5d5fd7759c5a5116e9813898c6e84d483c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:11:29 GMT
ENV NODE_VERSION=12.22.7
# Sat, 13 Nov 2021 11:32:32 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 13 Nov 2021 11:32:41 GMT
ENV YARN_VERSION=1.22.15
# Sat, 13 Nov 2021 11:32:55 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 13 Nov 2021 11:32:56 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 13 Nov 2021 11:32:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:33:04 GMT
CMD ["node"]
# Sat, 13 Nov 2021 18:17:31 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 13 Nov 2021 18:17:41 GMT
ARG EG_VERSION=1.16.11
# Sat, 13 Nov 2021 18:18:33 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 13 Nov 2021 18:18:41 GMT
ENV NODE_ENV=production
# Sat, 13 Nov 2021 18:18:46 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 13 Nov 2021 18:18:49 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 13 Nov 2021 18:18:53 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 13 Nov 2021 18:18:56 GMT
VOLUME [/var/lib/eg]
# Sat, 13 Nov 2021 18:19:02 GMT
EXPOSE 8080 9876
# Sat, 13 Nov 2021 18:19:03 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 13 Nov 2021 18:19:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 18:19:15 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc5e8928961b338cf25c838faa2046993d2ccb4ce534a1cfededef94bc5f281`  
		Last Modified: Sat, 13 Nov 2021 11:48:40 GMT  
		Size: 27.1 MB (27146999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccddeff5a471436a07e1e6b45b6361705ae2af05bb76403daf5dca2ba1889f5`  
		Last Modified: Sat, 13 Nov 2021 11:48:34 GMT  
		Size: 2.4 MB (2426441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1afa5d96596181e27f2e2a0dc2e69d84fba665d44b6d12f2c96c1d2993e8a95`  
		Last Modified: Sat, 13 Nov 2021 11:48:34 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc122172ea5c031af2527a0ff8f514a41bdcaaab5ac98954548502c4e8eab6d`  
		Last Modified: Sat, 13 Nov 2021 18:19:40 GMT  
		Size: 10.2 MB (10156408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775a21e509ac11c03bd1adf7d937394836fd24a9b0c8fcf8c49f6826eedd8876`  
		Last Modified: Sat, 13 Nov 2021 18:19:36 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `express-gateway:latest` - linux; s390x

```console
$ docker pull express-gateway@sha256:4bb71c2cf71abc7e35193cdbd5368ee2ea0d494046aae123272d52b286dc01be
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (40010230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2dd0dac5a7222ed6c8ad2ed859ca5eefe9b46fea65d7cec40b007799efc3c6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node","-e","require('express-gateway')().run();"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 03:27:56 GMT
ENV NODE_VERSION=12.22.7
# Sat, 13 Nov 2021 03:46:48 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c8672a664087e96b4e2804caf77a0aaa8c1375ae6b378edb220a678155383a81"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Sat, 13 Nov 2021 03:46:50 GMT
ENV YARN_VERSION=1.22.15
# Sat, 13 Nov 2021 03:46:53 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Sat, 13 Nov 2021 03:46:54 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:46:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 03:46:54 GMT
CMD ["node"]
# Sat, 13 Nov 2021 07:21:49 GMT
LABEL maintainer=Vincenzo Chianese, vincenzo@express-gateway.io
# Sat, 13 Nov 2021 07:21:49 GMT
ARG EG_VERSION=1.16.11
# Sat, 13 Nov 2021 07:22:09 GMT
# ARGS: EG_VERSION=1.16.11
RUN yarn global add express-gateway@$EG_VERSION && yarn cache clean
# Sat, 13 Nov 2021 07:22:11 GMT
ENV NODE_ENV=production
# Sat, 13 Nov 2021 07:22:11 GMT
ENV NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/
# Sat, 13 Nov 2021 07:22:11 GMT
ENV EG_CONFIG_DIR=/var/lib/eg
# Sat, 13 Nov 2021 07:22:11 GMT
ENV CHOKIDAR_USEPOLLING=true
# Sat, 13 Nov 2021 07:22:11 GMT
VOLUME [/var/lib/eg]
# Sat, 13 Nov 2021 07:22:11 GMT
EXPOSE 8080 9876
# Sat, 13 Nov 2021 07:22:12 GMT
COPY file:9481e65ab3ccc3b910b8af90d3df04d9f70030b8f8a0cfcc390840936290aaab in /usr/local/bin/ 
# Sat, 13 Nov 2021 07:22:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 07:22:12 GMT
CMD ["node" "-e" "require('express-gateway')().run();"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50c445e7137e7671fffbe855c4e77f3122ecbfc6ca5fb6375658fda154cb1a8`  
		Last Modified: Sat, 13 Nov 2021 03:56:55 GMT  
		Size: 24.8 MB (24815136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d695163060e9995121625aa9cc34ec309722eba760ab38c2b3a2e076a99f25`  
		Last Modified: Sat, 13 Nov 2021 03:56:52 GMT  
		Size: 2.4 MB (2428550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9168cdc2cd694640f1c305e58759cf93b70044d71621280011bf7467abd94feb`  
		Last Modified: Sat, 13 Nov 2021 03:56:51 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6680eb6a417a4c5d0de0d59c39a68660201dd216c46674a2e6aa21600df200a7`  
		Last Modified: Sat, 13 Nov 2021 07:22:35 GMT  
		Size: 10.2 MB (10156324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8255e8a54e0c09066e446c7aea4521d008c0e3a4d503101c48a8c31e4ce39a85`  
		Last Modified: Sat, 13 Nov 2021 07:22:33 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
