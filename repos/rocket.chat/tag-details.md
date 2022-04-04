<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rocket.chat`

-	[`rocket.chat:3`](#rocketchat3)
-	[`rocket.chat:3.18`](#rocketchat318)
-	[`rocket.chat:3.18.5`](#rocketchat3185)
-	[`rocket.chat:4`](#rocketchat4)
-	[`rocket.chat:4.4`](#rocketchat44)
-	[`rocket.chat:4.4.2`](#rocketchat442)
-	[`rocket.chat:4.5`](#rocketchat45)
-	[`rocket.chat:4.5.5`](#rocketchat455)
-	[`rocket.chat:4.6`](#rocketchat46)
-	[`rocket.chat:4.6.0`](#rocketchat460)
-	[`rocket.chat:latest`](#rocketchatlatest)

## `rocket.chat:3`

```console
$ docker pull rocket.chat@sha256:9d79572dcec09f498a180d6100ab96791458e32c0f39be470c03af3cbc34a6ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:3` - linux; amd64

```console
$ docker pull rocket.chat@sha256:50665a626768b99068ed32ab2c94dc94fa142b1c9c007a1479e765c1a672a6be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.0 MB (232048126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10af69eb2e7de00621754f2d9dd4f36c664019bbf36e032f301a41ae384386d1`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:52:28 GMT
ENV NODE_VERSION=12.22.1
# Tue, 29 Mar 2022 18:52:52 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:52:53 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:52:53 GMT
VOLUME [/app/uploads]
# Tue, 29 Mar 2022 18:52:53 GMT
ENV RC_VERSION=3.18.5
# Tue, 29 Mar 2022 18:52:53 GMT
WORKDIR /app
# Tue, 29 Mar 2022 18:53:49 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 29 Mar 2022 18:53:54 GMT
USER rocketchat
# Tue, 29 Mar 2022 18:53:54 GMT
WORKDIR /app/bundle
# Tue, 29 Mar 2022 18:53:54 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 29 Mar 2022 18:53:54 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 18:53:54 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c57473e917e82a6653b6b37e859af0295488c21b96d3a0e49487bd547aa4f0`  
		Last Modified: Tue, 29 Mar 2022 18:56:42 GMT  
		Size: 24.1 MB (24085286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640a9deebf8983a5f31433896ec4f39d41503e01af3291129065dc659d7bbf2c`  
		Last Modified: Tue, 29 Mar 2022 18:56:37 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9dbd1787387021958b849a9357142f052cd4cb8a5351cb7b79c57f29c7bf2c`  
		Last Modified: Tue, 29 Mar 2022 18:57:12 GMT  
		Size: 180.8 MB (180809063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.18`

```console
$ docker pull rocket.chat@sha256:9d79572dcec09f498a180d6100ab96791458e32c0f39be470c03af3cbc34a6ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:3.18` - linux; amd64

```console
$ docker pull rocket.chat@sha256:50665a626768b99068ed32ab2c94dc94fa142b1c9c007a1479e765c1a672a6be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.0 MB (232048126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10af69eb2e7de00621754f2d9dd4f36c664019bbf36e032f301a41ae384386d1`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:52:28 GMT
ENV NODE_VERSION=12.22.1
# Tue, 29 Mar 2022 18:52:52 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:52:53 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:52:53 GMT
VOLUME [/app/uploads]
# Tue, 29 Mar 2022 18:52:53 GMT
ENV RC_VERSION=3.18.5
# Tue, 29 Mar 2022 18:52:53 GMT
WORKDIR /app
# Tue, 29 Mar 2022 18:53:49 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 29 Mar 2022 18:53:54 GMT
USER rocketchat
# Tue, 29 Mar 2022 18:53:54 GMT
WORKDIR /app/bundle
# Tue, 29 Mar 2022 18:53:54 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 29 Mar 2022 18:53:54 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 18:53:54 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c57473e917e82a6653b6b37e859af0295488c21b96d3a0e49487bd547aa4f0`  
		Last Modified: Tue, 29 Mar 2022 18:56:42 GMT  
		Size: 24.1 MB (24085286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640a9deebf8983a5f31433896ec4f39d41503e01af3291129065dc659d7bbf2c`  
		Last Modified: Tue, 29 Mar 2022 18:56:37 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9dbd1787387021958b849a9357142f052cd4cb8a5351cb7b79c57f29c7bf2c`  
		Last Modified: Tue, 29 Mar 2022 18:57:12 GMT  
		Size: 180.8 MB (180809063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.18.5`

```console
$ docker pull rocket.chat@sha256:9d79572dcec09f498a180d6100ab96791458e32c0f39be470c03af3cbc34a6ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:3.18.5` - linux; amd64

```console
$ docker pull rocket.chat@sha256:50665a626768b99068ed32ab2c94dc94fa142b1c9c007a1479e765c1a672a6be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.0 MB (232048126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10af69eb2e7de00621754f2d9dd4f36c664019bbf36e032f301a41ae384386d1`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:52:28 GMT
ENV NODE_VERSION=12.22.1
# Tue, 29 Mar 2022 18:52:52 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:52:53 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:52:53 GMT
VOLUME [/app/uploads]
# Tue, 29 Mar 2022 18:52:53 GMT
ENV RC_VERSION=3.18.5
# Tue, 29 Mar 2022 18:52:53 GMT
WORKDIR /app
# Tue, 29 Mar 2022 18:53:49 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 29 Mar 2022 18:53:54 GMT
USER rocketchat
# Tue, 29 Mar 2022 18:53:54 GMT
WORKDIR /app/bundle
# Tue, 29 Mar 2022 18:53:54 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 29 Mar 2022 18:53:54 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 18:53:54 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c57473e917e82a6653b6b37e859af0295488c21b96d3a0e49487bd547aa4f0`  
		Last Modified: Tue, 29 Mar 2022 18:56:42 GMT  
		Size: 24.1 MB (24085286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640a9deebf8983a5f31433896ec4f39d41503e01af3291129065dc659d7bbf2c`  
		Last Modified: Tue, 29 Mar 2022 18:56:37 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9dbd1787387021958b849a9357142f052cd4cb8a5351cb7b79c57f29c7bf2c`  
		Last Modified: Tue, 29 Mar 2022 18:57:12 GMT  
		Size: 180.8 MB (180809063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:4`

```console
$ docker pull rocket.chat@sha256:cfafb2db795ccb2d226e28491b5e652ba7e05c95a264031434cc4c1613be6d48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:4` - linux; amd64

```console
$ docker pull rocket.chat@sha256:f1cd6447cc0d417c6e4dfd41f2fa53dd33874f5faa90929aaf1e951e34f10b1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.0 MB (242014603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a12f919af4dc2769fa4b4a13b47327668567189369e8452176258ae2f6614e3`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_VERSION=14.18.3
# Tue, 29 Mar 2022 18:47:00 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:47:01 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:47:01 GMT
VOLUME [/app/uploads]
# Mon, 04 Apr 2022 21:51:45 GMT
ENV RC_VERSION=4.6.0
# Mon, 04 Apr 2022 21:51:45 GMT
WORKDIR /app
# Mon, 04 Apr 2022 21:52:43 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Mon, 04 Apr 2022 21:52:48 GMT
USER rocketchat
# Mon, 04 Apr 2022 21:52:48 GMT
WORKDIR /app/bundle
# Mon, 04 Apr 2022 21:52:49 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Mon, 04 Apr 2022 21:52:49 GMT
EXPOSE 3000
# Mon, 04 Apr 2022 21:52:49 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b442f9585ae28c68558a5e9ffbffb97525ae710c6864bcae8a7182c393c616c`  
		Last Modified: Tue, 29 Mar 2022 18:54:26 GMT  
		Size: 35.5 MB (35524646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b93a16bb8903a3d20c827bd974ff1e6bb0c4e009bc1e4e6d8330c7494b0f88b`  
		Last Modified: Tue, 29 Mar 2022 18:54:20 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676642a6cad48760f35bd47eb8148e5b2be02eed4c3bc8f1b3212083b2530558`  
		Last Modified: Mon, 04 Apr 2022 21:53:47 GMT  
		Size: 179.3 MB (179336178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:4.4`

```console
$ docker pull rocket.chat@sha256:cad5f8c1396ca753a0b7163eb1a7e695325ecd706ea4fe20aa9ad60d49bc2505
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:4.4` - linux; amd64

```console
$ docker pull rocket.chat@sha256:add1002cc7822a4a78a078ba00cc56ff99eacd3683da487fff41ac4e5eb18c05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240164313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b619188fa0dd7ff2b8d64fa19eb4f66d35e755b4186ea775cc92c5bb567fa423`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:48:13 GMT
ENV NODE_VERSION=14.18.2
# Tue, 29 Mar 2022 18:48:37 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:48:38 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:48:38 GMT
VOLUME [/app/uploads]
# Tue, 29 Mar 2022 18:48:38 GMT
ENV RC_VERSION=4.4.2
# Tue, 29 Mar 2022 18:48:38 GMT
WORKDIR /app
# Tue, 29 Mar 2022 18:49:36 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 29 Mar 2022 18:49:41 GMT
USER rocketchat
# Tue, 29 Mar 2022 18:49:41 GMT
WORKDIR /app/bundle
# Tue, 29 Mar 2022 18:49:41 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 29 Mar 2022 18:49:41 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 18:49:41 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cd995d594ebd9a3a99c96085420c6f317e835654f412a1866fcbc4b5a4515b`  
		Last Modified: Tue, 29 Mar 2022 18:55:14 GMT  
		Size: 35.5 MB (35525071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19ec3089c9bfd3dc929ca3b736e335addc3cd2b8f70bd96de9d83bd40bc964f`  
		Last Modified: Tue, 29 Mar 2022 18:55:08 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec4cd6f378eb533cdf7d51cb7d2729018718a4ada6209817be169eafc3f4bf4`  
		Last Modified: Tue, 29 Mar 2022 18:55:42 GMT  
		Size: 177.5 MB (177485464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:4.4.2`

```console
$ docker pull rocket.chat@sha256:cad5f8c1396ca753a0b7163eb1a7e695325ecd706ea4fe20aa9ad60d49bc2505
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:4.4.2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:add1002cc7822a4a78a078ba00cc56ff99eacd3683da487fff41ac4e5eb18c05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240164313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b619188fa0dd7ff2b8d64fa19eb4f66d35e755b4186ea775cc92c5bb567fa423`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:48:13 GMT
ENV NODE_VERSION=14.18.2
# Tue, 29 Mar 2022 18:48:37 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       4ED778F539E3634C779C87C6D7062848A1AB005C       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       74F12602B6F1C4E913FAA37AD3A89613643B6201       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       A48C2BEE680E841632CD4E44F07496B3EB3C1762       108F52B48DB57BB0CC439B2997B01419BD92F80A       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:48:38 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:48:38 GMT
VOLUME [/app/uploads]
# Tue, 29 Mar 2022 18:48:38 GMT
ENV RC_VERSION=4.4.2
# Tue, 29 Mar 2022 18:48:38 GMT
WORKDIR /app
# Tue, 29 Mar 2022 18:49:36 GMT
RUN set -eux &&  apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg && rm -rf /var/lib/apt/lists/* &&  gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104 &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 29 Mar 2022 18:49:41 GMT
USER rocketchat
# Tue, 29 Mar 2022 18:49:41 GMT
WORKDIR /app/bundle
# Tue, 29 Mar 2022 18:49:41 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 29 Mar 2022 18:49:41 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 18:49:41 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4cd995d594ebd9a3a99c96085420c6f317e835654f412a1866fcbc4b5a4515b`  
		Last Modified: Tue, 29 Mar 2022 18:55:14 GMT  
		Size: 35.5 MB (35525071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19ec3089c9bfd3dc929ca3b736e335addc3cd2b8f70bd96de9d83bd40bc964f`  
		Last Modified: Tue, 29 Mar 2022 18:55:08 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec4cd6f378eb533cdf7d51cb7d2729018718a4ada6209817be169eafc3f4bf4`  
		Last Modified: Tue, 29 Mar 2022 18:55:42 GMT  
		Size: 177.5 MB (177485464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:4.5`

```console
$ docker pull rocket.chat@sha256:e4c68cdaa87d030b4528152121aeb6ee96f62564b8c5a6aa568f4b239a3d5b40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:4.5` - linux; amd64

```console
$ docker pull rocket.chat@sha256:2d28bd06003b6181487dd09f8c1e45e84a892c08264352364a296deb1a29b3c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.5 MB (241536742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab109f186607232d09fa7bfd2e3b5223762d1769b403fe466ea00e10cce7357`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_VERSION=14.18.3
# Tue, 29 Mar 2022 18:47:00 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:47:01 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:47:01 GMT
VOLUME [/app/uploads]
# Fri, 01 Apr 2022 02:27:58 GMT
ENV RC_VERSION=4.5.5
# Fri, 01 Apr 2022 02:27:58 GMT
WORKDIR /app
# Fri, 01 Apr 2022 02:28:59 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Fri, 01 Apr 2022 02:29:04 GMT
USER rocketchat
# Fri, 01 Apr 2022 02:29:04 GMT
WORKDIR /app/bundle
# Fri, 01 Apr 2022 02:29:04 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Fri, 01 Apr 2022 02:29:04 GMT
EXPOSE 3000
# Fri, 01 Apr 2022 02:29:04 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b442f9585ae28c68558a5e9ffbffb97525ae710c6864bcae8a7182c393c616c`  
		Last Modified: Tue, 29 Mar 2022 18:54:26 GMT  
		Size: 35.5 MB (35524646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b93a16bb8903a3d20c827bd974ff1e6bb0c4e009bc1e4e6d8330c7494b0f88b`  
		Last Modified: Tue, 29 Mar 2022 18:54:20 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e209e69e6b559f4d9efc65576cac81ee152bff66e9f37c1094b396c98aa30c1`  
		Last Modified: Fri, 01 Apr 2022 02:29:59 GMT  
		Size: 178.9 MB (178858317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:4.5.5`

```console
$ docker pull rocket.chat@sha256:e4c68cdaa87d030b4528152121aeb6ee96f62564b8c5a6aa568f4b239a3d5b40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:4.5.5` - linux; amd64

```console
$ docker pull rocket.chat@sha256:2d28bd06003b6181487dd09f8c1e45e84a892c08264352364a296deb1a29b3c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.5 MB (241536742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab109f186607232d09fa7bfd2e3b5223762d1769b403fe466ea00e10cce7357`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_VERSION=14.18.3
# Tue, 29 Mar 2022 18:47:00 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:47:01 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:47:01 GMT
VOLUME [/app/uploads]
# Fri, 01 Apr 2022 02:27:58 GMT
ENV RC_VERSION=4.5.5
# Fri, 01 Apr 2022 02:27:58 GMT
WORKDIR /app
# Fri, 01 Apr 2022 02:28:59 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Fri, 01 Apr 2022 02:29:04 GMT
USER rocketchat
# Fri, 01 Apr 2022 02:29:04 GMT
WORKDIR /app/bundle
# Fri, 01 Apr 2022 02:29:04 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Fri, 01 Apr 2022 02:29:04 GMT
EXPOSE 3000
# Fri, 01 Apr 2022 02:29:04 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b442f9585ae28c68558a5e9ffbffb97525ae710c6864bcae8a7182c393c616c`  
		Last Modified: Tue, 29 Mar 2022 18:54:26 GMT  
		Size: 35.5 MB (35524646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b93a16bb8903a3d20c827bd974ff1e6bb0c4e009bc1e4e6d8330c7494b0f88b`  
		Last Modified: Tue, 29 Mar 2022 18:54:20 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e209e69e6b559f4d9efc65576cac81ee152bff66e9f37c1094b396c98aa30c1`  
		Last Modified: Fri, 01 Apr 2022 02:29:59 GMT  
		Size: 178.9 MB (178858317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:4.6`

```console
$ docker pull rocket.chat@sha256:cfafb2db795ccb2d226e28491b5e652ba7e05c95a264031434cc4c1613be6d48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:4.6` - linux; amd64

```console
$ docker pull rocket.chat@sha256:f1cd6447cc0d417c6e4dfd41f2fa53dd33874f5faa90929aaf1e951e34f10b1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.0 MB (242014603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a12f919af4dc2769fa4b4a13b47327668567189369e8452176258ae2f6614e3`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_VERSION=14.18.3
# Tue, 29 Mar 2022 18:47:00 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:47:01 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:47:01 GMT
VOLUME [/app/uploads]
# Mon, 04 Apr 2022 21:51:45 GMT
ENV RC_VERSION=4.6.0
# Mon, 04 Apr 2022 21:51:45 GMT
WORKDIR /app
# Mon, 04 Apr 2022 21:52:43 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Mon, 04 Apr 2022 21:52:48 GMT
USER rocketchat
# Mon, 04 Apr 2022 21:52:48 GMT
WORKDIR /app/bundle
# Mon, 04 Apr 2022 21:52:49 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Mon, 04 Apr 2022 21:52:49 GMT
EXPOSE 3000
# Mon, 04 Apr 2022 21:52:49 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b442f9585ae28c68558a5e9ffbffb97525ae710c6864bcae8a7182c393c616c`  
		Last Modified: Tue, 29 Mar 2022 18:54:26 GMT  
		Size: 35.5 MB (35524646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b93a16bb8903a3d20c827bd974ff1e6bb0c4e009bc1e4e6d8330c7494b0f88b`  
		Last Modified: Tue, 29 Mar 2022 18:54:20 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676642a6cad48760f35bd47eb8148e5b2be02eed4c3bc8f1b3212083b2530558`  
		Last Modified: Mon, 04 Apr 2022 21:53:47 GMT  
		Size: 179.3 MB (179336178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:4.6.0`

```console
$ docker pull rocket.chat@sha256:cfafb2db795ccb2d226e28491b5e652ba7e05c95a264031434cc4c1613be6d48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:4.6.0` - linux; amd64

```console
$ docker pull rocket.chat@sha256:f1cd6447cc0d417c6e4dfd41f2fa53dd33874f5faa90929aaf1e951e34f10b1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.0 MB (242014603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a12f919af4dc2769fa4b4a13b47327668567189369e8452176258ae2f6614e3`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_VERSION=14.18.3
# Tue, 29 Mar 2022 18:47:00 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:47:01 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:47:01 GMT
VOLUME [/app/uploads]
# Mon, 04 Apr 2022 21:51:45 GMT
ENV RC_VERSION=4.6.0
# Mon, 04 Apr 2022 21:51:45 GMT
WORKDIR /app
# Mon, 04 Apr 2022 21:52:43 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Mon, 04 Apr 2022 21:52:48 GMT
USER rocketchat
# Mon, 04 Apr 2022 21:52:48 GMT
WORKDIR /app/bundle
# Mon, 04 Apr 2022 21:52:49 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Mon, 04 Apr 2022 21:52:49 GMT
EXPOSE 3000
# Mon, 04 Apr 2022 21:52:49 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b442f9585ae28c68558a5e9ffbffb97525ae710c6864bcae8a7182c393c616c`  
		Last Modified: Tue, 29 Mar 2022 18:54:26 GMT  
		Size: 35.5 MB (35524646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b93a16bb8903a3d20c827bd974ff1e6bb0c4e009bc1e4e6d8330c7494b0f88b`  
		Last Modified: Tue, 29 Mar 2022 18:54:20 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676642a6cad48760f35bd47eb8148e5b2be02eed4c3bc8f1b3212083b2530558`  
		Last Modified: Mon, 04 Apr 2022 21:53:47 GMT  
		Size: 179.3 MB (179336178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:cfafb2db795ccb2d226e28491b5e652ba7e05c95a264031434cc4c1613be6d48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:f1cd6447cc0d417c6e4dfd41f2fa53dd33874f5faa90929aaf1e951e34f10b1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.0 MB (242014603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a12f919af4dc2769fa4b4a13b47327668567189369e8452176258ae2f6614e3`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:38 GMT
ADD file:59187422476c57db46e60f894a4cfd0f243e80230ef9ea75b2d8dd4925d59df3 in / 
# Tue, 29 Mar 2022 00:22:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_ENV=production
# Tue, 29 Mar 2022 18:46:35 GMT
ENV NODE_VERSION=14.18.3
# Tue, 29 Mar 2022 18:47:00 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 18:47:01 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 29 Mar 2022 18:47:01 GMT
VOLUME [/app/uploads]
# Mon, 04 Apr 2022 21:51:45 GMT
ENV RC_VERSION=4.6.0
# Mon, 04 Apr 2022 21:51:45 GMT
WORKDIR /app
# Mon, 04 Apr 2022 21:52:43 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Mon, 04 Apr 2022 21:52:48 GMT
USER rocketchat
# Mon, 04 Apr 2022 21:52:48 GMT
WORKDIR /app/bundle
# Mon, 04 Apr 2022 21:52:49 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Mon, 04 Apr 2022 21:52:49 GMT
EXPOSE 3000
# Mon, 04 Apr 2022 21:52:49 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f003217c5aaebdfee0b9a448fbabd995e5f0159f5b231460c0ecc21baf171953`  
		Last Modified: Tue, 29 Mar 2022 00:28:02 GMT  
		Size: 27.2 MB (27151970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b442f9585ae28c68558a5e9ffbffb97525ae710c6864bcae8a7182c393c616c`  
		Last Modified: Tue, 29 Mar 2022 18:54:26 GMT  
		Size: 35.5 MB (35524646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b93a16bb8903a3d20c827bd974ff1e6bb0c4e009bc1e4e6d8330c7494b0f88b`  
		Last Modified: Tue, 29 Mar 2022 18:54:20 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676642a6cad48760f35bd47eb8148e5b2be02eed4c3bc8f1b3212083b2530558`  
		Last Modified: Mon, 04 Apr 2022 21:53:47 GMT  
		Size: 179.3 MB (179336178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
