## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:4caf65a9085c56be4fb5f0f83623839a51c097401251319f33a24dde85eaf736
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:5231f3622ae24c2d0ff0977ed09eae0bcf3a9a3d6337be0023fab8373cf5ff72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.7 MB (221662692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b89ff0452ce555a4ab23ae6cf287a57c401b10e2da2228d510a6699badfd1d0`
-	Default Command: `["node","main.js"]`

```dockerfile
# Sat, 01 Feb 2020 17:21:22 GMT
ADD file:7bddae780bfc4ce751148aec0e77e665e08c4c031b4e054a9f6b0e9920498285 in / 
# Sat, 01 Feb 2020 17:21:22 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:25:51 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD8F2338BAE7501E3DD5AC78C273792F7D83545D
# Sat, 01 Feb 2020 18:25:51 GMT
ENV NODE_VERSION=8.15.1
# Sat, 01 Feb 2020 18:25:51 GMT
ENV NODE_ENV=production
# Sat, 01 Feb 2020 18:27:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates curl fontconfig; 	rm -rf /var/lib/apt/lists/*; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-x64.tar.gz"; 	curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"; 	gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc; 	grep " node-v$NODE_VERSION-linux-x64.tar.gz\$" SHASUMS256.txt | sha256sum -c -; 	tar -xf "node-v$NODE_VERSION-linux-x64.tar.gz" -C /usr/local --strip-components=1 --no-same-owner; 	rm "node-v$NODE_VERSION-linux-x64.tar.gz" SHASUMS256.txt.asc SHASUMS256.txt; 	npm cache clear --force
# Sat, 01 Feb 2020 18:27:54 GMT
LABEL maintainer=buildmaster@rocket.chat
# Sat, 01 Feb 2020 18:27:55 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Sat, 01 Feb 2020 18:27:55 GMT
VOLUME [/app/uploads]
# Sat, 01 Feb 2020 18:27:56 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Sat, 01 Feb 2020 18:27:56 GMT
ENV RC_VERSION=2.4.1
# Sat, 01 Feb 2020 18:27:57 GMT
WORKDIR /app
# Sat, 01 Feb 2020 18:28:41 GMT
RUN curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxvf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Sat, 01 Feb 2020 18:28:43 GMT
USER rocketchat
# Sat, 01 Feb 2020 18:28:43 GMT
WORKDIR /app/bundle
# Sat, 01 Feb 2020 18:28:43 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Sat, 01 Feb 2020 18:28:44 GMT
EXPOSE 3000
# Sat, 01 Feb 2020 18:28:44 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:6f2295d35e78f75bc28bbc7b81c7a49bcc54eea446127fc14035418dd3d32456`  
		Last Modified: Sat, 01 Feb 2020 17:26:47 GMT  
		Size: 30.2 MB (30159539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5053cb7c47df274918e4c1cb227e960fa5b5891637fb8caa1bbaffe6b769c8c`  
		Last Modified: Sat, 01 Feb 2020 18:28:54 GMT  
		Size: 9.8 KB (9809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51cfe675c443897ee6035283166b3a9e5104013eeea8e34440e9addf6bc6fc8`  
		Last Modified: Sat, 01 Feb 2020 18:29:01 GMT  
		Size: 24.9 MB (24911387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce87d3499fb2fc8545b8a6e66434b6069300dd7abaf78ce02521b99243ce86e`  
		Last Modified: Sat, 01 Feb 2020 18:28:54 GMT  
		Size: 2.1 KB (2133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9d44c6e8640c8bb9e449fab0a6438395fe942d39d24a6b64032a3a241fadc5`  
		Last Modified: Sat, 01 Feb 2020 18:28:54 GMT  
		Size: 15.2 KB (15219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7d72549acafdf399039f29300f9eadb5e4c05677f167ba8413feca3b40cea3`  
		Last Modified: Sat, 01 Feb 2020 18:29:39 GMT  
		Size: 166.6 MB (166564605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
