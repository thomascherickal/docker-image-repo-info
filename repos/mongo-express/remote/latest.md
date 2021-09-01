## `mongo-express:latest`

```console
$ docker pull mongo-express@sha256:4a3524090bf4fe750aa84bc70a145569411541ee26f81388f929fc2aa3fe0ab5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo-express:latest` - linux; amd64

```console
$ docker pull mongo-express@sha256:9a171720228e5a5c25b22fad10a9b50fe15a08610be376c755fe4fee3de4bb50
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49203814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3505d6fafd023867b8c886cb7e9fd4aa3a36be4f5234afaf341d4dda1f913da`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:31 GMT
ADD file:9d14b11183983923090d9e6d15cc51ee210466296e913bfefbfd580b3de59c95 in / 
# Tue, 31 Aug 2021 23:18:31 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 23:43:22 GMT
ENV NODE_VERSION=12.22.6
# Tue, 31 Aug 2021 23:43:28 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="0ce2b97ecbbd84f1a5ed13278ed6845d93c6454d8550730b247a990438dba322"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Tue, 31 Aug 2021 23:43:29 GMT
ENV YARN_VERSION=1.22.5
# Tue, 31 Aug 2021 23:43:33 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Tue, 31 Aug 2021 23:43:33 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 31 Aug 2021 23:43:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 23:43:34 GMT
CMD ["node"]
# Tue, 31 Aug 2021 23:54:11 GMT
RUN apk add --no-cache bash tini
# Tue, 31 Aug 2021 23:54:11 GMT
EXPOSE 8081
# Tue, 31 Aug 2021 23:54:12 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_URL=mongodb://mongo:27017 ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Tue, 31 Aug 2021 23:54:12 GMT
ENV MONGO_EXPRESS=1.0.0-alpha.4
# Tue, 31 Aug 2021 23:54:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Tue, 31 Aug 2021 23:54:36 GMT
COPY file:4835df10525ec6f18e6339ce0c331b087391dd3279d964040c96a41ba7bf90b7 in / 
# Tue, 31 Aug 2021 23:54:36 GMT
WORKDIR /node_modules/mongo-express
# Tue, 31 Aug 2021 23:54:38 GMT
RUN cp config.default.js config.js
# Tue, 31 Aug 2021 23:54:38 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 23:54:39 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:6a428f9f83b0a29f1fdd2ccccca19a9bab805a925b8eddf432a5a3d3da04afbc`  
		Last Modified: Tue, 31 Aug 2021 23:19:15 GMT  
		Size: 2.8 MB (2817307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fe2b74aff960282c3c01d80bbbb5b45a12e84f7e2ad3b65daac8f42351d5a6`  
		Last Modified: Tue, 31 Aug 2021 23:52:27 GMT  
		Size: 24.6 MB (24620306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7ab7725978320093e26b86ae395a5b6e50ab2d4888b9e2a6c2ffd447598da8`  
		Last Modified: Tue, 31 Aug 2021 23:52:22 GMT  
		Size: 2.2 MB (2239378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c9d3375a027db46ec3b2edda79e800652d66b831df7e740c719db6000dbaf0`  
		Last Modified: Tue, 31 Aug 2021 23:52:21 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431ea7b7cdc1de5c4b972eab4757041b70e1af781e793fd94619ce23f60f3fad`  
		Last Modified: Tue, 31 Aug 2021 23:55:35 GMT  
		Size: 789.3 KB (789321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f1119577a03a85bfec62c4d9cf442dfd7e74410b31c2c5c0b59222afc7e578`  
		Last Modified: Tue, 31 Aug 2021 23:55:38 GMT  
		Size: 18.7 MB (18733187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43753e526514a52202b14aad5cdd5e0572aca0a679e84f3f1036bdbd4e916db`  
		Last Modified: Tue, 31 Aug 2021 23:55:34 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ece1d58841edd67e61b1be06f7ab3257873ddc4d5ec561f339a6ad985ff787`  
		Last Modified: Tue, 31 Aug 2021 23:55:34 GMT  
		Size: 3.3 KB (3301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo-express:latest` - linux; arm64 variant v8

```console
$ docker pull mongo-express@sha256:a0b71986462ed68d5540f35391687649d1cd3b7f94274c134c4339935b8bf996
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49665530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4954c373ff8a557dbb7b8f11db4ac2c90bca272878879215c43baa6b68dd12ab`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:15 GMT
ADD file:62109d08b751b6f41eb8dc5dcb3ea6b553619ef0a58a40685faa749a20c3b051 in / 
# Tue, 15 Jun 2021 21:45:15 GMT
CMD ["/bin/sh"]
# Fri, 13 Aug 2021 00:37:08 GMT
ENV NODE_VERSION=12.22.5
# Fri, 13 Aug 2021 01:05:14 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="1c8ce0d58828faff84486dc116ec817595841c8578ed01266eb69e5383c73201"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python2     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Fri, 13 Aug 2021 01:05:15 GMT
ENV YARN_VERSION=1.22.5
# Fri, 13 Aug 2021 01:05:19 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Fri, 13 Aug 2021 01:05:19 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Fri, 13 Aug 2021 01:05:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Aug 2021 01:05:20 GMT
CMD ["node"]
# Fri, 13 Aug 2021 05:37:26 GMT
RUN apk add --no-cache bash tini
# Fri, 13 Aug 2021 05:37:26 GMT
EXPOSE 8081
# Fri, 13 Aug 2021 05:37:26 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_URL=mongodb://mongo:27017 ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 13 Aug 2021 05:37:27 GMT
ENV MONGO_EXPRESS=1.0.0-alpha.4
# Fri, 13 Aug 2021 05:37:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 13 Aug 2021 05:37:45 GMT
COPY file:4835df10525ec6f18e6339ce0c331b087391dd3279d964040c96a41ba7bf90b7 in / 
# Fri, 13 Aug 2021 05:37:45 GMT
WORKDIR /node_modules/mongo-express
# Fri, 13 Aug 2021 05:37:45 GMT
RUN cp config.default.js config.js
# Fri, 13 Aug 2021 05:37:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 13 Aug 2021 05:37:46 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:535256e01bcb9590f56b9b2a053648a1d98fbe4dc0fd34c1fc3f32afec8c6e7b`  
		Last Modified: Wed, 14 Apr 2021 18:44:02 GMT  
		Size: 2.7 MB (2726928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e414149edd27c9ce3ebb9bd5d290b80ab928b33e84d35daa94f1622bfb44d604`  
		Last Modified: Fri, 13 Aug 2021 02:54:09 GMT  
		Size: 24.7 MB (24739240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc231990eae4128bca49f53af35f0f4936e9e2561c4b92c6f0b6190e7a98806`  
		Last Modified: Fri, 13 Aug 2021 02:54:05 GMT  
		Size: 2.3 MB (2300072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af09d62bb408368e0df99a629882bb5927d34c8691d94f118cef6e766aad97c`  
		Last Modified: Fri, 13 Aug 2021 02:54:05 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df9729f81b660b84681866db94e9723f2144b1a3ef0082c31d73fa888ab3d2c`  
		Last Modified: Fri, 13 Aug 2021 05:38:33 GMT  
		Size: 800.1 KB (800073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ab175457c11f5d8a6325b7e696ea372842c6100f1ace032f80cd94eae197f0`  
		Last Modified: Fri, 13 Aug 2021 05:38:36 GMT  
		Size: 19.1 MB (19094904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c203f63a33f6537eea952d6c02f149a43553822ca5a9a53fe4306e15a93780d`  
		Last Modified: Fri, 13 Aug 2021 05:38:33 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1c99195022c62b9582fd71359c687718a6ac3bbe26afe67efeaa48f8115a7d`  
		Last Modified: Fri, 13 Aug 2021 05:38:33 GMT  
		Size: 3.3 KB (3301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
