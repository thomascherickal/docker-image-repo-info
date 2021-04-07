## `mongo-express:latest`

```console
$ docker pull mongo-express@sha256:0cf297b43b7d5a0e049f16905010a31e5ba7db184c8c2f26b5ab705f0406342e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo-express:latest` - linux; amd64

```console
$ docker pull mongo-express@sha256:fb3a6da5c3e88204b2fcea2fbee6d7c837ec01393f11f0c5ede98ab55031dbaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46678791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5a1f58bcef120e2b7921e9a1fb18affb72fb9ad25e495b69dd062734bb53bc5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Wed, 07 Apr 2021 15:26:25 GMT
ENV NODE_VERSION=12.22.1
# Wed, 07 Apr 2021 15:26:31 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="b7c8a2cb26790b4cc21a69ea5896ecb3e88712a35dcd5f3ef1c799214ad1f5da"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Wed, 07 Apr 2021 15:26:32 GMT
ENV YARN_VERSION=1.22.5
# Wed, 07 Apr 2021 15:26:49 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Wed, 07 Apr 2021 15:26:49 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 07 Apr 2021 15:26:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Apr 2021 15:26:50 GMT
CMD ["node"]
# Wed, 07 Apr 2021 16:28:11 GMT
RUN apk add --no-cache bash tini
# Wed, 07 Apr 2021 16:28:12 GMT
EXPOSE 8081
# Wed, 07 Apr 2021 16:28:12 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Wed, 07 Apr 2021 16:28:12 GMT
ENV MONGO_EXPRESS=0.54.0
# Wed, 07 Apr 2021 16:28:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Wed, 07 Apr 2021 16:28:35 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Wed, 07 Apr 2021 16:28:35 GMT
WORKDIR /node_modules/mongo-express
# Wed, 07 Apr 2021 16:28:36 GMT
RUN cp config.default.js config.js
# Wed, 07 Apr 2021 16:28:36 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 07 Apr 2021 16:28:37 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acbbc96f494d8dc1e9251b7abeaa9c9f3b36f2d23e905761adfd946ff276327`  
		Last Modified: Wed, 07 Apr 2021 15:46:04 GMT  
		Size: 24.6 MB (24600861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387d9933a547f18c25ab51fdee57f95fb78d620147886d896d29a1c11824c0d5`  
		Last Modified: Wed, 07 Apr 2021 15:46:00 GMT  
		Size: 2.2 MB (2239502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2871dad4695816b0438bcd131bb0fa3f40e5e2d2bf6fa5bb35c245fa62ea5c5f`  
		Last Modified: Wed, 07 Apr 2021 15:45:58 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2d86c40b937786e6ffb2052359ac03d45589e09c31f1f0c27f0e45f846cd44`  
		Last Modified: Wed, 07 Apr 2021 16:28:54 GMT  
		Size: 789.3 KB (789316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585f4cee52ef0cdf914f8c3ecb052eb9ce1ce97be86a0657af4896ed33b9b46a`  
		Last Modified: Wed, 07 Apr 2021 16:28:57 GMT  
		Size: 16.2 MB (16229684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217117b9cef71a024378880860756e02c9b3f4f3908f036f387d7395dfe8af46`  
		Last Modified: Wed, 07 Apr 2021 16:28:54 GMT  
		Size: 654.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5a80f9dbbdd9683999528072fc169356ceb7e2f69317eac97cb6afbccf164d`  
		Last Modified: Wed, 07 Apr 2021 16:28:54 GMT  
		Size: 3.1 KB (3147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo-express:latest` - linux; arm64 variant v8

```console
$ docker pull mongo-express@sha256:62eb9e933d3996829520d8c8fb99527ffb17db7af7c44b8db0639d60ab6624c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46790357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1a94c2acda71aeefc258e76c50c4347e19aa06f3f892876a0a99f29893e34d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:02 GMT
ADD file:174ba1b913c5cf549fcdfc259e8e3aa8f49cea660865fd54b8aacb430602a783 in / 
# Wed, 31 Mar 2021 17:22:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:37:10 GMT
ENV NODE_VERSION=12.22.0
# Thu, 01 Apr 2021 01:47:14 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="9805fb554de70c7920aaa19b6eed9e464cd5b2b0b9d6e3f1cf6d7cb30fbb3baa"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Thu, 01 Apr 2021 01:47:17 GMT
ENV YARN_VERSION=1.22.5
# Thu, 01 Apr 2021 01:47:22 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Thu, 01 Apr 2021 01:47:23 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:47:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 01:47:25 GMT
CMD ["node"]
# Thu, 01 Apr 2021 02:21:15 GMT
RUN apk add --no-cache bash tini
# Thu, 01 Apr 2021 02:21:16 GMT
EXPOSE 8081
# Thu, 01 Apr 2021 02:21:17 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Thu, 01 Apr 2021 02:21:18 GMT
ENV MONGO_EXPRESS=0.54.0
# Thu, 01 Apr 2021 02:21:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Thu, 01 Apr 2021 02:21:51 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Thu, 01 Apr 2021 02:21:52 GMT
WORKDIR /node_modules/mongo-express
# Thu, 01 Apr 2021 02:21:55 GMT
RUN cp config.default.js config.js
# Thu, 01 Apr 2021 02:21:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 01 Apr 2021 02:21:57 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:a3cf95b55367cb73f51318ee9c854def347373482336709ca1882a5d4c20b7c7`  
		Last Modified: Wed, 31 Mar 2021 17:23:00 GMT  
		Size: 2.7 MB (2725871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1039068a45e1e16e6b7ef42ee38970c7b77af420c9126cb450f270770c1702`  
		Last Modified: Thu, 01 Apr 2021 02:19:01 GMT  
		Size: 24.7 MB (24741474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdce6357f4432027dc529543577f87737d201c6ddc5819ecf17533fc6c2bdebe`  
		Last Modified: Thu, 01 Apr 2021 02:18:54 GMT  
		Size: 2.3 MB (2302821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2498e5d99d49df0fb35ac83b69fe6e3b945a37a13b7b63a5410c8be07f22f22`  
		Last Modified: Thu, 01 Apr 2021 02:18:54 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a2b68c1b13c037b8c3ca0fc568b33218e01d6225a74d50b4e9f873c9901ac3`  
		Last Modified: Thu, 01 Apr 2021 02:22:16 GMT  
		Size: 800.1 KB (800062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad84ca6c25b325b686deab4056c23c050af4bf077dd9f95b0969e19b96703be`  
		Last Modified: Thu, 01 Apr 2021 02:22:22 GMT  
		Size: 16.2 MB (16216046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d07784d0a2840102a59c36c172a70ecf617750cfb8eb2f6f9d19424e025efc`  
		Last Modified: Thu, 01 Apr 2021 02:22:16 GMT  
		Size: 653.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4206181e5370ed85c4f0ab36abb8f3031ded8ecff7a619d6f10fa2ceb85c8664`  
		Last Modified: Thu, 01 Apr 2021 02:22:16 GMT  
		Size: 3.1 KB (3148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
