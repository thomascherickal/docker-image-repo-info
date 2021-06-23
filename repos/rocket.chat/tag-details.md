<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rocket.chat`

-	[`rocket.chat:2`](#rocketchat2)
-	[`rocket.chat:2.4`](#rocketchat24)
-	[`rocket.chat:2.4.14`](#rocketchat2414)
-	[`rocket.chat:3`](#rocketchat3)
-	[`rocket.chat:3.13`](#rocketchat313)
-	[`rocket.chat:3.13.5`](#rocketchat3135)
-	[`rocket.chat:3.14`](#rocketchat314)
-	[`rocket.chat:3.14.5`](#rocketchat3145)
-	[`rocket.chat:3.15`](#rocketchat315)
-	[`rocket.chat:3.15.1`](#rocketchat3151)
-	[`rocket.chat:latest`](#rocketchatlatest)

## `rocket.chat:2`

```console
$ docker pull rocket.chat@sha256:93471dccd56ef4f684a600c9dcd0c345250c786766855f20b0d8b620f605eb36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:4ff8a0975d960c1b896486f8f030f499dcc83d200ddfc9c66821fe66ac2e19d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.8 MB (216849504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47aacbd0c5bdc5cc774b6744143baa4fe96f19367e189982cc9e87104972b457`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:48:37 GMT
ENV NODE_VERSION=8.17.0
# Wed, 23 Jun 2021 16:48:56 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:48:57 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:48:57 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:48:57 GMT
ENV RC_VERSION=2.4.14
# Wed, 23 Jun 2021 16:48:58 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:49:39 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:49:43 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:49:43 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:49:43 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:49:44 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:49:44 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a4eefb90596023f092204285a13fe91c76e69cd481808b3ad7e3976b846125`  
		Last Modified: Wed, 23 Jun 2021 16:52:37 GMT  
		Size: 19.8 MB (19783337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55a62491c03ffd3e6505f4e3e42a5332d0bc46d580bb5c9aa70a70b2053a6c`  
		Last Modified: Wed, 23 Jun 2021 16:52:32 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7449c51b1e79a528d56b7923603f7152a5750e26ee79ce1e3826a38c631f53`  
		Last Modified: Wed, 23 Jun 2021 16:53:05 GMT  
		Size: 169.9 MB (169918511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4`

```console
$ docker pull rocket.chat@sha256:93471dccd56ef4f684a600c9dcd0c345250c786766855f20b0d8b620f605eb36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2.4` - linux; amd64

```console
$ docker pull rocket.chat@sha256:4ff8a0975d960c1b896486f8f030f499dcc83d200ddfc9c66821fe66ac2e19d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.8 MB (216849504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47aacbd0c5bdc5cc774b6744143baa4fe96f19367e189982cc9e87104972b457`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:48:37 GMT
ENV NODE_VERSION=8.17.0
# Wed, 23 Jun 2021 16:48:56 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:48:57 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:48:57 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:48:57 GMT
ENV RC_VERSION=2.4.14
# Wed, 23 Jun 2021 16:48:58 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:49:39 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:49:43 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:49:43 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:49:43 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:49:44 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:49:44 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a4eefb90596023f092204285a13fe91c76e69cd481808b3ad7e3976b846125`  
		Last Modified: Wed, 23 Jun 2021 16:52:37 GMT  
		Size: 19.8 MB (19783337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55a62491c03ffd3e6505f4e3e42a5332d0bc46d580bb5c9aa70a70b2053a6c`  
		Last Modified: Wed, 23 Jun 2021 16:52:32 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7449c51b1e79a528d56b7923603f7152a5750e26ee79ce1e3826a38c631f53`  
		Last Modified: Wed, 23 Jun 2021 16:53:05 GMT  
		Size: 169.9 MB (169918511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4.14`

```console
$ docker pull rocket.chat@sha256:93471dccd56ef4f684a600c9dcd0c345250c786766855f20b0d8b620f605eb36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2.4.14` - linux; amd64

```console
$ docker pull rocket.chat@sha256:4ff8a0975d960c1b896486f8f030f499dcc83d200ddfc9c66821fe66ac2e19d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.8 MB (216849504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47aacbd0c5bdc5cc774b6744143baa4fe96f19367e189982cc9e87104972b457`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:48:37 GMT
ENV NODE_VERSION=8.17.0
# Wed, 23 Jun 2021 16:48:56 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:48:57 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:48:57 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:48:57 GMT
ENV RC_VERSION=2.4.14
# Wed, 23 Jun 2021 16:48:58 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:49:39 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:49:43 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:49:43 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:49:43 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:49:44 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:49:44 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a4eefb90596023f092204285a13fe91c76e69cd481808b3ad7e3976b846125`  
		Last Modified: Wed, 23 Jun 2021 16:52:37 GMT  
		Size: 19.8 MB (19783337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad55a62491c03ffd3e6505f4e3e42a5332d0bc46d580bb5c9aa70a70b2053a6c`  
		Last Modified: Wed, 23 Jun 2021 16:52:32 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7449c51b1e79a528d56b7923603f7152a5750e26ee79ce1e3826a38c631f53`  
		Last Modified: Wed, 23 Jun 2021 16:53:05 GMT  
		Size: 169.9 MB (169918511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3`

```console
$ docker pull rocket.chat@sha256:643a513f5a99220532d74a31ffd098c976e932d593da61aaf4da8d772540465a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3` - linux; amd64

```console
$ docker pull rocket.chat@sha256:146dfda87fff22201ea4f12e006397dd3f9b9fabce0e82432a5d9d765c04afa1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224291829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12fd783ba8f716f1c2c291fe071e6333db66907f4797dc4a01995722ad5182d`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_VERSION=12.22.1
# Wed, 23 Jun 2021 16:44:24 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:44:25 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:44:26 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:44:26 GMT
ENV RC_VERSION=3.15.1
# Wed, 23 Jun 2021 16:44:26 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:45:29 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:45:32 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:45:32 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:45:33 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:45:33 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:45:33 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b773c639f211d56ee249fe68fbd89ea3206a56271db4b6628990f59b1e58512`  
		Last Modified: Wed, 23 Jun 2021 16:50:09 GMT  
		Size: 24.1 MB (24134407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0da238735c4f3bec824501ef96b0663761d657b428205c9decd4d6c53af216f`  
		Last Modified: Wed, 23 Jun 2021 16:50:04 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05243c3e0b84c22ae9adf57b36a10e616e37b8fa03bf21b6bf8d61420f89ae1b`  
		Last Modified: Wed, 23 Jun 2021 16:50:40 GMT  
		Size: 173.0 MB (173009762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.13`

```console
$ docker pull rocket.chat@sha256:e697665bc0ef1890466b630de53109d7b99cc99791290596cdc59223fa4b228c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.13` - linux; amd64

```console
$ docker pull rocket.chat@sha256:e80399859c5c8b1d606b9bf14022874fd39533b5e6ec7c292d459cc262b51f96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.1 MB (219070174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e888a19f577d33a9188890296c6da1c42276d801db07d1a0b4cfff6ba85c1a80`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:47:11 GMT
ENV NODE_VERSION=12.21.0
# Wed, 23 Jun 2021 16:47:31 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:47:32 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:47:32 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:47:32 GMT
ENV RC_VERSION=3.13.5
# Wed, 23 Jun 2021 16:47:33 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:48:28 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:48:32 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:48:33 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:48:33 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:48:33 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:48:33 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6260f01412f19797c3b89eb95dfa0de73c566f969a675753129c5b063f239b7`  
		Last Modified: Wed, 23 Jun 2021 16:51:52 GMT  
		Size: 24.1 MB (24123347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba77aa15c4f31d5fa94d37a8b0ee6071c8f32aee30b3134a4ff2bb76cf77e8a`  
		Last Modified: Wed, 23 Jun 2021 16:51:46 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3093cd4b6ca6aa0aec44087403015f4a065ec4a99b0fad56ae29322638230f`  
		Last Modified: Wed, 23 Jun 2021 16:52:22 GMT  
		Size: 167.8 MB (167799168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.13.5`

```console
$ docker pull rocket.chat@sha256:e697665bc0ef1890466b630de53109d7b99cc99791290596cdc59223fa4b228c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.13.5` - linux; amd64

```console
$ docker pull rocket.chat@sha256:e80399859c5c8b1d606b9bf14022874fd39533b5e6ec7c292d459cc262b51f96
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.1 MB (219070174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e888a19f577d33a9188890296c6da1c42276d801db07d1a0b4cfff6ba85c1a80`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:47:11 GMT
ENV NODE_VERSION=12.21.0
# Wed, 23 Jun 2021 16:47:31 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:47:32 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:47:32 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:47:32 GMT
ENV RC_VERSION=3.13.5
# Wed, 23 Jun 2021 16:47:33 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:48:28 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:48:32 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:48:33 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:48:33 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:48:33 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:48:33 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6260f01412f19797c3b89eb95dfa0de73c566f969a675753129c5b063f239b7`  
		Last Modified: Wed, 23 Jun 2021 16:51:52 GMT  
		Size: 24.1 MB (24123347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba77aa15c4f31d5fa94d37a8b0ee6071c8f32aee30b3134a4ff2bb76cf77e8a`  
		Last Modified: Wed, 23 Jun 2021 16:51:46 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3093cd4b6ca6aa0aec44087403015f4a065ec4a99b0fad56ae29322638230f`  
		Last Modified: Wed, 23 Jun 2021 16:52:22 GMT  
		Size: 167.8 MB (167799168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.14`

```console
$ docker pull rocket.chat@sha256:558bb9a4e5616726b3ec55934959ebd5253dca1bb9d8ae9d1593b843bda6c1e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.14` - linux; amd64

```console
$ docker pull rocket.chat@sha256:3675f3d28ee6f90341643db3a55d8ffcd3dc772f07f5edd7c669eedfcbd260ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223674338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd3b0affd143bd8589cfaa07eb047b5bf1aef210beabb527b72dd970cff2220`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_VERSION=12.22.1
# Wed, 23 Jun 2021 16:44:24 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:44:25 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:44:26 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:45:46 GMT
ENV RC_VERSION=3.14.5
# Wed, 23 Jun 2021 16:45:46 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:47:02 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:47:05 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:47:05 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:47:05 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:47:06 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:47:06 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b773c639f211d56ee249fe68fbd89ea3206a56271db4b6628990f59b1e58512`  
		Last Modified: Wed, 23 Jun 2021 16:50:09 GMT  
		Size: 24.1 MB (24134407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0da238735c4f3bec824501ef96b0663761d657b428205c9decd4d6c53af216f`  
		Last Modified: Wed, 23 Jun 2021 16:50:04 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6f674f4c0900132e595915fe6b2b674f87c42ce39a4ed371b2ed7110afe1e9`  
		Last Modified: Wed, 23 Jun 2021 16:51:35 GMT  
		Size: 172.4 MB (172392271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.14.5`

```console
$ docker pull rocket.chat@sha256:558bb9a4e5616726b3ec55934959ebd5253dca1bb9d8ae9d1593b843bda6c1e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.14.5` - linux; amd64

```console
$ docker pull rocket.chat@sha256:3675f3d28ee6f90341643db3a55d8ffcd3dc772f07f5edd7c669eedfcbd260ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223674338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cd3b0affd143bd8589cfaa07eb047b5bf1aef210beabb527b72dd970cff2220`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_VERSION=12.22.1
# Wed, 23 Jun 2021 16:44:24 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:44:25 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:44:26 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:45:46 GMT
ENV RC_VERSION=3.14.5
# Wed, 23 Jun 2021 16:45:46 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:47:02 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:47:05 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:47:05 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:47:05 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:47:06 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:47:06 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b773c639f211d56ee249fe68fbd89ea3206a56271db4b6628990f59b1e58512`  
		Last Modified: Wed, 23 Jun 2021 16:50:09 GMT  
		Size: 24.1 MB (24134407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0da238735c4f3bec824501ef96b0663761d657b428205c9decd4d6c53af216f`  
		Last Modified: Wed, 23 Jun 2021 16:50:04 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6f674f4c0900132e595915fe6b2b674f87c42ce39a4ed371b2ed7110afe1e9`  
		Last Modified: Wed, 23 Jun 2021 16:51:35 GMT  
		Size: 172.4 MB (172392271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.15`

```console
$ docker pull rocket.chat@sha256:643a513f5a99220532d74a31ffd098c976e932d593da61aaf4da8d772540465a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.15` - linux; amd64

```console
$ docker pull rocket.chat@sha256:146dfda87fff22201ea4f12e006397dd3f9b9fabce0e82432a5d9d765c04afa1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224291829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12fd783ba8f716f1c2c291fe071e6333db66907f4797dc4a01995722ad5182d`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_VERSION=12.22.1
# Wed, 23 Jun 2021 16:44:24 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:44:25 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:44:26 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:44:26 GMT
ENV RC_VERSION=3.15.1
# Wed, 23 Jun 2021 16:44:26 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:45:29 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:45:32 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:45:32 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:45:33 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:45:33 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:45:33 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b773c639f211d56ee249fe68fbd89ea3206a56271db4b6628990f59b1e58512`  
		Last Modified: Wed, 23 Jun 2021 16:50:09 GMT  
		Size: 24.1 MB (24134407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0da238735c4f3bec824501ef96b0663761d657b428205c9decd4d6c53af216f`  
		Last Modified: Wed, 23 Jun 2021 16:50:04 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05243c3e0b84c22ae9adf57b36a10e616e37b8fa03bf21b6bf8d61420f89ae1b`  
		Last Modified: Wed, 23 Jun 2021 16:50:40 GMT  
		Size: 173.0 MB (173009762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.15.1`

```console
$ docker pull rocket.chat@sha256:643a513f5a99220532d74a31ffd098c976e932d593da61aaf4da8d772540465a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.15.1` - linux; amd64

```console
$ docker pull rocket.chat@sha256:146dfda87fff22201ea4f12e006397dd3f9b9fabce0e82432a5d9d765c04afa1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224291829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12fd783ba8f716f1c2c291fe071e6333db66907f4797dc4a01995722ad5182d`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_VERSION=12.22.1
# Wed, 23 Jun 2021 16:44:24 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:44:25 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:44:26 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:44:26 GMT
ENV RC_VERSION=3.15.1
# Wed, 23 Jun 2021 16:44:26 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:45:29 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:45:32 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:45:32 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:45:33 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:45:33 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:45:33 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b773c639f211d56ee249fe68fbd89ea3206a56271db4b6628990f59b1e58512`  
		Last Modified: Wed, 23 Jun 2021 16:50:09 GMT  
		Size: 24.1 MB (24134407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0da238735c4f3bec824501ef96b0663761d657b428205c9decd4d6c53af216f`  
		Last Modified: Wed, 23 Jun 2021 16:50:04 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05243c3e0b84c22ae9adf57b36a10e616e37b8fa03bf21b6bf8d61420f89ae1b`  
		Last Modified: Wed, 23 Jun 2021 16:50:40 GMT  
		Size: 173.0 MB (173009762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:643a513f5a99220532d74a31ffd098c976e932d593da61aaf4da8d772540465a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:146dfda87fff22201ea4f12e006397dd3f9b9fabce0e82432a5d9d765c04afa1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.3 MB (224291829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12fd783ba8f716f1c2c291fe071e6333db66907f4797dc4a01995722ad5182d`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_ENV=production
# Wed, 23 Jun 2021 16:44:04 GMT
ENV NODE_VERSION=12.22.1
# Wed, 23 Jun 2021 16:44:24 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 23 Jun 2021 16:44:25 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Wed, 23 Jun 2021 16:44:26 GMT
VOLUME [/app/uploads]
# Wed, 23 Jun 2021 16:44:26 GMT
ENV RC_VERSION=3.15.1
# Wed, 23 Jun 2021 16:44:26 GMT
WORKDIR /app
# Wed, 23 Jun 2021 16:45:29 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 23 Jun 2021 16:45:32 GMT
USER rocketchat
# Wed, 23 Jun 2021 16:45:32 GMT
WORKDIR /app/bundle
# Wed, 23 Jun 2021 16:45:33 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 23 Jun 2021 16:45:33 GMT
EXPOSE 3000
# Wed, 23 Jun 2021 16:45:33 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b773c639f211d56ee249fe68fbd89ea3206a56271db4b6628990f59b1e58512`  
		Last Modified: Wed, 23 Jun 2021 16:50:09 GMT  
		Size: 24.1 MB (24134407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0da238735c4f3bec824501ef96b0663761d657b428205c9decd4d6c53af216f`  
		Last Modified: Wed, 23 Jun 2021 16:50:04 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05243c3e0b84c22ae9adf57b36a10e616e37b8fa03bf21b6bf8d61420f89ae1b`  
		Last Modified: Wed, 23 Jun 2021 16:50:40 GMT  
		Size: 173.0 MB (173009762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
