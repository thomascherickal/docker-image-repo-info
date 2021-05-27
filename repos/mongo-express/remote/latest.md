## `mongo-express:latest`

```console
$ docker pull mongo-express@sha256:1df4d44b722aadb31335105972c62e9c971e015f83e68623cec24e6a1a3f0d38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo-express:latest` - linux; amd64

```console
$ docker pull mongo-express@sha256:daa7305624df060553b71a1e4947353409dd838860bb487eac40603e96169777
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46691989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51fc3f2af7a1f02f982ac2dd0aa139d962cd7e048e7a2c9f54c300f4aed58711`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:56 GMT
ADD file:282b9d56236cae29600bf8b698cb0a865ab17db7beea0be6870f9de63e7d4f80 in / 
# Wed, 14 Apr 2021 19:19:56 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:20:13 GMT
ENV NODE_VERSION=12.22.1
# Wed, 14 Apr 2021 23:20:18 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="b7c8a2cb26790b4cc21a69ea5896ecb3e88712a35dcd5f3ef1c799214ad1f5da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 14 Apr 2021 23:20:19 GMT
ENV YARN_VERSION=1.22.5
# Wed, 14 Apr 2021 23:20:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 14 Apr 2021 23:20:22 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:20:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:20:23 GMT
CMD ["node"]
# Thu, 15 Apr 2021 09:44:21 GMT
RUN apk add --no-cache bash tini
# Thu, 15 Apr 2021 09:44:21 GMT
EXPOSE 8081
# Thu, 15 Apr 2021 09:44:21 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Thu, 15 Apr 2021 09:44:21 GMT
ENV MONGO_EXPRESS=0.54.0
# Thu, 15 Apr 2021 09:44:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Thu, 15 Apr 2021 09:44:41 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Thu, 15 Apr 2021 09:44:42 GMT
WORKDIR /node_modules/mongo-express
# Thu, 15 Apr 2021 09:44:43 GMT
RUN cp config.default.js config.js
# Thu, 15 Apr 2021 09:44:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 09:44:43 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:ddad3d7c1e96adf9153f8921a7c9790f880a390163df453be1566e9ef0d546e0`  
		Last Modified: Wed, 14 Apr 2021 19:21:03 GMT  
		Size: 2.8 MB (2816246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8370f05d5d4a08dba62a139bd9286c42712a66ea263d39c0914d4a37eafe72`  
		Last Modified: Wed, 14 Apr 2021 23:28:43 GMT  
		Size: 24.6 MB (24601281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a8563b7feaa9ea167906666dd1173a08512f3f84acaaa6dd4cd3261d15fbf9`  
		Last Modified: Wed, 14 Apr 2021 23:28:42 GMT  
		Size: 2.2 MB (2239488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119c7e14957d3c5cab0ae2e0748bbd997a7a54f01b668d939e5bf656ad6dd585`  
		Last Modified: Wed, 14 Apr 2021 23:28:38 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06612553eefe3d25ae80e5c86bd6422ceb45ebf0344de8df4ef76f852d50b98`  
		Last Modified: Thu, 15 Apr 2021 09:44:57 GMT  
		Size: 789.3 KB (789319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931f05f69fde839b475abef494a9dd4ffdcc2d7206dbd7b3eff5882ba2f1bf54`  
		Last Modified: Thu, 15 Apr 2021 09:44:59 GMT  
		Size: 16.2 MB (16241570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2766ec5ce375e650e1a96aa2d2030d3506bb744938f89c3681dedddcda5f30f0`  
		Last Modified: Thu, 15 Apr 2021 09:44:57 GMT  
		Size: 656.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60269e588ca20cee53491a4d13c5f6bf050585967a274258b16e4d5cb05bba4`  
		Last Modified: Thu, 15 Apr 2021 09:44:57 GMT  
		Size: 3.1 KB (3148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo-express:latest` - linux; arm64 variant v8

```console
$ docker pull mongo-express@sha256:a19c2920b87ea82a54b2aca7f3937456a89e66103332b4d785afaa951554efe4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46860185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6d5086e83839a7ffd981d0cc9f9abbb19594995b75785e604c259f9fc4b4e85`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Wed, 14 Apr 2021 18:43:05 GMT
ADD file:62109d08b751b6f41eb8dc5dcb3ea6b553619ef0a58a40685faa749a20c3b051 in / 
# Wed, 14 Apr 2021 18:43:06 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 07:17:18 GMT
ENV NODE_VERSION=12.22.1
# Thu, 27 May 2021 07:44:08 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="b7c8a2cb26790b4cc21a69ea5896ecb3e88712a35dcd5f3ef1c799214ad1f5da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Thu, 27 May 2021 07:44:08 GMT
ENV YARN_VERSION=1.22.5
# Thu, 27 May 2021 07:44:11 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Thu, 27 May 2021 07:44:11 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 27 May 2021 07:44:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 May 2021 07:44:11 GMT
CMD ["node"]
# Thu, 27 May 2021 16:38:38 GMT
RUN apk add --no-cache bash tini
# Thu, 27 May 2021 16:38:39 GMT
EXPOSE 8081
# Thu, 27 May 2021 16:38:39 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Thu, 27 May 2021 16:38:39 GMT
ENV MONGO_EXPRESS=0.54.0
# Thu, 27 May 2021 16:38:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Thu, 27 May 2021 16:38:56 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Thu, 27 May 2021 16:38:57 GMT
WORKDIR /node_modules/mongo-express
# Thu, 27 May 2021 16:38:57 GMT
RUN cp config.default.js config.js
# Thu, 27 May 2021 16:38:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 27 May 2021 16:38:58 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:535256e01bcb9590f56b9b2a053648a1d98fbe4dc0fd34c1fc3f32afec8c6e7b`  
		Last Modified: Wed, 14 Apr 2021 18:44:02 GMT  
		Size: 2.7 MB (2726928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d112730d1ddf25e7096d9cda2fc6d8c19a4d3fd4a792eefc0a437e242fa7f9a`  
		Last Modified: Thu, 27 May 2021 08:31:39 GMT  
		Size: 24.7 MB (24742409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cea8e18e70591923a3ef290b60a396a4c6930c06acb3c9beb4f2f97ea905acc`  
		Last Modified: Thu, 27 May 2021 08:31:35 GMT  
		Size: 2.3 MB (2302943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedec78921eb58b0fc0a154f7f65128892611eecea935ad1728aa86225e88da`  
		Last Modified: Thu, 27 May 2021 08:31:34 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7c3c4226dfa6c97cd9dc04e8ad7795858ad969397c90861b17feca18fe9a02`  
		Last Modified: Thu, 27 May 2021 16:39:14 GMT  
		Size: 800.1 KB (800079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3258b59ed4cb832895a01205ab7d9e2ceb6d85b03ad86c05ef3a3257dd1090`  
		Last Modified: Thu, 27 May 2021 16:39:17 GMT  
		Size: 16.3 MB (16283739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2006e6b0ca5e6deb8b0f6a72086709a714ad46043186813bd5eb5f4eba6ec150`  
		Last Modified: Thu, 27 May 2021 16:39:14 GMT  
		Size: 656.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cc26039942e21b3f0f94699a503c2c84573470740319ff97098348a7beb890`  
		Last Modified: Thu, 27 May 2021 16:39:14 GMT  
		Size: 3.1 KB (3149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
