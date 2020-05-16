## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:b0af916c430f50ffe9a80718b0d603983dd316a027c94191411c1b94c0db2a6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:0262c9e7b216df9175883ba4a5b2a88332dcd35599985f23c63e91d303a6a994
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (233967250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf7d835b6d8db6f5ad0cc114f3246b6a6a5e25bdff9f00e4faa1ef5643e9e8bd`
-	Default Command: `["node","main.js"]`

```dockerfile
# Fri, 15 May 2020 06:29:39 GMT
ADD file:faa01786a6e5d5cc8855c0af88b1d49ddee288ddd39f479eff4da038a8e88065 in / 
# Fri, 15 May 2020 06:29:39 GMT
CMD ["bash"]
# Sat, 16 May 2020 02:21:11 GMT
ENV NODE_ENV=production
# Sat, 16 May 2020 02:21:11 GMT
ENV NODE_VERSION=12.16.1
# Sat, 16 May 2020 02:24:08 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 16 May 2020 02:24:10 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Sat, 16 May 2020 02:24:10 GMT
VOLUME [/app/uploads]
# Sat, 16 May 2020 02:24:12 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Sat, 16 May 2020 02:24:12 GMT
ENV RC_VERSION=3.2.2
# Sat, 16 May 2020 02:24:12 GMT
WORKDIR /app
# Sat, 16 May 2020 02:29:20 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Sat, 16 May 2020 02:29:22 GMT
USER rocketchat
# Sat, 16 May 2020 02:29:22 GMT
WORKDIR /app/bundle
# Sat, 16 May 2020 02:29:22 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Sat, 16 May 2020 02:29:22 GMT
EXPOSE 3000
# Sat, 16 May 2020 02:29:23 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:a4834f3e07e2bd6b73cd4027a9549e06e42312f401d6307015085f7c0c2f112d`  
		Last Modified: Fri, 15 May 2020 06:38:13 GMT  
		Size: 30.2 MB (30159415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7f1235f6efb40e71a57ca92c9ae7423d984f61c394b8a40841c02b5f033510`  
		Last Modified: Sat, 16 May 2020 02:38:33 GMT  
		Size: 24.2 MB (24202075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525b1657f946cbf27e800c231adf8dc85d59d9482f3786cf62d9ae435388fb16`  
		Last Modified: Sat, 16 May 2020 02:38:23 GMT  
		Size: 2.1 KB (2136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267634010c4e7ced8caed242d1e6f9e36cc01744caec0ba88561142851adcad`  
		Last Modified: Sat, 16 May 2020 02:38:23 GMT  
		Size: 171.3 KB (171283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f34b0e6adf96dbbf26881fe3c76a4607e7ead342121a4765ecccf9b92730520`  
		Last Modified: Sat, 16 May 2020 02:39:17 GMT  
		Size: 179.4 MB (179432341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
