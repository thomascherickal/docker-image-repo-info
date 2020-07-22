## `node:dubnium-alpine3.9`

```console
$ docker pull node@sha256:b468f5f08d126a8ca4fd2c27dd6b7e8e14e60bedcbd70d1600665e769e586882
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `node:dubnium-alpine3.9` - linux; amd64

```console
$ docker pull node@sha256:049566f8be83e3638d8ff8cc3f416a94d353c937eb7e7cf6dcf03d38b59a5949
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.5 MB (27464643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60e7ea7937d2517171e07c12150b78f8d2dbbfd3cde0691642ed90027185271`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 00:49:51 GMT
ENV NODE_VERSION=10.22.0
# Wed, 22 Jul 2020 00:50:01 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 22 Jul 2020 00:50:02 GMT
ENV YARN_VERSION=1.22.4
# Wed, 22 Jul 2020 00:50:07 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 22 Jul 2020 00:50:08 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 22 Jul 2020 00:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:50:09 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624b2df44f79422b3d496ca3486b9c5d1f38412e8b0628dc39fab2aee6a8203e`  
		Last Modified: Wed, 22 Jul 2020 00:55:45 GMT  
		Size: 22.3 MB (22346589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96cb8c116ca3de805a543a368a92396b75933ac6515c4a9bba4a771e0cb0de`  
		Last Modified: Wed, 22 Jul 2020 00:55:36 GMT  
		Size: 2.3 MB (2344359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bda82b94640bb53eaf0cff15375c8013f5b49fbf7f861521880b2ece6247bcb`  
		Last Modified: Wed, 22 Jul 2020 00:55:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:dubnium-alpine3.9` - linux; arm variant v6

```console
$ docker pull node@sha256:be189c90e2c6e776cb4a6e0b732a3035b259ad2394962f97ca637175765c7456
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.4 MB (26447169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ae07a83d8284055737dd46b6e2e2e0d2f890923207a5eac27b065a70d96c2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Tue, 21 Jul 2020 23:09:14 GMT
ENV NODE_VERSION=10.22.0
# Tue, 21 Jul 2020 23:14:42 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 21 Jul 2020 23:14:45 GMT
ENV YARN_VERSION=1.22.4
# Tue, 21 Jul 2020 23:14:59 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 21 Jul 2020 23:15:00 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 21 Jul 2020 23:15:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Jul 2020 23:15:02 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080341cacdf035b9747280515575004fd4205bca6d228d3f1b1c05f98a21090d`  
		Last Modified: Tue, 21 Jul 2020 23:28:39 GMT  
		Size: 21.5 MB (21526163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e66304b9fdadaff4bee24e749ce8912ad9561836c856682941a531f8bd48bad`  
		Last Modified: Tue, 21 Jul 2020 23:28:32 GMT  
		Size: 2.4 MB (2372000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2e5f28edc55e350f3674b05f20c65f649443f95fea7d41d24fcb53dd7b7fd5`  
		Last Modified: Tue, 21 Jul 2020 23:28:31 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:dubnium-alpine3.9` - linux; arm variant v7

```console
$ docker pull node@sha256:a91ba7fda7b152fcba0b1e3c70fc0c85498e37af7f61b4882c52e45181e37ec8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.9 MB (25904346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47e16298b21ec651a09f65c591a4e816e349d219ac32f6d3e7d7eded123ed620`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:56 GMT
ADD file:5cfee90da24e94bf9a1c0f2ba8e03667ab5be058c265cc072bd60517c5e37eb4 in / 
# Thu, 23 Apr 2020 22:04:58 GMT
CMD ["/bin/sh"]
# Wed, 22 Jul 2020 00:01:31 GMT
ENV NODE_VERSION=10.22.0
# Wed, 22 Jul 2020 00:06:36 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 22 Jul 2020 00:06:38 GMT
ENV YARN_VERSION=1.22.4
# Wed, 22 Jul 2020 00:06:44 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 22 Jul 2020 00:06:45 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 22 Jul 2020 00:06:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:06:46 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:ca413bedb4ea5c78f6e0893c7e6abe204eaa1a07d3fb0505e96e0c8d526108f7`  
		Last Modified: Thu, 23 Apr 2020 22:05:29 GMT  
		Size: 2.4 MB (2355563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5baf56f61dc589f106491a12facc91980f8b0f7a4d46b0cb0c59360ef6780905`  
		Last Modified: Wed, 22 Jul 2020 00:20:19 GMT  
		Size: 21.2 MB (21176760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d31622e26a71576d0b436b0dbdd0362690ae7014e122e0209a3aa08edd0b38`  
		Last Modified: Wed, 22 Jul 2020 00:20:11 GMT  
		Size: 2.4 MB (2371741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d3d4e5269892b185c24a061054959d1ef0f90e569823a86f2ded0931233715`  
		Last Modified: Wed, 22 Jul 2020 00:20:10 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:dubnium-alpine3.9` - linux; arm64 variant v8

```console
$ docker pull node@sha256:fb0026278913309fbe4d0b99e7d85158a9ffd675c5507275f0bae161c610dd27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27623240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fccd86fcd4ff4644cda86f7f6ac18bdb4dc0b4cdd4587c07d203e0860c6934da`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Tue, 21 Jul 2020 23:36:00 GMT
ENV NODE_VERSION=10.22.0
# Tue, 21 Jul 2020 23:41:30 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 21 Jul 2020 23:41:32 GMT
ENV YARN_VERSION=1.22.4
# Tue, 21 Jul 2020 23:41:37 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 21 Jul 2020 23:41:37 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 21 Jul 2020 23:41:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Jul 2020 23:41:39 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194b592029bc78898fce9cd91be9a9955a6fc63a44490e66491f47780e633b70`  
		Last Modified: Tue, 21 Jul 2020 23:57:15 GMT  
		Size: 22.5 MB (22516154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acee69a1e709e4f106d3987964947b319a0f62d27c4029bd33f91cfffa770690`  
		Last Modified: Tue, 21 Jul 2020 23:57:09 GMT  
		Size: 2.4 MB (2412337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6edd05225abb77bcec8658708f2f65d72d3ab7eecfe613dedbc5b0cbbddc71`  
		Last Modified: Tue, 21 Jul 2020 23:57:08 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:dubnium-alpine3.9` - linux; 386

```console
$ docker pull node@sha256:e8bf1ec9bce7bfdef8fec948188308ba82ab06910d9aea97d4ef88a02149dd81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27715735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eed9db795acdbd7ab7cbc381e9c8a2dc3ca42d09067ed80e92db12c936bdef3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 01:44:54 GMT
ENV NODE_VERSION=10.21.0
# Wed, 03 Jun 2020 02:15:53 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="355919f1ccf585c4078fffeff1e3d0a0e44855f5d84777bbf110db131093aafe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 03 Jun 2020 02:15:53 GMT
ENV YARN_VERSION=1.22.4
# Wed, 03 Jun 2020 02:15:57 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 03 Jun 2020 02:15:57 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 03 Jun 2020 02:15:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Jun 2020 02:15:58 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ddbbda772fb23608ff17e281576443f853422b35cbf1df132f44af3bbf5992`  
		Last Modified: Wed, 03 Jun 2020 03:13:17 GMT  
		Size: 22.6 MB (22578747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734c87823d6b33f47c637ba5e30c4ade0a434ce766926597e538f7f0a16049db`  
		Last Modified: Wed, 03 Jun 2020 03:13:11 GMT  
		Size: 2.4 MB (2366972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9afb5a6a9ba31a38bd2949a96ebd3afab35c693b2c9195f22ca525394b5d974`  
		Last Modified: Wed, 03 Jun 2020 03:13:11 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:dubnium-alpine3.9` - linux; ppc64le

```console
$ docker pull node@sha256:4b20d72f25e5ddfc257c24c93480939f28eb8b0125514a2397d57174cbe13e1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29542864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a2cfc2e09becaea0764a6125aa7e3963f54c22636596bb8131b847dfb387714`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 23 Apr 2020 20:41:14 GMT
ADD file:2eaa074d9379f98d31cc4112997e1c1bb55b3871574af6aee576cf1c5ed99645 in / 
# Thu, 23 Apr 2020 20:41:16 GMT
CMD ["/bin/sh"]
# Wed, 03 Jun 2020 07:15:27 GMT
ENV NODE_VERSION=10.21.0
# Wed, 03 Jun 2020 07:27:06 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="355919f1ccf585c4078fffeff1e3d0a0e44855f5d84777bbf110db131093aafe"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 03 Jun 2020 07:27:11 GMT
ENV YARN_VERSION=1.22.4
# Wed, 03 Jun 2020 07:27:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 03 Jun 2020 07:27:23 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 03 Jun 2020 07:27:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Jun 2020 07:27:27 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:16f2eaeeecc1446c304d41ae21441f168e376dc76733ec3a9f8f2d17119638a1`  
		Last Modified: Thu, 23 Apr 2020 20:41:57 GMT  
		Size: 2.8 MB (2787865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a2f445583f5fdcfd42831a1db3d1114373285cc9c153f2acd1afc36ae035c1`  
		Last Modified: Wed, 03 Jun 2020 08:10:16 GMT  
		Size: 24.3 MB (24347406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1c60759eebade54f2d7a1b5e7d19314572a931df2a5e78f4dbbf127b02d1a4`  
		Last Modified: Wed, 03 Jun 2020 08:09:51 GMT  
		Size: 2.4 MB (2407310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218816d283161e6bfc80ac60434855d312d9d71e1dff4655d77cb365bd69ac4c`  
		Last Modified: Wed, 03 Jun 2020 08:09:50 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:dubnium-alpine3.9` - linux; s390x

```console
$ docker pull node@sha256:31587a5dc3c8646eeca521a88e9575cf9a0735cce1b84a5f4bfd07f91965a990
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.2 MB (27245161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d480548de453b95e109a4024be7fa7775c14a5d9b06f94ee01ad4e13d1c95fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 23 Apr 2020 17:51:19 GMT
ADD file:87357838aa76ab358b68ac6734871df2dacb0b5918d89a091836f0d33264f803 in / 
# Thu, 23 Apr 2020 17:51:20 GMT
CMD ["/bin/sh"]
# Tue, 21 Jul 2020 23:07:17 GMT
ENV NODE_VERSION=10.22.0
# Tue, 21 Jul 2020 23:18:27 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="2afa21473a5eb8f407c52fe3bf08180630f3ac9541d52b98e99dbf4fe79f82d2"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 21 Jul 2020 23:18:29 GMT
ENV YARN_VERSION=1.22.4
# Tue, 21 Jul 2020 23:18:32 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 21 Jul 2020 23:18:32 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 21 Jul 2020 23:18:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Jul 2020 23:18:33 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:1aff3887737eb15ee1a53e92e8c87162b9caac2281ecb01242da00d1a32f5a04`  
		Last Modified: Thu, 23 Apr 2020 17:51:52 GMT  
		Size: 2.6 MB (2550329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be5b553eb8ef11230e5cfc86003ffb32ab535d11179083c49ba48ae3af589f2`  
		Last Modified: Tue, 21 Jul 2020 23:43:48 GMT  
		Size: 22.3 MB (22287354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b07563e789d2024d92725e85de0171bf846821b6ed412dc724a993de7bf41d`  
		Last Modified: Tue, 21 Jul 2020 23:43:45 GMT  
		Size: 2.4 MB (2407198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb92f0c6f8152ca34c55a3434a12b373264de945a46298b5897c2a454df1ab1c`  
		Last Modified: Tue, 21 Jul 2020 23:43:50 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
