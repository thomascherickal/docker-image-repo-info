<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rocket.chat`

-	[`rocket.chat:2`](#rocketchat2)
-	[`rocket.chat:2.4`](#rocketchat24)
-	[`rocket.chat:2.4.1`](#rocketchat241)
-	[`rocket.chat:latest`](#rocketchatlatest)

## `rocket.chat:2`

```console
$ docker pull rocket.chat@sha256:61743e6d22856fa823c516f75e42a5ad7cad78a2d1189f37d0fadf4703f17f28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:580fbe2431a27f85bcd2d32a5c3777d05d0fb72d3a3f84d299953b037e28f51f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.7 MB (201669637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5aac25b6daa4cb5ea54de2c1d4c76275331d0eece4aadc7d4908ca0e2e873ba`
-	Default Command: `["node","main.js"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:46 GMT
ADD file:bfa07c80ea2ec0396e781ef354835dbb10845a99934a7c7a226c2098b3641b6b in / 
# Sat, 28 Dec 2019 04:21:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:21 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD8F2338BAE7501E3DD5AC78C273792F7D83545D
# Sat, 28 Dec 2019 15:25:21 GMT
ENV NODE_VERSION=8.15.1
# Sat, 28 Dec 2019 15:25:22 GMT
ENV NODE_ENV=production
# Sat, 28 Dec 2019 15:27:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates curl fontconfig; 	rm -rf /var/lib/apt/lists/*; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz"; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"; 	gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc; 	grep " node-v$NODE_VERSION-linux-x64.tar.gz\$" SHASUMS256.txt | sha256sum -c -; 	tar -xf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1 --no-same-owner; 	rm "node-v$NODE_VERSION-linux-x64.tar.gz" SHASUMS256.txt.asc SHASUMS256.txt; 	npm cache clear --force
# Sat, 28 Dec 2019 15:27:18 GMT
LABEL maintainer=buildmaster@rocket.chat
# Sat, 28 Dec 2019 15:27:20 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Sat, 28 Dec 2019 15:27:20 GMT
VOLUME [/app/uploads]
# Sat, 28 Dec 2019 15:27:21 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Sat, 28 Dec 2019 15:27:21 GMT
ENV RC_VERSION=2.3.1
# Sat, 28 Dec 2019 15:27:22 GMT
WORKDIR /app
# Sat, 28 Dec 2019 15:28:06 GMT
RUN curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxvf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Sat, 28 Dec 2019 15:28:09 GMT
USER rocketchat
# Sat, 28 Dec 2019 15:28:10 GMT
WORKDIR /app/bundle
# Sat, 28 Dec 2019 15:28:11 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Sat, 28 Dec 2019 15:28:12 GMT
EXPOSE 3000
# Sat, 28 Dec 2019 15:28:13 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f79bccfe408cf63380358b522e6727a24da2086df8fc7dc7db005ccff874370d`  
		Last Modified: Sat, 28 Dec 2019 04:26:18 GMT  
		Size: 30.2 MB (30159553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a3ed552c0d7a392c822f04678d23d8ef21eee5cff271fe50764abd597f2a13`  
		Last Modified: Sat, 28 Dec 2019 15:28:23 GMT  
		Size: 9.8 KB (9808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2536ca95dc07ee04d690c1ead78dfa434b8f47d4207ba27fc9ce4595c0d2506d`  
		Last Modified: Sat, 28 Dec 2019 15:28:29 GMT  
		Size: 24.9 MB (24911246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b937c32ce70fd130a9ce7e4c273fbf4c08ade35cfcd2afa9aa264e4c2dcd72`  
		Last Modified: Sat, 28 Dec 2019 15:28:23 GMT  
		Size: 2.1 KB (2132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd9f7d7b1566178fff0ca9c64b4dd3f70ea050f0adcfc01a51e8fe144c2527b`  
		Last Modified: Sat, 28 Dec 2019 15:28:23 GMT  
		Size: 14.7 KB (14666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b50b2b22d86bc1e6e165c6afae1dcca861b70e885b6fef6a9981062062937e`  
		Last Modified: Sat, 28 Dec 2019 15:28:58 GMT  
		Size: 146.6 MB (146572232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.4`

**does not exist** (yet?)

## `rocket.chat:2.4.1`

**does not exist** (yet?)

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:61743e6d22856fa823c516f75e42a5ad7cad78a2d1189f37d0fadf4703f17f28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:580fbe2431a27f85bcd2d32a5c3777d05d0fb72d3a3f84d299953b037e28f51f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.7 MB (201669637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5aac25b6daa4cb5ea54de2c1d4c76275331d0eece4aadc7d4908ca0e2e873ba`
-	Default Command: `["node","main.js"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:46 GMT
ADD file:bfa07c80ea2ec0396e781ef354835dbb10845a99934a7c7a226c2098b3641b6b in / 
# Sat, 28 Dec 2019 04:21:47 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:25:21 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD8F2338BAE7501E3DD5AC78C273792F7D83545D
# Sat, 28 Dec 2019 15:25:21 GMT
ENV NODE_VERSION=8.15.1
# Sat, 28 Dec 2019 15:25:22 GMT
ENV NODE_ENV=production
# Sat, 28 Dec 2019 15:27:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates curl fontconfig; 	rm -rf /var/lib/apt/lists/*; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz"; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"; 	gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc; 	grep " node-v$NODE_VERSION-linux-x64.tar.gz\$" SHASUMS256.txt | sha256sum -c -; 	tar -xf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1 --no-same-owner; 	rm "node-v$NODE_VERSION-linux-x64.tar.gz" SHASUMS256.txt.asc SHASUMS256.txt; 	npm cache clear --force
# Sat, 28 Dec 2019 15:27:18 GMT
LABEL maintainer=buildmaster@rocket.chat
# Sat, 28 Dec 2019 15:27:20 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Sat, 28 Dec 2019 15:27:20 GMT
VOLUME [/app/uploads]
# Sat, 28 Dec 2019 15:27:21 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Sat, 28 Dec 2019 15:27:21 GMT
ENV RC_VERSION=2.3.1
# Sat, 28 Dec 2019 15:27:22 GMT
WORKDIR /app
# Sat, 28 Dec 2019 15:28:06 GMT
RUN curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxvf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Sat, 28 Dec 2019 15:28:09 GMT
USER rocketchat
# Sat, 28 Dec 2019 15:28:10 GMT
WORKDIR /app/bundle
# Sat, 28 Dec 2019 15:28:11 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Sat, 28 Dec 2019 15:28:12 GMT
EXPOSE 3000
# Sat, 28 Dec 2019 15:28:13 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:f79bccfe408cf63380358b522e6727a24da2086df8fc7dc7db005ccff874370d`  
		Last Modified: Sat, 28 Dec 2019 04:26:18 GMT  
		Size: 30.2 MB (30159553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a3ed552c0d7a392c822f04678d23d8ef21eee5cff271fe50764abd597f2a13`  
		Last Modified: Sat, 28 Dec 2019 15:28:23 GMT  
		Size: 9.8 KB (9808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2536ca95dc07ee04d690c1ead78dfa434b8f47d4207ba27fc9ce4595c0d2506d`  
		Last Modified: Sat, 28 Dec 2019 15:28:29 GMT  
		Size: 24.9 MB (24911246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b937c32ce70fd130a9ce7e4c273fbf4c08ade35cfcd2afa9aa264e4c2dcd72`  
		Last Modified: Sat, 28 Dec 2019 15:28:23 GMT  
		Size: 2.1 KB (2132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd9f7d7b1566178fff0ca9c64b4dd3f70ea050f0adcfc01a51e8fe144c2527b`  
		Last Modified: Sat, 28 Dec 2019 15:28:23 GMT  
		Size: 14.7 KB (14666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b50b2b22d86bc1e6e165c6afae1dcca861b70e885b6fef6a9981062062937e`  
		Last Modified: Sat, 28 Dec 2019 15:28:58 GMT  
		Size: 146.6 MB (146572232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
