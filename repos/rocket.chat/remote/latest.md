## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:de45eb74febf1dea63180f528f3274e734767e3a6c888387f3a2c72f54578330
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:f673490ca9b5da594d94d1d9bf8ae486331d51d80fa12d7013798cb53e994d89
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226179048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a31c3dd8891072d8b177b0896f2440a27ee16b9eb8aaaed861ac6a08202a873b`
-	Default Command: `["node","main.js"]`

```dockerfile
# Thu, 16 Apr 2020 03:23:30 GMT
ADD file:4dc0e977ce6a3fd7ac215d6eea152bdf77f76fd2bfd390a5ef6889385b3d00ab in / 
# Thu, 16 Apr 2020 03:23:30 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 21:02:15 GMT
ENV NODE_ENV=production
# Thu, 16 Apr 2020 21:02:15 GMT
ENV NODE_VERSION=12.14.0
# Thu, 16 Apr 2020 21:04:54 GMT
RUN ARCH="x64"     && set -eux     && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils     && rm -rf /var/lib/apt/lists/*     && for key in       94AE36675C464D64BAFA68DD7434390BDBE9B9C5       FD3A5288F042B6850C66B31F09FE44734EB7990E       71DCFD284A79C3B38668286BC97EC7A07EDE3FC1       DD8F2338BAE7501E3DD5AC78C273792F7D83545D       C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8       B9AE9905FFD7803F25714661B63B535A4C206CA9       77984A986EBC2AA786BC0F66B01FBB92821C587A       8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600       4ED778F539E3634C779C87C6D7062848A1AB005C       A48C2BEE680E841632CD4E44F07496B3EB3C1762       B9E2F5981AA6E0CD28160D9FF13993A75599653C     ; do       gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||       gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||       gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;     done     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"     && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"     && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc     && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -     && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner     && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt     && apt-mark auto '.*' > /dev/null     && find /usr/local -type f -executable -exec ldd '{}' ';'       | awk '/=>/ { print $(NF-1) }'       | sort -u       | xargs -r dpkg-query --search       | cut -d: -f1       | sort -u       | xargs -r apt-mark manual     && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Apr 2020 21:04:55 GMT
RUN groupadd -r rocketchat &&  useradd -r -g rocketchat rocketchat &&  mkdir -p /app/uploads &&  chown rocketchat:rocketchat /app/uploads
# Thu, 16 Apr 2020 21:04:55 GMT
VOLUME [/app/uploads]
# Thu, 16 Apr 2020 21:04:56 GMT
RUN gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104
# Thu, 16 Apr 2020 21:04:56 GMT
ENV RC_VERSION=3.0.12
# Thu, 16 Apr 2020 21:04:56 GMT
WORKDIR /app
# Thu, 16 Apr 2020 21:09:40 GMT
RUN apt-get update &&  apt-get install -y --no-install-recommends fontconfig &&  aptMark="$(apt-mark showmanual)" &&  apt-get install -y --no-install-recommends g++ make python ca-certificates curl &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz &&  curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc &&  gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz &&  tar zxf rocket.chat.tgz &&  rm rocket.chat.tgz rocket.chat.tgz.asc &&  cd bundle/programs/server &&  npm install &&  apt-mark auto '.*' > /dev/null &&  apt-mark manual $aptMark > /dev/null &&  find /usr/local -type f -executable -exec ldd '{}' ';'     | awk '/=>/ { print $(NF-1) }'     | sort -u     | xargs -r dpkg-query --search     | cut -d: -f1     | sort -u     | xargs -r apt-mark manual &&  apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false &&  npm cache clear --force &&  chown -R rocketchat:rocketchat /app
# Thu, 16 Apr 2020 21:09:43 GMT
USER rocketchat
# Thu, 16 Apr 2020 21:09:43 GMT
WORKDIR /app/bundle
# Thu, 16 Apr 2020 21:09:43 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Thu, 16 Apr 2020 21:09:43 GMT
EXPOSE 3000
# Thu, 16 Apr 2020 21:09:43 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:007f6a8f62408642e3ff1d624b788470ce5a58b805c24ee4e1be641919d64751`  
		Last Modified: Thu, 16 Apr 2020 03:32:23 GMT  
		Size: 30.2 MB (30159502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39a8867c89b1479034967f092f677feda07051946cb743c98d5be0bf345f54e`  
		Last Modified: Thu, 16 Apr 2020 21:17:49 GMT  
		Size: 24.0 MB (23991683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3da6e05e32437845324911c0e6914418df7d55383d0bf8ca9378c50a841b00`  
		Last Modified: Thu, 16 Apr 2020 21:17:36 GMT  
		Size: 2.1 KB (2138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05a891960cb3a21be1e03d4f53751712d8170178e5382475f874ada993e6aaf`  
		Last Modified: Thu, 16 Apr 2020 21:17:36 GMT  
		Size: 171.3 KB (171282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936c437b5f5a90fefeebf0b1a1779c459430f2c261f0038ce56d9329413f02cf`  
		Last Modified: Thu, 16 Apr 2020 21:19:05 GMT  
		Size: 171.9 MB (171854443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
