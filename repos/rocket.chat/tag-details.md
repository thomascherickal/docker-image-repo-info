<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rocket.chat`

-	[`rocket.chat:2`](#rocketchat2)
-	[`rocket.chat:2.3`](#rocketchat23)
-	[`rocket.chat:2.3.1`](#rocketchat231)
-	[`rocket.chat:latest`](#rocketchatlatest)

## `rocket.chat:2`

```console
$ docker pull rocket.chat@sha256:1a6f80dd0e04308bfceb2ee91641afeb590a46162174a21594c77fa5349473b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:2c30604b3e8000f4eeb262fda0bf7891dada2b27aca6a33ccaaead8b6eb20f1f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.9 MB (198865792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f276876aed26304b881703550d82c82969cb01355f81323652d86fd620516a`
-	Default Command: `["node","main.js"]`

```dockerfile
# Fri, 22 Nov 2019 14:56:04 GMT
ADD file:41e78f98c436ed4f05c337e67e10439bb860bbea86c78368cc0e80100026cf40 in / 
# Fri, 22 Nov 2019 14:56:04 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:52:52 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD8F2338BAE7501E3DD5AC78C273792F7D83545D
# Sat, 23 Nov 2019 00:52:52 GMT
ENV NODE_VERSION=8.15.1
# Sat, 23 Nov 2019 00:52:53 GMT
ENV NODE_ENV=production
# Sat, 23 Nov 2019 00:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates curl; 	rm -rf /var/lib/apt/lists/*; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz"; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"; 	gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc; 	grep " node-v$NODE_VERSION-linux-x64.tar.gz\$" SHASUMS256.txt | sha256sum -c -; 	tar -xf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1 --no-same-owner; 	rm "node-v$NODE_VERSION-linux-x64.tar.gz" SHASUMS256.txt.asc SHASUMS256.txt; 	npm cache clear --force
# Sat, 23 Nov 2019 00:54:50 GMT
LABEL maintainer=buildmaster@rocket.chat
# Sat, 23 Nov 2019 00:54:51 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Sat, 23 Nov 2019 00:54:52 GMT
VOLUME [/app/uploads]
# Sat, 23 Nov 2019 00:54:53 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Sat, 23 Nov 2019 00:54:53 GMT
ENV RC_VERSION=2.2.0
# Sat, 23 Nov 2019 00:54:53 GMT
WORKDIR /app
# Sat, 23 Nov 2019 00:55:41 GMT
RUN curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxvf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Sat, 23 Nov 2019 00:55:44 GMT
USER rocketchat
# Sat, 23 Nov 2019 00:55:44 GMT
WORKDIR /app/bundle
# Sat, 23 Nov 2019 00:55:44 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Sat, 23 Nov 2019 00:55:44 GMT
EXPOSE 3000
# Sat, 23 Nov 2019 00:55:45 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:02d147d362835efa14b8a83e3b4a7dd20dd53dd0ba1619316a691acb9e614c13`  
		Last Modified: Fri, 22 Nov 2019 15:03:20 GMT  
		Size: 30.2 MB (30159468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3449a347fc04f19e863b2862c950110099dc301f5b603e215520c43f26c4478e`  
		Last Modified: Sat, 23 Nov 2019 00:55:52 GMT  
		Size: 9.8 KB (9809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8388be9515cf399345f74078db8b27ccfcecbff8c2db4e33af0f75c66a9ed327`  
		Last Modified: Sat, 23 Nov 2019 00:55:58 GMT  
		Size: 22.5 MB (22525849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbb47cca17d93b16277c8a4ef8f181e2696ba8e357297770b0131986495c3fe`  
		Last Modified: Sat, 23 Nov 2019 00:55:53 GMT  
		Size: 2.1 KB (2137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5d34e2fef7c484422271a79c600f81ec0ef7f9958ae7b1377a35b3d314af5e`  
		Last Modified: Sat, 23 Nov 2019 00:55:52 GMT  
		Size: 14.7 KB (14663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353b45922afddef7565e08296dc7d1e6fa7f4c8fa7141185a81598dd4aceaa1`  
		Last Modified: Sat, 23 Nov 2019 00:56:34 GMT  
		Size: 146.2 MB (146153866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:2.3`

```console
$ docker pull rocket.chat@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `rocket.chat:2.3.1`

```console
$ docker pull rocket.chat@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:1a6f80dd0e04308bfceb2ee91641afeb590a46162174a21594c77fa5349473b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:2c30604b3e8000f4eeb262fda0bf7891dada2b27aca6a33ccaaead8b6eb20f1f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.9 MB (198865792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87f276876aed26304b881703550d82c82969cb01355f81323652d86fd620516a`
-	Default Command: `["node","main.js"]`

```dockerfile
# Fri, 22 Nov 2019 14:56:04 GMT
ADD file:41e78f98c436ed4f05c337e67e10439bb860bbea86c78368cc0e80100026cf40 in / 
# Fri, 22 Nov 2019 14:56:04 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:52:52 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD8F2338BAE7501E3DD5AC78C273792F7D83545D
# Sat, 23 Nov 2019 00:52:52 GMT
ENV NODE_VERSION=8.15.1
# Sat, 23 Nov 2019 00:52:53 GMT
ENV NODE_ENV=production
# Sat, 23 Nov 2019 00:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates curl; 	rm -rf /var/lib/apt/lists/*; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz"; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"; 	gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc; 	grep " node-v$NODE_VERSION-linux-x64.tar.gz\$" SHASUMS256.txt | sha256sum -c -; 	tar -xf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1 --no-same-owner; 	rm "node-v$NODE_VERSION-linux-x64.tar.gz" SHASUMS256.txt.asc SHASUMS256.txt; 	npm cache clear --force
# Sat, 23 Nov 2019 00:54:50 GMT
LABEL maintainer=buildmaster@rocket.chat
# Sat, 23 Nov 2019 00:54:51 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Sat, 23 Nov 2019 00:54:52 GMT
VOLUME [/app/uploads]
# Sat, 23 Nov 2019 00:54:53 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Sat, 23 Nov 2019 00:54:53 GMT
ENV RC_VERSION=2.2.0
# Sat, 23 Nov 2019 00:54:53 GMT
WORKDIR /app
# Sat, 23 Nov 2019 00:55:41 GMT
RUN curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxvf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Sat, 23 Nov 2019 00:55:44 GMT
USER rocketchat
# Sat, 23 Nov 2019 00:55:44 GMT
WORKDIR /app/bundle
# Sat, 23 Nov 2019 00:55:44 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Sat, 23 Nov 2019 00:55:44 GMT
EXPOSE 3000
# Sat, 23 Nov 2019 00:55:45 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:02d147d362835efa14b8a83e3b4a7dd20dd53dd0ba1619316a691acb9e614c13`  
		Last Modified: Fri, 22 Nov 2019 15:03:20 GMT  
		Size: 30.2 MB (30159468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3449a347fc04f19e863b2862c950110099dc301f5b603e215520c43f26c4478e`  
		Last Modified: Sat, 23 Nov 2019 00:55:52 GMT  
		Size: 9.8 KB (9809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8388be9515cf399345f74078db8b27ccfcecbff8c2db4e33af0f75c66a9ed327`  
		Last Modified: Sat, 23 Nov 2019 00:55:58 GMT  
		Size: 22.5 MB (22525849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbb47cca17d93b16277c8a4ef8f181e2696ba8e357297770b0131986495c3fe`  
		Last Modified: Sat, 23 Nov 2019 00:55:53 GMT  
		Size: 2.1 KB (2137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5d34e2fef7c484422271a79c600f81ec0ef7f9958ae7b1377a35b3d314af5e`  
		Last Modified: Sat, 23 Nov 2019 00:55:52 GMT  
		Size: 14.7 KB (14663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353b45922afddef7565e08296dc7d1e6fa7f4c8fa7141185a81598dd4aceaa1`  
		Last Modified: Sat, 23 Nov 2019 00:56:34 GMT  
		Size: 146.2 MB (146153866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
