<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rocket.chat`

-	[`rocket.chat:2`](#rocketchat2)
-	[`rocket.chat:2.4`](#rocketchat24)
-	[`rocket.chat:2.4.12`](#rocketchat2412)
-	[`rocket.chat:3`](#rocketchat3)
-	[`rocket.chat:3.2`](#rocketchat32)
-	[`rocket.chat:3.2.2`](#rocketchat322)
-	[`rocket.chat:latest`](#rocketchatlatest)

## `rocket.chat:2`

```console
$ docker pull rocket.chat@sha256:f5bb898a6521efedade1b458a78db6b2027d345b3ea19f07f98c67aa9cd58b57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:fb879422fbdc54c228491c49bee2a945cb8c9ef206f726d712b1708fe03e3db1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.1 MB (230052760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b129b9acca305572493d2e65f09ee6066564281835f06dd6adda8b5f1afff58`
-	Default Command: `["node","main.js"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:56 GMT
ADD file:12f431dee31c4b68fb9086f9cb161ce7ee7d5a9240c585fb97753d6c1947dca1 in / 
# Thu, 23 Apr 2020 00:20:56 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:19:30 GMT
ENV NODE_ENV=production
# Thu, 23 Apr 2020 01:27:37 GMT
ENV NODE_VERSION=8.17.0
# Thu, 23 Apr 2020 01:30:14 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 01:30:16 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Thu, 23 Apr 2020 01:30:17 GMT
VOLUME [/app/uploads]
# Thu, 23 Apr 2020 01:30:18 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Thu, 23 Apr 2020 01:30:18 GMT
ENV RC_VERSION=2.4.11
# Thu, 23 Apr 2020 01:30:18 GMT
WORKDIR /app
# Thu, 23 Apr 2020 01:34:34 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Thu, 23 Apr 2020 01:34:36 GMT
USER rocketchat
# Thu, 23 Apr 2020 01:34:36 GMT
WORKDIR /app/bundle
# Thu, 23 Apr 2020 01:34:36 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Thu, 23 Apr 2020 01:34:36 GMT
EXPOSE 3000
# Thu, 23 Apr 2020 01:34:36 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:370e9f631e97a4ed400761a93ab4822527644e7a600f3121f98707f8c2e32f2e`  
		Last Modified: Thu, 23 Apr 2020 00:25:33 GMT  
		Size: 30.2 MB (30159480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87660d2b0d45cbbdc004bc1cc00b9c039142b5f7088959e84a073ccb9a68c2b6`  
		Last Modified: Thu, 23 Apr 2020 01:35:55 GMT  
		Size: 19.9 MB (19944651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29456d8ae75f79dfb37daef0acf01a5359b3b60f69a039269a550ed118a3c24`  
		Last Modified: Thu, 23 Apr 2020 01:35:51 GMT  
		Size: 2.1 KB (2134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2bf2b19e6f4c5e024123b66c49dc5a8fb707ff3b3142f159ab1a89598203c1`  
		Last Modified: Thu, 23 Apr 2020 01:35:50 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a070b6dfe9874e6dc44a514d3823f2c53ed8eb8dbf9a2f0e1962af6b44eb664`  
		Last Modified: Thu, 23 Apr 2020 01:36:30 GMT  
		Size: 179.8 MB (179775213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4`

```console
$ docker pull rocket.chat@sha256:f5bb898a6521efedade1b458a78db6b2027d345b3ea19f07f98c67aa9cd58b57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2.4` - linux; amd64

```console
$ docker pull rocket.chat@sha256:fb879422fbdc54c228491c49bee2a945cb8c9ef206f726d712b1708fe03e3db1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.1 MB (230052760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b129b9acca305572493d2e65f09ee6066564281835f06dd6adda8b5f1afff58`
-	Default Command: `["node","main.js"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:56 GMT
ADD file:12f431dee31c4b68fb9086f9cb161ce7ee7d5a9240c585fb97753d6c1947dca1 in / 
# Thu, 23 Apr 2020 00:20:56 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:19:30 GMT
ENV NODE_ENV=production
# Thu, 23 Apr 2020 01:27:37 GMT
ENV NODE_VERSION=8.17.0
# Thu, 23 Apr 2020 01:30:14 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 01:30:16 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Thu, 23 Apr 2020 01:30:17 GMT
VOLUME [/app/uploads]
# Thu, 23 Apr 2020 01:30:18 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Thu, 23 Apr 2020 01:30:18 GMT
ENV RC_VERSION=2.4.11
# Thu, 23 Apr 2020 01:30:18 GMT
WORKDIR /app
# Thu, 23 Apr 2020 01:34:34 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Thu, 23 Apr 2020 01:34:36 GMT
USER rocketchat
# Thu, 23 Apr 2020 01:34:36 GMT
WORKDIR /app/bundle
# Thu, 23 Apr 2020 01:34:36 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Thu, 23 Apr 2020 01:34:36 GMT
EXPOSE 3000
# Thu, 23 Apr 2020 01:34:36 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:370e9f631e97a4ed400761a93ab4822527644e7a600f3121f98707f8c2e32f2e`  
		Last Modified: Thu, 23 Apr 2020 00:25:33 GMT  
		Size: 30.2 MB (30159480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87660d2b0d45cbbdc004bc1cc00b9c039142b5f7088959e84a073ccb9a68c2b6`  
		Last Modified: Thu, 23 Apr 2020 01:35:55 GMT  
		Size: 19.9 MB (19944651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29456d8ae75f79dfb37daef0acf01a5359b3b60f69a039269a550ed118a3c24`  
		Last Modified: Thu, 23 Apr 2020 01:35:51 GMT  
		Size: 2.1 KB (2134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2bf2b19e6f4c5e024123b66c49dc5a8fb707ff3b3142f159ab1a89598203c1`  
		Last Modified: Thu, 23 Apr 2020 01:35:50 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a070b6dfe9874e6dc44a514d3823f2c53ed8eb8dbf9a2f0e1962af6b44eb664`  
		Last Modified: Thu, 23 Apr 2020 01:36:30 GMT  
		Size: 179.8 MB (179775213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4.12`

**does not exist** (yet?)

## `rocket.chat:3`

```console
$ docker pull rocket.chat@sha256:ae4abef698f5ae2ca0e32361fc4d88ea9120a7a58210eb0e2db75b3875570231
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3` - linux; amd64

```console
$ docker pull rocket.chat@sha256:6d9a0ede1e2648f0f9f2db52bfe7a3f5888ea2db3d5f94fc48560b1979917d97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226182938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bae5bbdc5e55ac03c5fcf4883b5f1483cf8c3dd748593d3936dce2eada1257f`
-	Default Command: `["node","main.js"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:56 GMT
ADD file:12f431dee31c4b68fb9086f9cb161ce7ee7d5a9240c585fb97753d6c1947dca1 in / 
# Thu, 23 Apr 2020 00:20:56 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:19:30 GMT
ENV NODE_ENV=production
# Thu, 23 Apr 2020 01:19:30 GMT
ENV NODE_VERSION=12.14.0
# Thu, 23 Apr 2020 01:22:09 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 01:22:10 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Thu, 23 Apr 2020 01:22:11 GMT
VOLUME [/app/uploads]
# Thu, 23 Apr 2020 01:22:11 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Thu, 23 Apr 2020 01:22:12 GMT
ENV RC_VERSION=3.0.12
# Thu, 23 Apr 2020 01:22:12 GMT
WORKDIR /app
# Thu, 23 Apr 2020 01:27:23 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Thu, 23 Apr 2020 01:27:25 GMT
USER rocketchat
# Thu, 23 Apr 2020 01:27:26 GMT
WORKDIR /app/bundle
# Thu, 23 Apr 2020 01:27:26 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Thu, 23 Apr 2020 01:27:27 GMT
EXPOSE 3000
# Thu, 23 Apr 2020 01:27:27 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:370e9f631e97a4ed400761a93ab4822527644e7a600f3121f98707f8c2e32f2e`  
		Last Modified: Thu, 23 Apr 2020 00:25:33 GMT  
		Size: 30.2 MB (30159480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d516b9cc7f9919845abe24aa09c466e1dba77d2cb76a9669e201c591b3a87950`  
		Last Modified: Thu, 23 Apr 2020 01:34:53 GMT  
		Size: 24.0 MB (23991717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71e91ed1aa6abdf19dd1f8357aff2b53bf70754dad1df2e279d37436ecb21e8`  
		Last Modified: Thu, 23 Apr 2020 01:34:47 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b82675c8ec5712904a152817f89b2d6d83ed95ec9b47a00ffd0cd02b11f69c`  
		Last Modified: Thu, 23 Apr 2020 01:34:46 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1430023942b31358eb471c3eac296140b41d457da7236744a1bb69b7fb882552`  
		Last Modified: Thu, 23 Apr 2020 01:35:27 GMT  
		Size: 171.9 MB (171858320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.2`

**does not exist** (yet?)

## `rocket.chat:3.2.2`

**does not exist** (yet?)

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:ae4abef698f5ae2ca0e32361fc4d88ea9120a7a58210eb0e2db75b3875570231
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:6d9a0ede1e2648f0f9f2db52bfe7a3f5888ea2db3d5f94fc48560b1979917d97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226182938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bae5bbdc5e55ac03c5fcf4883b5f1483cf8c3dd748593d3936dce2eada1257f`
-	Default Command: `["node","main.js"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:56 GMT
ADD file:12f431dee31c4b68fb9086f9cb161ce7ee7d5a9240c585fb97753d6c1947dca1 in / 
# Thu, 23 Apr 2020 00:20:56 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 01:19:30 GMT
ENV NODE_ENV=production
# Thu, 23 Apr 2020 01:19:30 GMT
ENV NODE_VERSION=12.14.0
# Thu, 23 Apr 2020 01:22:09 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 01:22:10 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Thu, 23 Apr 2020 01:22:11 GMT
VOLUME [/app/uploads]
# Thu, 23 Apr 2020 01:22:11 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Thu, 23 Apr 2020 01:22:12 GMT
ENV RC_VERSION=3.0.12
# Thu, 23 Apr 2020 01:22:12 GMT
WORKDIR /app
# Thu, 23 Apr 2020 01:27:23 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Thu, 23 Apr 2020 01:27:25 GMT
USER rocketchat
# Thu, 23 Apr 2020 01:27:26 GMT
WORKDIR /app/bundle
# Thu, 23 Apr 2020 01:27:26 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Thu, 23 Apr 2020 01:27:27 GMT
EXPOSE 3000
# Thu, 23 Apr 2020 01:27:27 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:370e9f631e97a4ed400761a93ab4822527644e7a600f3121f98707f8c2e32f2e`  
		Last Modified: Thu, 23 Apr 2020 00:25:33 GMT  
		Size: 30.2 MB (30159480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d516b9cc7f9919845abe24aa09c466e1dba77d2cb76a9669e201c591b3a87950`  
		Last Modified: Thu, 23 Apr 2020 01:34:53 GMT  
		Size: 24.0 MB (23991717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71e91ed1aa6abdf19dd1f8357aff2b53bf70754dad1df2e279d37436ecb21e8`  
		Last Modified: Thu, 23 Apr 2020 01:34:47 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b82675c8ec5712904a152817f89b2d6d83ed95ec9b47a00ffd0cd02b11f69c`  
		Last Modified: Thu, 23 Apr 2020 01:34:46 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1430023942b31358eb471c3eac296140b41d457da7236744a1bb69b7fb882552`  
		Last Modified: Thu, 23 Apr 2020 01:35:27 GMT  
		Size: 171.9 MB (171858320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
