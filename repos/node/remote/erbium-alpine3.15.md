## `node:erbium-alpine3.15`

```console
$ docker pull node@sha256:80e40de9063beb82ea366d7570d76cf6a74e1f0a4204648419a74cb00fa859ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `node:erbium-alpine3.15` - linux; amd64

```console
$ docker pull node@sha256:2acec71ae2d9fc85cbdf3d933f3e69d848b84668fdc12c666d4a1518d66c79bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30078602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:289073580657fac895183cb8b1335531ea2fc097f64b550ed1e07e1a4117b832`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

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

### `node:erbium-alpine3.15` - linux; arm variant v6

```console
$ docker pull node@sha256:a9ac837d2c3bfd3f8c7291f1191852f7d4fcbe97ef58e148f74893c6e766fd0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.2 MB (29225435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db8ca0d8304f406ce654929c7559bb0c66ba5deeead3680d7ab7a0df3b08c8c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 17 Mar 2022 02:26:45 GMT
ADD file:9c8618405ef54d562132919ffe49c862d014b402e0e4813b87bf01574fa04c0e in / 
# Thu, 17 Mar 2022 02:26:45 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 20:21:59 GMT
ENV NODE_VERSION=12.22.11
# Fri, 18 Mar 2022 20:38:43 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="c30c9ba214a8eb2db6199db9147f14ff2cbb0fc07e4517e3a8758f213cc71128"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       141F07595B7B3FFE74309A937405533BE57C7D57       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 20:38:44 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 20:38:53 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 20:38:53 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 20:38:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 20:38:54 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:787f016efa9bc7812361be134f731e845b97fba19169cf3615e7048c0412380e`  
		Last Modified: Thu, 17 Mar 2022 02:28:24 GMT  
		Size: 2.6 MB (2624973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d6d267df123c75010d632e508827c338c3fa42baf4859cb28cb511d86686d5`  
		Last Modified: Fri, 18 Mar 2022 20:49:11 GMT  
		Size: 24.2 MB (24170091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b961ac3c82e3e231565864ac72fbef0bde35ec51017de0df340c6821ae699fb`  
		Last Modified: Fri, 18 Mar 2022 20:49:01 GMT  
		Size: 2.4 MB (2429924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abf58c21e0f85c686a9cef0d751b686b89b22e6d1e1966c8dbd91c56bd37556`  
		Last Modified: Fri, 18 Mar 2022 20:49:00 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:erbium-alpine3.15` - linux; arm variant v7

```console
$ docker pull node@sha256:23720d93016d16f081d20901cea3cf08ac9dc56b61435456866ab8b60fc2a91e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.6 MB (28580167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2d854ad717023df3a6d69c51cc99bc8a375bc6c3c85c5856632eaba57b93eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 17 Mar 2022 09:26:34 GMT
ADD file:01e87d7f83dfb32fd8a1b7b889b923432c2e0516d79a4196e01ad0ad15e33d68 in / 
# Thu, 17 Mar 2022 09:26:35 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 16:31:34 GMT
ENV NODE_VERSION=12.22.10
# Fri, 18 Mar 2022 16:44:34 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="ec1e2f0c33a495002ffb1647159d8e17643e2f229c0f4fe2c1be33398f56b5f4"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 16:44:35 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 16:44:42 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 16:44:42 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 16:44:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 16:44:43 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:205cbce5da6d59acc17b2db4c1af7903ca3497b99d4bedb94ef66ace17303808`  
		Last Modified: Thu, 17 Mar 2022 09:28:11 GMT  
		Size: 2.4 MB (2427136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789368e4132ed283917897c5b8c01052e08e7acc0bffdcacdab1b17388e19986`  
		Last Modified: Fri, 18 Mar 2022 17:22:34 GMT  
		Size: 23.7 MB (23729472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee371157bf5e7a0034eedea73626473417ad013cdc7135bb52c921aca2d3a62`  
		Last Modified: Fri, 18 Mar 2022 17:22:19 GMT  
		Size: 2.4 MB (2423111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322cfd7c57ba3a9df2f078f34866f33bfe82af0c2304c7980ec20dbbe3f0abc3`  
		Last Modified: Fri, 18 Mar 2022 17:22:17 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:erbium-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull node@sha256:0e5053852c567c38ef67cb4a8cbe00343a2146f95e24b06c98291701044080ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29941313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:187c3bf384dce983e2d0d0b8b415d23efbe30d25152ae6805ac9a791af5832e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 13:25:39 GMT
ENV NODE_VERSION=12.22.10
# Thu, 17 Mar 2022 13:44:06 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="ec1e2f0c33a495002ffb1647159d8e17643e2f229c0f4fe2c1be33398f56b5f4"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Thu, 17 Mar 2022 13:44:07 GMT
ENV YARN_VERSION=1.22.17
# Thu, 17 Mar 2022 13:44:12 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Thu, 17 Mar 2022 13:44:13 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Thu, 17 Mar 2022 13:44:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 13:44:14 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de3dee09cba6c90a44dde061e15c9eaa6ba2585c8db7b808314f8f82ed9eacb`  
		Last Modified: Thu, 17 Mar 2022 14:01:04 GMT  
		Size: 24.8 MB (24793009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed0a03de1fc555a4413f40bd375959c09b8d8d1cfb19cb63bcff2824c5a3460`  
		Last Modified: Thu, 17 Mar 2022 14:01:00 GMT  
		Size: 2.4 MB (2433049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17735e52d9cade7b4b2b75777ee96cd49de65a47971f2859c5701e5e6f2982b9`  
		Last Modified: Thu, 17 Mar 2022 14:00:59 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:erbium-alpine3.15` - linux; ppc64le

```console
$ docker pull node@sha256:9aa0ad7dfbea814b6fe78e68bc259a2477f878ec1331820af4d3d253d40d55bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32377921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01da6d8a4ada6d6be8d92c13fcd14efac032d4eec1633ead06532cf829f62ebf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 17 Mar 2022 11:14:04 GMT
ADD file:ddc94e1e084c05807db26adcc95b47a137fa47fb391e75998b338ada65e00c1c in / 
# Thu, 17 Mar 2022 11:14:09 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 07:31:42 GMT
ENV NODE_VERSION=12.22.10
# Fri, 18 Mar 2022 07:57:30 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="ec1e2f0c33a495002ffb1647159d8e17643e2f229c0f4fe2c1be33398f56b5f4"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 18 Mar 2022 07:57:41 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 07:58:10 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 18 Mar 2022 07:58:13 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 07:58:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 07:58:30 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:eef85fcc847498263d979ef7ec75680d05e90815eb83a9ec4db135b990c0d8b8`  
		Last Modified: Thu, 17 Mar 2022 11:15:15 GMT  
		Size: 2.8 MB (2814051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb6e0e4d3a050763da2ad6c80eac325ad12e7166daeb1ccc92a3d92ba34ae4c`  
		Last Modified: Fri, 18 Mar 2022 08:42:10 GMT  
		Size: 27.1 MB (27130142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007c91ae02b36880f4e65e84b5d0eb044838cec306f9b6607889392ad8819f43`  
		Last Modified: Fri, 18 Mar 2022 08:42:05 GMT  
		Size: 2.4 MB (2433277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08d8fd69422465bed6e9ec39db3bd3bff5fd71f117c0ad208800f75d27f38a6`  
		Last Modified: Fri, 18 Mar 2022 08:42:04 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:erbium-alpine3.15` - linux; s390x

```console
$ docker pull node@sha256:7215c45b0652e12ca37236b4301e76e2fbe0cdc29c595165f7eb0d5ec713acf8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29844816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21c14ceebad16ab4b30d23d2ae610b2dc7139a9ffbe4a0343ece560a38fe48a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

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
