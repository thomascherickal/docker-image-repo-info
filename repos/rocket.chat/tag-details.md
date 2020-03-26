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
$ docker pull rocket.chat@sha256:614710298cd9a38f10b9463b30e21e935eb9b778c50ad8423c81ebec9caa46b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:5b4a8cbaf239e8e57364acd7ec38e768ea828da366f52d3c0c05fd9d966161f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230025114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0cf1479de4d64455d163586df7b9ff736b218aeedef861dc87b921206a4a0d9`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 26 Feb 2020 00:38:14 GMT
ADD file:e136713a1415b6bdfe20d8e37a2b6def6eb2c81ad08ea67b73ac1216107ab73e in / 
# Wed, 26 Feb 2020 00:38:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 02:35:59 GMT
ENV NODE_ENV=production
# Fri, 06 Mar 2020 02:44:49 GMT
ENV NODE_VERSION=8.17.0
# Fri, 06 Mar 2020 02:47:57 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 06 Mar 2020 02:47:58 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Fri, 06 Mar 2020 02:47:59 GMT
VOLUME [/app/uploads]
# Fri, 06 Mar 2020 02:48:00 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Fri, 06 Mar 2020 02:48:01 GMT
ENV RC_VERSION=2.4.11
# Fri, 06 Mar 2020 02:48:01 GMT
WORKDIR /app
# Fri, 06 Mar 2020 02:53:15 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Fri, 06 Mar 2020 02:53:18 GMT
USER rocketchat
# Fri, 06 Mar 2020 02:53:19 GMT
WORKDIR /app/bundle
# Fri, 06 Mar 2020 02:53:19 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Fri, 06 Mar 2020 02:53:20 GMT
EXPOSE 3000
# Fri, 06 Mar 2020 02:53:20 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:ad10394a96ec2ef0a20a97cf25199c27e8251f0a596a02431d18fee7d5e4f534`  
		Last Modified: Wed, 26 Feb 2020 00:44:53 GMT  
		Size: 30.2 MB (30159549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32214a09c23818a7afc62e1b6fe164fe08e1392fb87432d7d02ac30d503ffc3e`  
		Last Modified: Fri, 06 Mar 2020 02:54:52 GMT  
		Size: 19.9 MB (19930882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36649438e8bd440d2900ab1dca3134aa2b953b596228a8aa3c0d351e9e3d696c`  
		Last Modified: Fri, 06 Mar 2020 02:54:41 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d9a050af3b592915e6f126d1f801b007c270592e25fb296332b9aced5b746d`  
		Last Modified: Fri, 06 Mar 2020 02:54:41 GMT  
		Size: 161.2 KB (161211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e3a4cb9cac0ec74d9b8a45df3a9baef0929292728a270c2d8384ddc5dc1c5`  
		Last Modified: Fri, 06 Mar 2020 02:55:38 GMT  
		Size: 179.8 MB (179771333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4`

```console
$ docker pull rocket.chat@sha256:614710298cd9a38f10b9463b30e21e935eb9b778c50ad8423c81ebec9caa46b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2.4` - linux; amd64

```console
$ docker pull rocket.chat@sha256:5b4a8cbaf239e8e57364acd7ec38e768ea828da366f52d3c0c05fd9d966161f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230025114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0cf1479de4d64455d163586df7b9ff736b218aeedef861dc87b921206a4a0d9`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 26 Feb 2020 00:38:14 GMT
ADD file:e136713a1415b6bdfe20d8e37a2b6def6eb2c81ad08ea67b73ac1216107ab73e in / 
# Wed, 26 Feb 2020 00:38:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 02:35:59 GMT
ENV NODE_ENV=production
# Fri, 06 Mar 2020 02:44:49 GMT
ENV NODE_VERSION=8.17.0
# Fri, 06 Mar 2020 02:47:57 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 06 Mar 2020 02:47:58 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Fri, 06 Mar 2020 02:47:59 GMT
VOLUME [/app/uploads]
# Fri, 06 Mar 2020 02:48:00 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Fri, 06 Mar 2020 02:48:01 GMT
ENV RC_VERSION=2.4.11
# Fri, 06 Mar 2020 02:48:01 GMT
WORKDIR /app
# Fri, 06 Mar 2020 02:53:15 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Fri, 06 Mar 2020 02:53:18 GMT
USER rocketchat
# Fri, 06 Mar 2020 02:53:19 GMT
WORKDIR /app/bundle
# Fri, 06 Mar 2020 02:53:19 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Fri, 06 Mar 2020 02:53:20 GMT
EXPOSE 3000
# Fri, 06 Mar 2020 02:53:20 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:ad10394a96ec2ef0a20a97cf25199c27e8251f0a596a02431d18fee7d5e4f534`  
		Last Modified: Wed, 26 Feb 2020 00:44:53 GMT  
		Size: 30.2 MB (30159549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32214a09c23818a7afc62e1b6fe164fe08e1392fb87432d7d02ac30d503ffc3e`  
		Last Modified: Fri, 06 Mar 2020 02:54:52 GMT  
		Size: 19.9 MB (19930882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36649438e8bd440d2900ab1dca3134aa2b953b596228a8aa3c0d351e9e3d696c`  
		Last Modified: Fri, 06 Mar 2020 02:54:41 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d9a050af3b592915e6f126d1f801b007c270592e25fb296332b9aced5b746d`  
		Last Modified: Fri, 06 Mar 2020 02:54:41 GMT  
		Size: 161.2 KB (161211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e3a4cb9cac0ec74d9b8a45df3a9baef0929292728a270c2d8384ddc5dc1c5`  
		Last Modified: Fri, 06 Mar 2020 02:55:38 GMT  
		Size: 179.8 MB (179771333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4.11`

```console
$ docker pull rocket.chat@sha256:614710298cd9a38f10b9463b30e21e935eb9b778c50ad8423c81ebec9caa46b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2.4.11` - linux; amd64

```console
$ docker pull rocket.chat@sha256:5b4a8cbaf239e8e57364acd7ec38e768ea828da366f52d3c0c05fd9d966161f5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.0 MB (230025114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0cf1479de4d64455d163586df7b9ff736b218aeedef861dc87b921206a4a0d9`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 26 Feb 2020 00:38:14 GMT
ADD file:e136713a1415b6bdfe20d8e37a2b6def6eb2c81ad08ea67b73ac1216107ab73e in / 
# Wed, 26 Feb 2020 00:38:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 02:35:59 GMT
ENV NODE_ENV=production
# Fri, 06 Mar 2020 02:44:49 GMT
ENV NODE_VERSION=8.17.0
# Fri, 06 Mar 2020 02:47:57 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 06 Mar 2020 02:47:58 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Fri, 06 Mar 2020 02:47:59 GMT
VOLUME [/app/uploads]
# Fri, 06 Mar 2020 02:48:00 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Fri, 06 Mar 2020 02:48:01 GMT
ENV RC_VERSION=2.4.11
# Fri, 06 Mar 2020 02:48:01 GMT
WORKDIR /app
# Fri, 06 Mar 2020 02:53:15 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Fri, 06 Mar 2020 02:53:18 GMT
USER rocketchat
# Fri, 06 Mar 2020 02:53:19 GMT
WORKDIR /app/bundle
# Fri, 06 Mar 2020 02:53:19 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Fri, 06 Mar 2020 02:53:20 GMT
EXPOSE 3000
# Fri, 06 Mar 2020 02:53:20 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:ad10394a96ec2ef0a20a97cf25199c27e8251f0a596a02431d18fee7d5e4f534`  
		Last Modified: Wed, 26 Feb 2020 00:44:53 GMT  
		Size: 30.2 MB (30159549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32214a09c23818a7afc62e1b6fe164fe08e1392fb87432d7d02ac30d503ffc3e`  
		Last Modified: Fri, 06 Mar 2020 02:54:52 GMT  
		Size: 19.9 MB (19930882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36649438e8bd440d2900ab1dca3134aa2b953b596228a8aa3c0d351e9e3d696c`  
		Last Modified: Fri, 06 Mar 2020 02:54:41 GMT  
		Size: 2.1 KB (2139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d9a050af3b592915e6f126d1f801b007c270592e25fb296332b9aced5b746d`  
		Last Modified: Fri, 06 Mar 2020 02:54:41 GMT  
		Size: 161.2 KB (161211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e3a4cb9cac0ec74d9b8a45df3a9baef0929292728a270c2d8384ddc5dc1c5`  
		Last Modified: Fri, 06 Mar 2020 02:55:38 GMT  
		Size: 179.8 MB (179771333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3`

```console
$ docker pull rocket.chat@sha256:b6166f034ebcc697afb9a0c6fa96e42acd29ecac343ec0b1a66279f612bffa59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3` - linux; amd64

```console
$ docker pull rocket.chat@sha256:c65b00f49d069509549b96b320c9a17162d658b9ae32c80c25e70f131316e010
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226115899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29131e980715c069316539ead9139496dbcf77c82dde6a018daf56ad516f81fb`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 26 Feb 2020 00:38:14 GMT
ADD file:e136713a1415b6bdfe20d8e37a2b6def6eb2c81ad08ea67b73ac1216107ab73e in / 
# Wed, 26 Feb 2020 00:38:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 02:35:59 GMT
ENV NODE_ENV=production
# Fri, 06 Mar 2020 02:35:59 GMT
ENV NODE_VERSION=12.14.0
# Fri, 06 Mar 2020 02:38:52 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 06 Mar 2020 02:38:54 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Fri, 06 Mar 2020 02:38:55 GMT
VOLUME [/app/uploads]
# Fri, 06 Mar 2020 02:38:56 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Wed, 25 Mar 2020 21:25:59 GMT
ENV RC_VERSION=3.0.6
# Wed, 25 Mar 2020 21:25:59 GMT
WORKDIR /app
# Wed, 25 Mar 2020 21:30:27 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 25 Mar 2020 21:30:29 GMT
USER rocketchat
# Wed, 25 Mar 2020 21:30:29 GMT
WORKDIR /app/bundle
# Wed, 25 Mar 2020 21:30:29 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 25 Mar 2020 21:30:29 GMT
EXPOSE 3000
# Wed, 25 Mar 2020 21:30:29 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:ad10394a96ec2ef0a20a97cf25199c27e8251f0a596a02431d18fee7d5e4f534`  
		Last Modified: Wed, 26 Feb 2020 00:44:53 GMT  
		Size: 30.2 MB (30159549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dd96be30b0aca0bdb1c578a096ec07e7af0a56e209a9d5b3ebb4cbc01c0dc6`  
		Last Modified: Fri, 06 Mar 2020 02:53:45 GMT  
		Size: 24.0 MB (23981486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d508da08e2cdc123dd2bf7d414cd01380f91a1b80feebe3a93f16f752e9400ca`  
		Last Modified: Fri, 06 Mar 2020 02:53:34 GMT  
		Size: 2.1 KB (2143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e443d2aaa022a99032015bf26bb5758d4a1ba61c12361da6467cfec4effb5ef`  
		Last Modified: Fri, 06 Mar 2020 02:53:34 GMT  
		Size: 161.2 KB (161207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c3818ef2400c0556c9559af6af5b4960882d6f2b86f9fd411b2cdc94a60cd6`  
		Last Modified: Wed, 25 Mar 2020 21:31:35 GMT  
		Size: 171.8 MB (171811514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.0`

```console
$ docker pull rocket.chat@sha256:b6166f034ebcc697afb9a0c6fa96e42acd29ecac343ec0b1a66279f612bffa59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:3.0` - linux; amd64

```console
$ docker pull rocket.chat@sha256:c65b00f49d069509549b96b320c9a17162d658b9ae32c80c25e70f131316e010
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226115899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29131e980715c069316539ead9139496dbcf77c82dde6a018daf56ad516f81fb`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 26 Feb 2020 00:38:14 GMT
ADD file:e136713a1415b6bdfe20d8e37a2b6def6eb2c81ad08ea67b73ac1216107ab73e in / 
# Wed, 26 Feb 2020 00:38:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 02:35:59 GMT
ENV NODE_ENV=production
# Fri, 06 Mar 2020 02:35:59 GMT
ENV NODE_VERSION=12.14.0
# Fri, 06 Mar 2020 02:38:52 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 06 Mar 2020 02:38:54 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Fri, 06 Mar 2020 02:38:55 GMT
VOLUME [/app/uploads]
# Fri, 06 Mar 2020 02:38:56 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Wed, 25 Mar 2020 21:25:59 GMT
ENV RC_VERSION=3.0.6
# Wed, 25 Mar 2020 21:25:59 GMT
WORKDIR /app
# Wed, 25 Mar 2020 21:30:27 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 25 Mar 2020 21:30:29 GMT
USER rocketchat
# Wed, 25 Mar 2020 21:30:29 GMT
WORKDIR /app/bundle
# Wed, 25 Mar 2020 21:30:29 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 25 Mar 2020 21:30:29 GMT
EXPOSE 3000
# Wed, 25 Mar 2020 21:30:29 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:ad10394a96ec2ef0a20a97cf25199c27e8251f0a596a02431d18fee7d5e4f534`  
		Last Modified: Wed, 26 Feb 2020 00:44:53 GMT  
		Size: 30.2 MB (30159549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dd96be30b0aca0bdb1c578a096ec07e7af0a56e209a9d5b3ebb4cbc01c0dc6`  
		Last Modified: Fri, 06 Mar 2020 02:53:45 GMT  
		Size: 24.0 MB (23981486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d508da08e2cdc123dd2bf7d414cd01380f91a1b80feebe3a93f16f752e9400ca`  
		Last Modified: Fri, 06 Mar 2020 02:53:34 GMT  
		Size: 2.1 KB (2143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e443d2aaa022a99032015bf26bb5758d4a1ba61c12361da6467cfec4effb5ef`  
		Last Modified: Fri, 06 Mar 2020 02:53:34 GMT  
		Size: 161.2 KB (161207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c3818ef2400c0556c9559af6af5b4960882d6f2b86f9fd411b2cdc94a60cd6`  
		Last Modified: Wed, 25 Mar 2020 21:31:35 GMT  
		Size: 171.8 MB (171811514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:3.0.7`

**does not exist** (yet?)

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:b6166f034ebcc697afb9a0c6fa96e42acd29ecac343ec0b1a66279f612bffa59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:c65b00f49d069509549b96b320c9a17162d658b9ae32c80c25e70f131316e010
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.1 MB (226115899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29131e980715c069316539ead9139496dbcf77c82dde6a018daf56ad516f81fb`
-	Default Command: `["node","main.js"]`

```dockerfile
# Wed, 26 Feb 2020 00:38:14 GMT
ADD file:e136713a1415b6bdfe20d8e37a2b6def6eb2c81ad08ea67b73ac1216107ab73e in / 
# Wed, 26 Feb 2020 00:38:14 GMT
CMD ["bash"]
# Fri, 06 Mar 2020 02:35:59 GMT
ENV NODE_ENV=production
# Fri, 06 Mar 2020 02:35:59 GMT
ENV NODE_VERSION=12.14.0
# Fri, 06 Mar 2020 02:38:52 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 06 Mar 2020 02:38:54 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Fri, 06 Mar 2020 02:38:55 GMT
VOLUME [/app/uploads]
# Fri, 06 Mar 2020 02:38:56 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Wed, 25 Mar 2020 21:25:59 GMT
ENV RC_VERSION=3.0.6
# Wed, 25 Mar 2020 21:25:59 GMT
WORKDIR /app
# Wed, 25 Mar 2020 21:30:27 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Wed, 25 Mar 2020 21:30:29 GMT
USER rocketchat
# Wed, 25 Mar 2020 21:30:29 GMT
WORKDIR /app/bundle
# Wed, 25 Mar 2020 21:30:29 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Wed, 25 Mar 2020 21:30:29 GMT
EXPOSE 3000
# Wed, 25 Mar 2020 21:30:29 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:ad10394a96ec2ef0a20a97cf25199c27e8251f0a596a02431d18fee7d5e4f534`  
		Last Modified: Wed, 26 Feb 2020 00:44:53 GMT  
		Size: 30.2 MB (30159549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dd96be30b0aca0bdb1c578a096ec07e7af0a56e209a9d5b3ebb4cbc01c0dc6`  
		Last Modified: Fri, 06 Mar 2020 02:53:45 GMT  
		Size: 24.0 MB (23981486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d508da08e2cdc123dd2bf7d414cd01380f91a1b80feebe3a93f16f752e9400ca`  
		Last Modified: Fri, 06 Mar 2020 02:53:34 GMT  
		Size: 2.1 KB (2143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e443d2aaa022a99032015bf26bb5758d4a1ba61c12361da6467cfec4effb5ef`  
		Last Modified: Fri, 06 Mar 2020 02:53:34 GMT  
		Size: 161.2 KB (161207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c3818ef2400c0556c9559af6af5b4960882d6f2b86f9fd411b2cdc94a60cd6`  
		Last Modified: Wed, 25 Mar 2020 21:31:35 GMT  
		Size: 171.8 MB (171811514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
