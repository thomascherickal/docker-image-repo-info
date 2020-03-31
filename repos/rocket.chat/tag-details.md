<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rocket.chat`

-	[`rocket.chat:2`](#rocketchat2)
-	[`rocket.chat:2.4`](#rocketchat24)
-	[`rocket.chat:2.4.11`](#rocketchat2411)
-	[`rocket.chat:3`](#rocketchat3)
-	[`rocket.chat:3.0`](#rocketchat30)
-	[`rocket.chat:3.0.7`](#rocketchat307)
-	[`rocket.chat:latest`](#rocketchatlatest)

## `rocket.chat:2`

```console
$ docker pull rocket.chat@sha256:2128626fe69f5d8ce6867ecc3ffeb1b007ce004655144a4adcfdda344f8da106
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:3a08548f6c78d79653ea00feb5d60aa4a3b2149178b542bdab2c8b345efeba4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230024444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7716427b5cfb92727e8863a77f6eeee4ea81795b59ba591e6a90cabd094bd656`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:29 GMT
ADD file:a608eb5aef5e5a93290d263faec3564b4cdeebb2c3596cd3e0b6d16708702e95 in / 
# Tue, 31 Mar 2020 01:21:30 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_ENV=production
# Tue, 31 Mar 2020 20:35:21 GMT
ENV NODE_VERSION=8.17.0
# Tue, 31 Mar 2020 20:38:13 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 31 Mar 2020 20:38:14 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 31 Mar 2020 20:38:15 GMT
VOLUME [/app/uploads]
# Tue, 31 Mar 2020 20:38:17 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 31 Mar 2020 20:38:17 GMT
ENV RC_VERSION=2.4.11
# Tue, 31 Mar 2020 20:38:17 GMT
WORKDIR /app
# Tue, 31 Mar 2020 20:43:07 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 31 Mar 2020 20:43:10 GMT
USER rocketchat
# Tue, 31 Mar 2020 20:43:11 GMT
WORKDIR /app/bundle
# Tue, 31 Mar 2020 20:43:11 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 31 Mar 2020 20:43:11 GMT
EXPOSE 3000
# Tue, 31 Mar 2020 20:43:12 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:a8ae8a1bb8caea4adfc9e40f1873b018b04b858d6467be8ee7f9edf902ed02bc`  
		Last Modified: Tue, 31 Mar 2020 01:27:09 GMT  
		Size: 30.2 MB (30159663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd24688d90e6b8fe7398f3b51d9e40c08bb302d39e7fe50570d093fac645d98`  
		Last Modified: Tue, 31 Mar 2020 20:44:40 GMT  
		Size: 19.9 MB (19944317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20c611779ea60b3274dd6c1c7c15c263e1da1950ca2717d64b0928037e4e50f`  
		Last Modified: Tue, 31 Mar 2020 20:44:32 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb49b515ba8b3a5ff036264c7fdc09f8a9bf19e5b61550d54be375a5019b2e5`  
		Last Modified: Tue, 31 Mar 2020 20:44:32 GMT  
		Size: 170.7 KB (170734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d941bbf08284900912cd8e0db1790dcdaece354449624a4992f4e61b4cb32`  
		Last Modified: Tue, 31 Mar 2020 20:45:20 GMT  
		Size: 179.7 MB (179747591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4`

```console
$ docker pull rocket.chat@sha256:2128626fe69f5d8ce6867ecc3ffeb1b007ce004655144a4adcfdda344f8da106
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2.4` - linux; amd64

```console
$ docker pull rocket.chat@sha256:3a08548f6c78d79653ea00feb5d60aa4a3b2149178b542bdab2c8b345efeba4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230024444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7716427b5cfb92727e8863a77f6eeee4ea81795b59ba591e6a90cabd094bd656`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:29 GMT
ADD file:a608eb5aef5e5a93290d263faec3564b4cdeebb2c3596cd3e0b6d16708702e95 in / 
# Tue, 31 Mar 2020 01:21:30 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_ENV=production
# Tue, 31 Mar 2020 20:35:21 GMT
ENV NODE_VERSION=8.17.0
# Tue, 31 Mar 2020 20:38:13 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 31 Mar 2020 20:38:14 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 31 Mar 2020 20:38:15 GMT
VOLUME [/app/uploads]
# Tue, 31 Mar 2020 20:38:17 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 31 Mar 2020 20:38:17 GMT
ENV RC_VERSION=2.4.11
# Tue, 31 Mar 2020 20:38:17 GMT
WORKDIR /app
# Tue, 31 Mar 2020 20:43:07 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 31 Mar 2020 20:43:10 GMT
USER rocketchat
# Tue, 31 Mar 2020 20:43:11 GMT
WORKDIR /app/bundle
# Tue, 31 Mar 2020 20:43:11 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 31 Mar 2020 20:43:11 GMT
EXPOSE 3000
# Tue, 31 Mar 2020 20:43:12 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:a8ae8a1bb8caea4adfc9e40f1873b018b04b858d6467be8ee7f9edf902ed02bc`  
		Last Modified: Tue, 31 Mar 2020 01:27:09 GMT  
		Size: 30.2 MB (30159663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd24688d90e6b8fe7398f3b51d9e40c08bb302d39e7fe50570d093fac645d98`  
		Last Modified: Tue, 31 Mar 2020 20:44:40 GMT  
		Size: 19.9 MB (19944317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20c611779ea60b3274dd6c1c7c15c263e1da1950ca2717d64b0928037e4e50f`  
		Last Modified: Tue, 31 Mar 2020 20:44:32 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb49b515ba8b3a5ff036264c7fdc09f8a9bf19e5b61550d54be375a5019b2e5`  
		Last Modified: Tue, 31 Mar 2020 20:44:32 GMT  
		Size: 170.7 KB (170734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d941bbf08284900912cd8e0db1790dcdaece354449624a4992f4e61b4cb32`  
		Last Modified: Tue, 31 Mar 2020 20:45:20 GMT  
		Size: 179.7 MB (179747591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4.11`

```console
$ docker pull rocket.chat@sha256:2128626fe69f5d8ce6867ecc3ffeb1b007ce004655144a4adcfdda344f8da106
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2.4.11` - linux; amd64

```console
$ docker pull rocket.chat@sha256:3a08548f6c78d79653ea00feb5d60aa4a3b2149178b542bdab2c8b345efeba4a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230024444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7716427b5cfb92727e8863a77f6eeee4ea81795b59ba591e6a90cabd094bd656`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:29 GMT
ADD file:a608eb5aef5e5a93290d263faec3564b4cdeebb2c3596cd3e0b6d16708702e95 in / 
# Tue, 31 Mar 2020 01:21:30 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_ENV=production
# Tue, 31 Mar 2020 20:35:21 GMT
ENV NODE_VERSION=8.17.0
# Tue, 31 Mar 2020 20:38:13 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 31 Mar 2020 20:38:14 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 31 Mar 2020 20:38:15 GMT
VOLUME [/app/uploads]
# Tue, 31 Mar 2020 20:38:17 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 31 Mar 2020 20:38:17 GMT
ENV RC_VERSION=2.4.11
# Tue, 31 Mar 2020 20:38:17 GMT
WORKDIR /app
# Tue, 31 Mar 2020 20:43:07 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 31 Mar 2020 20:43:10 GMT
USER rocketchat
# Tue, 31 Mar 2020 20:43:11 GMT
WORKDIR /app/bundle
# Tue, 31 Mar 2020 20:43:11 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 31 Mar 2020 20:43:11 GMT
EXPOSE 3000
# Tue, 31 Mar 2020 20:43:12 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:a8ae8a1bb8caea4adfc9e40f1873b018b04b858d6467be8ee7f9edf902ed02bc`  
		Last Modified: Tue, 31 Mar 2020 01:27:09 GMT  
		Size: 30.2 MB (30159663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd24688d90e6b8fe7398f3b51d9e40c08bb302d39e7fe50570d093fac645d98`  
		Last Modified: Tue, 31 Mar 2020 20:44:40 GMT  
		Size: 19.9 MB (19944317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20c611779ea60b3274dd6c1c7c15c263e1da1950ca2717d64b0928037e4e50f`  
		Last Modified: Tue, 31 Mar 2020 20:44:32 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb49b515ba8b3a5ff036264c7fdc09f8a9bf19e5b61550d54be375a5019b2e5`  
		Last Modified: Tue, 31 Mar 2020 20:44:32 GMT  
		Size: 170.7 KB (170734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8d941bbf08284900912cd8e0db1790dcdaece354449624a4992f4e61b4cb32`  
		Last Modified: Tue, 31 Mar 2020 20:45:20 GMT  
		Size: 179.7 MB (179747591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3`

```console
$ docker pull rocket.chat@sha256:91f45714bba112990e89e8dda5c2d76c715d52a3e5a1cdef79b3c69beedb8203
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3` - linux; amd64

```console
$ docker pull rocket.chat@sha256:22f7c79dee6448acd9a77bae3e49325f401c1b0c31c92a39c54d47c3cf461e71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226135670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3ba52c2f25f689fc874c18881667fefec5d1b2ebb8c349e52239ad36f5b4f6b`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:29 GMT
ADD file:a608eb5aef5e5a93290d263faec3564b4cdeebb2c3596cd3e0b6d16708702e95 in / 
# Tue, 31 Mar 2020 01:21:30 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_ENV=production
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_VERSION=12.14.0
# Tue, 31 Mar 2020 20:29:27 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 31 Mar 2020 20:29:29 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 31 Mar 2020 20:29:29 GMT
VOLUME [/app/uploads]
# Tue, 31 Mar 2020 20:29:31 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 31 Mar 2020 20:29:31 GMT
ENV RC_VERSION=3.0.7
# Tue, 31 Mar 2020 20:29:32 GMT
WORKDIR /app
# Tue, 31 Mar 2020 20:35:01 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 31 Mar 2020 20:35:03 GMT
USER rocketchat
# Tue, 31 Mar 2020 20:35:03 GMT
WORKDIR /app/bundle
# Tue, 31 Mar 2020 20:35:04 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 31 Mar 2020 20:35:04 GMT
EXPOSE 3000
# Tue, 31 Mar 2020 20:35:04 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:a8ae8a1bb8caea4adfc9e40f1873b018b04b858d6467be8ee7f9edf902ed02bc`  
		Last Modified: Tue, 31 Mar 2020 01:27:09 GMT  
		Size: 30.2 MB (30159663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6d376e3536f6ab4064c5485bd2f563b4d090cfbb6e48ba7349373fbe3479c1`  
		Last Modified: Tue, 31 Mar 2020 20:43:40 GMT  
		Size: 24.0 MB (23991691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4baaaf9d474e54882cd067bfa96e894d6e037a9d0e9efe3f4ef7c83c773e5`  
		Last Modified: Tue, 31 Mar 2020 20:43:32 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d43c4a94fa978c4e4cd255436c2f47ede74aed95c0ecc5dd31d16727f91d09c`  
		Last Modified: Tue, 31 Mar 2020 20:43:32 GMT  
		Size: 170.7 KB (170734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004612de2b531451f1793908c680b306829c50895ae07b75ff49062e7fe38bad`  
		Last Modified: Tue, 31 Mar 2020 20:44:24 GMT  
		Size: 171.8 MB (171811443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.0`

```console
$ docker pull rocket.chat@sha256:91f45714bba112990e89e8dda5c2d76c715d52a3e5a1cdef79b3c69beedb8203
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.0` - linux; amd64

```console
$ docker pull rocket.chat@sha256:22f7c79dee6448acd9a77bae3e49325f401c1b0c31c92a39c54d47c3cf461e71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226135670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3ba52c2f25f689fc874c18881667fefec5d1b2ebb8c349e52239ad36f5b4f6b`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:29 GMT
ADD file:a608eb5aef5e5a93290d263faec3564b4cdeebb2c3596cd3e0b6d16708702e95 in / 
# Tue, 31 Mar 2020 01:21:30 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_ENV=production
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_VERSION=12.14.0
# Tue, 31 Mar 2020 20:29:27 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 31 Mar 2020 20:29:29 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 31 Mar 2020 20:29:29 GMT
VOLUME [/app/uploads]
# Tue, 31 Mar 2020 20:29:31 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 31 Mar 2020 20:29:31 GMT
ENV RC_VERSION=3.0.7
# Tue, 31 Mar 2020 20:29:32 GMT
WORKDIR /app
# Tue, 31 Mar 2020 20:35:01 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 31 Mar 2020 20:35:03 GMT
USER rocketchat
# Tue, 31 Mar 2020 20:35:03 GMT
WORKDIR /app/bundle
# Tue, 31 Mar 2020 20:35:04 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 31 Mar 2020 20:35:04 GMT
EXPOSE 3000
# Tue, 31 Mar 2020 20:35:04 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:a8ae8a1bb8caea4adfc9e40f1873b018b04b858d6467be8ee7f9edf902ed02bc`  
		Last Modified: Tue, 31 Mar 2020 01:27:09 GMT  
		Size: 30.2 MB (30159663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6d376e3536f6ab4064c5485bd2f563b4d090cfbb6e48ba7349373fbe3479c1`  
		Last Modified: Tue, 31 Mar 2020 20:43:40 GMT  
		Size: 24.0 MB (23991691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4baaaf9d474e54882cd067bfa96e894d6e037a9d0e9efe3f4ef7c83c773e5`  
		Last Modified: Tue, 31 Mar 2020 20:43:32 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d43c4a94fa978c4e4cd255436c2f47ede74aed95c0ecc5dd31d16727f91d09c`  
		Last Modified: Tue, 31 Mar 2020 20:43:32 GMT  
		Size: 170.7 KB (170734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004612de2b531451f1793908c680b306829c50895ae07b75ff49062e7fe38bad`  
		Last Modified: Tue, 31 Mar 2020 20:44:24 GMT  
		Size: 171.8 MB (171811443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.0.7`

```console
$ docker pull rocket.chat@sha256:91f45714bba112990e89e8dda5c2d76c715d52a3e5a1cdef79b3c69beedb8203
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.0.7` - linux; amd64

```console
$ docker pull rocket.chat@sha256:22f7c79dee6448acd9a77bae3e49325f401c1b0c31c92a39c54d47c3cf461e71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226135670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3ba52c2f25f689fc874c18881667fefec5d1b2ebb8c349e52239ad36f5b4f6b`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:29 GMT
ADD file:a608eb5aef5e5a93290d263faec3564b4cdeebb2c3596cd3e0b6d16708702e95 in / 
# Tue, 31 Mar 2020 01:21:30 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_ENV=production
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_VERSION=12.14.0
# Tue, 31 Mar 2020 20:29:27 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 31 Mar 2020 20:29:29 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 31 Mar 2020 20:29:29 GMT
VOLUME [/app/uploads]
# Tue, 31 Mar 2020 20:29:31 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 31 Mar 2020 20:29:31 GMT
ENV RC_VERSION=3.0.7
# Tue, 31 Mar 2020 20:29:32 GMT
WORKDIR /app
# Tue, 31 Mar 2020 20:35:01 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 31 Mar 2020 20:35:03 GMT
USER rocketchat
# Tue, 31 Mar 2020 20:35:03 GMT
WORKDIR /app/bundle
# Tue, 31 Mar 2020 20:35:04 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 31 Mar 2020 20:35:04 GMT
EXPOSE 3000
# Tue, 31 Mar 2020 20:35:04 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:a8ae8a1bb8caea4adfc9e40f1873b018b04b858d6467be8ee7f9edf902ed02bc`  
		Last Modified: Tue, 31 Mar 2020 01:27:09 GMT  
		Size: 30.2 MB (30159663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6d376e3536f6ab4064c5485bd2f563b4d090cfbb6e48ba7349373fbe3479c1`  
		Last Modified: Tue, 31 Mar 2020 20:43:40 GMT  
		Size: 24.0 MB (23991691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4baaaf9d474e54882cd067bfa96e894d6e037a9d0e9efe3f4ef7c83c773e5`  
		Last Modified: Tue, 31 Mar 2020 20:43:32 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d43c4a94fa978c4e4cd255436c2f47ede74aed95c0ecc5dd31d16727f91d09c`  
		Last Modified: Tue, 31 Mar 2020 20:43:32 GMT  
		Size: 170.7 KB (170734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004612de2b531451f1793908c680b306829c50895ae07b75ff49062e7fe38bad`  
		Last Modified: Tue, 31 Mar 2020 20:44:24 GMT  
		Size: 171.8 MB (171811443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:91f45714bba112990e89e8dda5c2d76c715d52a3e5a1cdef79b3c69beedb8203
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:22f7c79dee6448acd9a77bae3e49325f401c1b0c31c92a39c54d47c3cf461e71
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226135670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3ba52c2f25f689fc874c18881667fefec5d1b2ebb8c349e52239ad36f5b4f6b`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:29 GMT
ADD file:a608eb5aef5e5a93290d263faec3564b4cdeebb2c3596cd3e0b6d16708702e95 in / 
# Tue, 31 Mar 2020 01:21:30 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_ENV=production
# Tue, 31 Mar 2020 20:26:32 GMT
ENV NODE_VERSION=12.14.0
# Tue, 31 Mar 2020 20:29:27 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 31 Mar 2020 20:29:29 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Tue, 31 Mar 2020 20:29:29 GMT
VOLUME [/app/uploads]
# Tue, 31 Mar 2020 20:29:31 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Tue, 31 Mar 2020 20:29:31 GMT
ENV RC_VERSION=3.0.7
# Tue, 31 Mar 2020 20:29:32 GMT
WORKDIR /app
# Tue, 31 Mar 2020 20:35:01 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Tue, 31 Mar 2020 20:35:03 GMT
USER rocketchat
# Tue, 31 Mar 2020 20:35:03 GMT
WORKDIR /app/bundle
# Tue, 31 Mar 2020 20:35:04 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 31 Mar 2020 20:35:04 GMT
EXPOSE 3000
# Tue, 31 Mar 2020 20:35:04 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:a8ae8a1bb8caea4adfc9e40f1873b018b04b858d6467be8ee7f9edf902ed02bc`  
		Last Modified: Tue, 31 Mar 2020 01:27:09 GMT  
		Size: 30.2 MB (30159663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6d376e3536f6ab4064c5485bd2f563b4d090cfbb6e48ba7349373fbe3479c1`  
		Last Modified: Tue, 31 Mar 2020 20:43:40 GMT  
		Size: 24.0 MB (23991691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a4baaaf9d474e54882cd067bfa96e894d6e037a9d0e9efe3f4ef7c83c773e5`  
		Last Modified: Tue, 31 Mar 2020 20:43:32 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d43c4a94fa978c4e4cd255436c2f47ede74aed95c0ecc5dd31d16727f91d09c`  
		Last Modified: Tue, 31 Mar 2020 20:43:32 GMT  
		Size: 170.7 KB (170734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004612de2b531451f1793908c680b306829c50895ae07b75ff49062e7fe38bad`  
		Last Modified: Tue, 31 Mar 2020 20:44:24 GMT  
		Size: 171.8 MB (171811443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
