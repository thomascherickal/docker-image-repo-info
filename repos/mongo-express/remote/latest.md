## `mongo-express:latest`

```console
$ docker pull mongo-express@sha256:f320d7547f788c44d8ea6301c51824205f3bca85f80749b5189340d885771dfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `mongo-express:latest` - linux; amd64

```console
$ docker pull mongo-express@sha256:d9476a62605f66379c5ff3283b67a12f79d196d0cfa73288852f5f8cb13b5c14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47144596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f843141ba2b11edcfd214904f17ff3a1a8b8d6ffe8ce268915190daf2724246f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 20:33:48 GMT
ENV NODE_VERSION=12.18.1
# Thu, 18 Jun 2020 20:33:54 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="dbe26351b57cabd0fd41a8ad5f688a4e9f2e1e037bd984c2fa14852e1ac46a94"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Thu, 18 Jun 2020 20:33:54 GMT
ENV YARN_VERSION=1.22.4
# Thu, 18 Jun 2020 20:33:56 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Thu, 18 Jun 2020 20:33:56 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 18 Jun 2020 20:33:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 20:33:57 GMT
CMD ["node"]
# Thu, 18 Jun 2020 20:52:50 GMT
RUN apk add --no-cache bash tini
# Thu, 18 Jun 2020 20:52:51 GMT
EXPOSE 8081
# Thu, 18 Jun 2020 20:52:51 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Thu, 18 Jun 2020 20:52:51 GMT
ENV MONGO_EXPRESS=0.54.0
# Thu, 18 Jun 2020 20:53:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Thu, 18 Jun 2020 20:53:10 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Thu, 18 Jun 2020 20:53:11 GMT
WORKDIR /node_modules/mongo-express
# Thu, 18 Jun 2020 20:53:11 GMT
RUN cp config.default.js config.js
# Thu, 18 Jun 2020 20:53:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 18 Jun 2020 20:53:12 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2b5366d6fa2ea4ed2878427ed706a5058f70b6042df071362c6ab52c5f5dbd`  
		Last Modified: Thu, 18 Jun 2020 20:36:55 GMT  
		Size: 24.7 MB (24653702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58676d466619a4615f0d7be9b5bd5945b473c6e3327603e7605ef5df5a1c4d9`  
		Last Modified: Thu, 18 Jun 2020 20:36:51 GMT  
		Size: 2.2 MB (2239158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acc70cf2ab68878010cc2e8aa3fb8fa043fafa0a909defb5358b9c37efef5f1`  
		Last Modified: Thu, 18 Jun 2020 20:36:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f683beee0282d140931d0e5cf242cd58f70b890a9d1d1abd7df5c647d2276176`  
		Last Modified: Thu, 18 Jun 2020 20:53:22 GMT  
		Size: 789.2 KB (789197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed70dd960bb915c395b81e96973ccdfea4ee7384d9502b7349ac0d4c97859aff`  
		Last Modified: Thu, 18 Jun 2020 20:53:25 GMT  
		Size: 16.6 MB (16645141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68a0553fde6f68781852ed194c8d552faa8e77c2904e8dcef52cd2b55e178cb`  
		Last Modified: Thu, 18 Jun 2020 20:53:22 GMT  
		Size: 655.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9f4c60cc33fddab4173c143bcfcb41900cbcd5323a86c8eb417852159e712a`  
		Last Modified: Thu, 18 Jun 2020 20:53:22 GMT  
		Size: 3.1 KB (3146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo-express:latest` - linux; arm64 variant v8

```console
$ docker pull mongo-express@sha256:f5f3da8b6d3e1ee72ef0c6d28a8f905cc7e4ce49da6d102d81e12e7d90548ad3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47270348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09eb76ec14e94c6c79746d4b2a8cf2a817a0a8d7b199d1d2cc2d4dc7d9741f42`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["mongo-express"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Thu, 18 Jun 2020 23:38:19 GMT
ENV NODE_VERSION=12.18.1
# Thu, 18 Jun 2020 23:48:54 GMT
RUN addgroup -g 1000 node     && adduser -u 1000 -G node -s /bin/sh -D node     && apk add --no-cache         libstdc++     && apk add --no-cache --virtual .build-deps         curl     && ARCH= && alpineArch="$(apk --print-arch)"       && case "${alpineArch##*-}" in         x86_64)           ARCH='x64'           CHECKSUM="dbe26351b57cabd0fd41a8ad5f688a4e9f2e1e037bd984c2fa14852e1ac46a94"           ;;         *) ;;       esac   && if [ -n "${CHECKSUM}" ]; then     set -eu;     curl -fsSLO --compressed "https://unofficial-builds.nodejs.org/download/release/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz";     echo "$CHECKSUM  node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" | sha256sum -c -       && tar -xJf "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz" -C /usr/local --strip-components=1 --no-same-owner       && ln -s /usr/local/bin/node /usr/local/bin/nodejs;   else     echo "Building from source"     && apk add --no-cache --virtual .build-deps-full         binutils-gold         g++         gcc         gnupg         libgcc         linux-headers         make         python     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xf "node-v$NODE_VERSION.tar.xz"     && cd "node-v$NODE_VERSION"     && ./configure     && make -j$(getconf _NPROCESSORS_ONLN) V=     && make install     && apk del .build-deps-full     && cd ..     && rm -Rf "node-v$NODE_VERSION"     && rm "node-v$NODE_VERSION.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt;   fi   && rm -f "node-v$NODE_VERSION-linux-$ARCH-musl.tar.xz"   && apk del .build-deps   && node --version   && npm --version
# Thu, 18 Jun 2020 23:48:56 GMT
ENV YARN_VERSION=1.22.4
# Thu, 18 Jun 2020 23:49:00 GMT
RUN apk add --no-cache --virtual .build-deps-yarn curl gnupg tar   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && apk del .build-deps-yarn   && yarn --version
# Thu, 18 Jun 2020 23:49:01 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 18 Jun 2020 23:49:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 23:49:02 GMT
CMD ["node"]
# Fri, 19 Jun 2020 00:22:50 GMT
RUN apk add --no-cache bash tini
# Fri, 19 Jun 2020 00:22:51 GMT
EXPOSE 8081
# Fri, 19 Jun 2020 00:22:51 GMT
ENV ME_CONFIG_EDITORTHEME=default ME_CONFIG_MONGODB_SERVER=mongo ME_CONFIG_MONGODB_ENABLE_ADMIN=true ME_CONFIG_BASICAUTH_USERNAME= ME_CONFIG_BASICAUTH_PASSWORD= VCAP_APP_HOST=0.0.0.0
# Fri, 19 Jun 2020 00:22:52 GMT
ENV MONGO_EXPRESS=0.54.0
# Fri, 19 Jun 2020 00:23:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .me-install-deps git; 	npm install mongo-express@$MONGO_EXPRESS; 	apk del --no-network .me-install-deps
# Fri, 19 Jun 2020 00:23:21 GMT
COPY file:ad71ad0a2a1967b86be9140686f9a9aa6f78dc470d2ec9de89cbf1a25e85b550 in / 
# Fri, 19 Jun 2020 00:23:22 GMT
WORKDIR /node_modules/mongo-express
# Fri, 19 Jun 2020 00:23:23 GMT
RUN cp config.default.js config.js
# Fri, 19 Jun 2020 00:23:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 19 Jun 2020 00:23:24 GMT
CMD ["mongo-express"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f330c3b5d7dfd93586e0a9cd86305dbb9f20fdd072303b2ab63b5b643476d55`  
		Last Modified: Thu, 18 Jun 2020 23:54:12 GMT  
		Size: 24.8 MB (24786700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895ca0c2289de2ec5eb556dd742d8f2a291a82514d322e900fb587c9d34bca1b`  
		Last Modified: Thu, 18 Jun 2020 23:54:04 GMT  
		Size: 2.3 MB (2302124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a71dcab8e9721c0f38e687383e95097029d807642ab752fd3c59e32f4a9d5bf`  
		Last Modified: Thu, 18 Jun 2020 23:54:03 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c9d9bfc2eafd675aee874dbd1d0797ae06659d36b56a3aab1e1a9c637dc8b5`  
		Last Modified: Fri, 19 Jun 2020 00:23:34 GMT  
		Size: 800.1 KB (800071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35c0195f6c3f8b71d2667ac21b3f6393216ee85d6c2a6329c2eef948ee3dcec`  
		Last Modified: Fri, 19 Jun 2020 00:23:39 GMT  
		Size: 16.7 MB (16652946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d84cc4268f95c9ea33d6336d422311a2a1265b982aa55f1eb1579f90dc773c`  
		Last Modified: Fri, 19 Jun 2020 00:23:34 GMT  
		Size: 655.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1994a327d80d0b81961a4b0190696cbc0467cd7f3d7c4bd9e63a39943c705cc9`  
		Last Modified: Fri, 19 Jun 2020 00:23:34 GMT  
		Size: 3.1 KB (3148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
