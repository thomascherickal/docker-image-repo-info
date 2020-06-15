<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rocket.chat`

-	[`rocket.chat:2`](#rocketchat2)
-	[`rocket.chat:2.4`](#rocketchat24)
-	[`rocket.chat:2.4.12`](#rocketchat2412)
-	[`rocket.chat:3`](#rocketchat3)
-	[`rocket.chat:3.3`](#rocketchat33)
-	[`rocket.chat:3.3.3`](#rocketchat333)
-	[`rocket.chat:latest`](#rocketchatlatest)

## `rocket.chat:2`

```console
$ docker pull rocket.chat@sha256:17b8adc0762413f76378235ee40fb13e5f60a1cdc2126d3f669b112f18a590a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:40f6b8d17b1ba33533bb16eea0abe80456882a78f821e3f113d21b38e4c2e204
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230037957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb6bbe5b702e27e09bd1236cdc94e1db3676d3b6c49fe1116bd90de4d56e5d1`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 09 Jun 2020 01:21:21 GMT
ADD file:688df9de0754445bcbcc9161f81427901f2e8fbbcd65faa60be3268305f83b57 in / 
# Tue, 09 Jun 2020 01:21:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 17:01:54 GMT
ENV NODE_ENV=production
# Tue, 09 Jun 2020 17:10:00 GMT
ENV NODE_VERSION=8.17.0
# Tue, 09 Jun 2020 17:12:43 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 17:12:45 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 09 Jun 2020 17:12:45 GMT
VOLUME [/app/uploads]
# Tue, 09 Jun 2020 17:12:47 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 09 Jun 2020 17:12:47 GMT
ENV RC_VERSION=2.4.12
# Tue, 09 Jun 2020 17:12:47 GMT
WORKDIR /app
# Tue, 09 Jun 2020 17:17:25 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 09 Jun 2020 17:17:27 GMT
USER rocketchat
# Tue, 09 Jun 2020 17:17:27 GMT
WORKDIR /app/bundle
# Tue, 09 Jun 2020 17:17:28 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 09 Jun 2020 17:17:28 GMT
EXPOSE 3000
# Tue, 09 Jun 2020 17:17:28 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:40091d2722f75524c5e9cffae33258a97a77a2f9f9f73e4161a68a998b206b79`  
		Last Modified: Tue, 09 Jun 2020 01:26:17 GMT  
		Size: 30.2 MB (30159671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39de4abbcc711e5d941f78c7c23fadc21a38aa752145db846c819c0845a90c1`  
		Last Modified: Tue, 09 Jun 2020 17:18:42 GMT  
		Size: 19.9 MB (19944690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a8e036fa7e5ab277d4f85a6ecc7cc28ae3a0124abef44c60ea4d048b21d206`  
		Last Modified: Tue, 09 Jun 2020 17:18:37 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6c4b0fb4fba5081c20ae5deb163f91890e12733bc577d39f178b7855f9527`  
		Last Modified: Tue, 09 Jun 2020 17:18:37 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c71a5fa2a0991ce021a3509e04d2cc73c4fe2bf1a2c0f62d46420d817ec1098`  
		Last Modified: Tue, 09 Jun 2020 17:19:44 GMT  
		Size: 179.8 MB (179760178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4`

```console
$ docker pull rocket.chat@sha256:17b8adc0762413f76378235ee40fb13e5f60a1cdc2126d3f669b112f18a590a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2.4` - linux; amd64

```console
$ docker pull rocket.chat@sha256:40f6b8d17b1ba33533bb16eea0abe80456882a78f821e3f113d21b38e4c2e204
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230037957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb6bbe5b702e27e09bd1236cdc94e1db3676d3b6c49fe1116bd90de4d56e5d1`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 09 Jun 2020 01:21:21 GMT
ADD file:688df9de0754445bcbcc9161f81427901f2e8fbbcd65faa60be3268305f83b57 in / 
# Tue, 09 Jun 2020 01:21:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 17:01:54 GMT
ENV NODE_ENV=production
# Tue, 09 Jun 2020 17:10:00 GMT
ENV NODE_VERSION=8.17.0
# Tue, 09 Jun 2020 17:12:43 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 17:12:45 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 09 Jun 2020 17:12:45 GMT
VOLUME [/app/uploads]
# Tue, 09 Jun 2020 17:12:47 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 09 Jun 2020 17:12:47 GMT
ENV RC_VERSION=2.4.12
# Tue, 09 Jun 2020 17:12:47 GMT
WORKDIR /app
# Tue, 09 Jun 2020 17:17:25 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 09 Jun 2020 17:17:27 GMT
USER rocketchat
# Tue, 09 Jun 2020 17:17:27 GMT
WORKDIR /app/bundle
# Tue, 09 Jun 2020 17:17:28 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 09 Jun 2020 17:17:28 GMT
EXPOSE 3000
# Tue, 09 Jun 2020 17:17:28 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:40091d2722f75524c5e9cffae33258a97a77a2f9f9f73e4161a68a998b206b79`  
		Last Modified: Tue, 09 Jun 2020 01:26:17 GMT  
		Size: 30.2 MB (30159671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39de4abbcc711e5d941f78c7c23fadc21a38aa752145db846c819c0845a90c1`  
		Last Modified: Tue, 09 Jun 2020 17:18:42 GMT  
		Size: 19.9 MB (19944690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a8e036fa7e5ab277d4f85a6ecc7cc28ae3a0124abef44c60ea4d048b21d206`  
		Last Modified: Tue, 09 Jun 2020 17:18:37 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6c4b0fb4fba5081c20ae5deb163f91890e12733bc577d39f178b7855f9527`  
		Last Modified: Tue, 09 Jun 2020 17:18:37 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c71a5fa2a0991ce021a3509e04d2cc73c4fe2bf1a2c0f62d46420d817ec1098`  
		Last Modified: Tue, 09 Jun 2020 17:19:44 GMT  
		Size: 179.8 MB (179760178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4.12`

```console
$ docker pull rocket.chat@sha256:17b8adc0762413f76378235ee40fb13e5f60a1cdc2126d3f669b112f18a590a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2.4.12` - linux; amd64

```console
$ docker pull rocket.chat@sha256:40f6b8d17b1ba33533bb16eea0abe80456882a78f821e3f113d21b38e4c2e204
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230037957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb6bbe5b702e27e09bd1236cdc94e1db3676d3b6c49fe1116bd90de4d56e5d1`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 09 Jun 2020 01:21:21 GMT
ADD file:688df9de0754445bcbcc9161f81427901f2e8fbbcd65faa60be3268305f83b57 in / 
# Tue, 09 Jun 2020 01:21:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 17:01:54 GMT
ENV NODE_ENV=production
# Tue, 09 Jun 2020 17:10:00 GMT
ENV NODE_VERSION=8.17.0
# Tue, 09 Jun 2020 17:12:43 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 17:12:45 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 09 Jun 2020 17:12:45 GMT
VOLUME [/app/uploads]
# Tue, 09 Jun 2020 17:12:47 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 09 Jun 2020 17:12:47 GMT
ENV RC_VERSION=2.4.12
# Tue, 09 Jun 2020 17:12:47 GMT
WORKDIR /app
# Tue, 09 Jun 2020 17:17:25 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 09 Jun 2020 17:17:27 GMT
USER rocketchat
# Tue, 09 Jun 2020 17:17:27 GMT
WORKDIR /app/bundle
# Tue, 09 Jun 2020 17:17:28 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 09 Jun 2020 17:17:28 GMT
EXPOSE 3000
# Tue, 09 Jun 2020 17:17:28 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:40091d2722f75524c5e9cffae33258a97a77a2f9f9f73e4161a68a998b206b79`  
		Last Modified: Tue, 09 Jun 2020 01:26:17 GMT  
		Size: 30.2 MB (30159671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39de4abbcc711e5d941f78c7c23fadc21a38aa752145db846c819c0845a90c1`  
		Last Modified: Tue, 09 Jun 2020 17:18:42 GMT  
		Size: 19.9 MB (19944690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a8e036fa7e5ab277d4f85a6ecc7cc28ae3a0124abef44c60ea4d048b21d206`  
		Last Modified: Tue, 09 Jun 2020 17:18:37 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6c4b0fb4fba5081c20ae5deb163f91890e12733bc577d39f178b7855f9527`  
		Last Modified: Tue, 09 Jun 2020 17:18:37 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c71a5fa2a0991ce021a3509e04d2cc73c4fe2bf1a2c0f62d46420d817ec1098`  
		Last Modified: Tue, 09 Jun 2020 17:19:44 GMT  
		Size: 179.8 MB (179760178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3`

```console
$ docker pull rocket.chat@sha256:ef58468bd4ad06c5a144896af2186ae5c0c353109c8fbce1177b3bb2a32d91ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3` - linux; amd64

```console
$ docker pull rocket.chat@sha256:2e8dd755ca428daefc891926402da2b9956dfa2ea74d5c44318d6b000d6a4194
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236078164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2294137dffddf827a5be8337f050ad99d33e6004a8cba19dd544f7a69e2acdbd`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 09 Jun 2020 01:21:21 GMT
ADD file:688df9de0754445bcbcc9161f81427901f2e8fbbcd65faa60be3268305f83b57 in / 
# Tue, 09 Jun 2020 01:21:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 17:01:54 GMT
ENV NODE_ENV=production
# Tue, 09 Jun 2020 17:01:54 GMT
ENV NODE_VERSION=12.16.1
# Tue, 09 Jun 2020 17:04:26 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 17:04:27 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 09 Jun 2020 17:04:28 GMT
VOLUME [/app/uploads]
# Tue, 09 Jun 2020 17:04:28 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 09 Jun 2020 17:04:29 GMT
ENV RC_VERSION=3.3.0
# Tue, 09 Jun 2020 17:04:29 GMT
WORKDIR /app
# Tue, 09 Jun 2020 17:09:41 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 09 Jun 2020 17:09:45 GMT
USER rocketchat
# Tue, 09 Jun 2020 17:09:45 GMT
WORKDIR /app/bundle
# Tue, 09 Jun 2020 17:09:45 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 09 Jun 2020 17:09:46 GMT
EXPOSE 3000
# Tue, 09 Jun 2020 17:09:46 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:40091d2722f75524c5e9cffae33258a97a77a2f9f9f73e4161a68a998b206b79`  
		Last Modified: Tue, 09 Jun 2020 01:26:17 GMT  
		Size: 30.2 MB (30159671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d5d5e05d38ec403393d42e03204749f9adf4c1ed9d2448fa15ab26b2a2ae11`  
		Last Modified: Tue, 09 Jun 2020 17:17:48 GMT  
		Size: 24.2 MB (24202148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60c1732caadbf8b1eeecc2b93d5b5e8aadefec33990dafb98b5224c0ae77a51`  
		Last Modified: Tue, 09 Jun 2020 17:17:41 GMT  
		Size: 2.1 KB (2133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b937b8ec9a4b18605891efdc4c75cd888ddd5a69cac5ef596ae5d6a12651a99`  
		Last Modified: Tue, 09 Jun 2020 17:17:41 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaa951192f53e7b6148ad28671cfbd91723b94f94928b54166afdcc7a7ce00f`  
		Last Modified: Tue, 09 Jun 2020 17:18:31 GMT  
		Size: 181.5 MB (181542930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.3`

```console
$ docker pull rocket.chat@sha256:ef58468bd4ad06c5a144896af2186ae5c0c353109c8fbce1177b3bb2a32d91ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.3` - linux; amd64

```console
$ docker pull rocket.chat@sha256:2e8dd755ca428daefc891926402da2b9956dfa2ea74d5c44318d6b000d6a4194
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236078164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2294137dffddf827a5be8337f050ad99d33e6004a8cba19dd544f7a69e2acdbd`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 09 Jun 2020 01:21:21 GMT
ADD file:688df9de0754445bcbcc9161f81427901f2e8fbbcd65faa60be3268305f83b57 in / 
# Tue, 09 Jun 2020 01:21:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 17:01:54 GMT
ENV NODE_ENV=production
# Tue, 09 Jun 2020 17:01:54 GMT
ENV NODE_VERSION=12.16.1
# Tue, 09 Jun 2020 17:04:26 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 17:04:27 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 09 Jun 2020 17:04:28 GMT
VOLUME [/app/uploads]
# Tue, 09 Jun 2020 17:04:28 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 09 Jun 2020 17:04:29 GMT
ENV RC_VERSION=3.3.0
# Tue, 09 Jun 2020 17:04:29 GMT
WORKDIR /app
# Tue, 09 Jun 2020 17:09:41 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 09 Jun 2020 17:09:45 GMT
USER rocketchat
# Tue, 09 Jun 2020 17:09:45 GMT
WORKDIR /app/bundle
# Tue, 09 Jun 2020 17:09:45 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 09 Jun 2020 17:09:46 GMT
EXPOSE 3000
# Tue, 09 Jun 2020 17:09:46 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:40091d2722f75524c5e9cffae33258a97a77a2f9f9f73e4161a68a998b206b79`  
		Last Modified: Tue, 09 Jun 2020 01:26:17 GMT  
		Size: 30.2 MB (30159671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d5d5e05d38ec403393d42e03204749f9adf4c1ed9d2448fa15ab26b2a2ae11`  
		Last Modified: Tue, 09 Jun 2020 17:17:48 GMT  
		Size: 24.2 MB (24202148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60c1732caadbf8b1eeecc2b93d5b5e8aadefec33990dafb98b5224c0ae77a51`  
		Last Modified: Tue, 09 Jun 2020 17:17:41 GMT  
		Size: 2.1 KB (2133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b937b8ec9a4b18605891efdc4c75cd888ddd5a69cac5ef596ae5d6a12651a99`  
		Last Modified: Tue, 09 Jun 2020 17:17:41 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaa951192f53e7b6148ad28671cfbd91723b94f94928b54166afdcc7a7ce00f`  
		Last Modified: Tue, 09 Jun 2020 17:18:31 GMT  
		Size: 181.5 MB (181542930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.3.3`

**does not exist** (yet?)

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:ef58468bd4ad06c5a144896af2186ae5c0c353109c8fbce1177b3bb2a32d91ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:2e8dd755ca428daefc891926402da2b9956dfa2ea74d5c44318d6b000d6a4194
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236078164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2294137dffddf827a5be8337f050ad99d33e6004a8cba19dd544f7a69e2acdbd`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 09 Jun 2020 01:21:21 GMT
ADD file:688df9de0754445bcbcc9161f81427901f2e8fbbcd65faa60be3268305f83b57 in / 
# Tue, 09 Jun 2020 01:21:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 17:01:54 GMT
ENV NODE_ENV=production
# Tue, 09 Jun 2020 17:01:54 GMT
ENV NODE_VERSION=12.16.1
# Tue, 09 Jun 2020 17:04:26 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Jun 2020 17:04:27 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 09 Jun 2020 17:04:28 GMT
VOLUME [/app/uploads]
# Tue, 09 Jun 2020 17:04:28 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 09 Jun 2020 17:04:29 GMT
ENV RC_VERSION=3.3.0
# Tue, 09 Jun 2020 17:04:29 GMT
WORKDIR /app
# Tue, 09 Jun 2020 17:09:41 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 09 Jun 2020 17:09:45 GMT
USER rocketchat
# Tue, 09 Jun 2020 17:09:45 GMT
WORKDIR /app/bundle
# Tue, 09 Jun 2020 17:09:45 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 09 Jun 2020 17:09:46 GMT
EXPOSE 3000
# Tue, 09 Jun 2020 17:09:46 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:40091d2722f75524c5e9cffae33258a97a77a2f9f9f73e4161a68a998b206b79`  
		Last Modified: Tue, 09 Jun 2020 01:26:17 GMT  
		Size: 30.2 MB (30159671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d5d5e05d38ec403393d42e03204749f9adf4c1ed9d2448fa15ab26b2a2ae11`  
		Last Modified: Tue, 09 Jun 2020 17:17:48 GMT  
		Size: 24.2 MB (24202148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60c1732caadbf8b1eeecc2b93d5b5e8aadefec33990dafb98b5224c0ae77a51`  
		Last Modified: Tue, 09 Jun 2020 17:17:41 GMT  
		Size: 2.1 KB (2133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b937b8ec9a4b18605891efdc4c75cd888ddd5a69cac5ef596ae5d6a12651a99`  
		Last Modified: Tue, 09 Jun 2020 17:17:41 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaa951192f53e7b6148ad28671cfbd91723b94f94928b54166afdcc7a7ce00f`  
		Last Modified: Tue, 09 Jun 2020 17:18:31 GMT  
		Size: 181.5 MB (181542930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
