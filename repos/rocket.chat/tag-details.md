<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rocket.chat`

-	[`rocket.chat:6`](#rocketchat6)
-	[`rocket.chat:6.2`](#rocketchat62)
-	[`rocket.chat:6.2.12`](#rocketchat6212)
-	[`rocket.chat:6.3`](#rocketchat63)
-	[`rocket.chat:6.3.10`](#rocketchat6310)
-	[`rocket.chat:6.4`](#rocketchat64)
-	[`rocket.chat:6.4.2`](#rocketchat642)
-	[`rocket.chat:latest`](#rocketchatlatest)

## `rocket.chat:6`

```console
$ docker pull rocket.chat@sha256:9e593d35628636b5686d79400a22fc9f47e8969159356a61039833dab3580e91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:6` - linux; amd64

```console
$ docker pull rocket.chat@sha256:4f5f249f13ceb4d46d4330132d2091933d49b71aafa2b52934381e22d9000a3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (353004803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5d7997de8cfa63b4e721d12fae33fedf3094b0470608141db02854d77c72bf`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:14:33 GMT
ENV NODE_ENV=production
# Tue, 21 Nov 2023 20:14:33 GMT
ENV NODE_VERSION=14.21.3
# Tue, 21 Nov 2023 20:14:57 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 20:14:58 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 21 Nov 2023 20:14:58 GMT
VOLUME [/app/uploads]
# Tue, 21 Nov 2023 20:14:58 GMT
ENV RC_VERSION=6.4.2
# Tue, 21 Nov 2023 20:14:58 GMT
WORKDIR /app
# Tue, 21 Nov 2023 20:16:08 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Tue, 21 Nov 2023 20:16:13 GMT
USER rocketchat
# Tue, 21 Nov 2023 20:16:13 GMT
WORKDIR /app/bundle
# Tue, 21 Nov 2023 20:16:13 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 21 Nov 2023 20:16:13 GMT
EXPOSE 3000
# Tue, 21 Nov 2023 20:16:13 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527ff252bcd31a42a8eb4a25cafda21a89dff4fc92e1e4053944b5fbb7d42736`  
		Last Modified: Tue, 21 Nov 2023 20:20:26 GMT  
		Size: 35.8 MB (35762171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0839e00e325a0b1c7cb7408dd4cde6befae1575466cceadf323e013b309324c`  
		Last Modified: Tue, 21 Nov 2023 20:20:21 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a82115aa490bbb14cbcec79500ca261f4ce69a3fde84bb3158422a8e07597b`  
		Last Modified: Tue, 21 Nov 2023 20:21:11 GMT  
		Size: 285.8 MB (285822998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:6.2`

```console
$ docker pull rocket.chat@sha256:8a72a506e164761bbf6edecee1232ee2dc43f31a828087b9c9cb93a56ecadaf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:6.2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:ec199e133b30dfbf1f28c177511befe96f0ad3045f7311ae6330e527c8b0ef95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313325918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b3e2e08ca98cba85c098116928bbd46766f5b0475cc281a851ce3e3c954191`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 21 Nov 2023 05:22:20 GMT
ADD file:7672eb709be933bb0edec47b8141cd2ebff266a770dfae1278205f7cee43c71a in / 
# Tue, 21 Nov 2023 05:22:20 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:16:26 GMT
ENV NODE_ENV=production
# Tue, 21 Nov 2023 20:18:20 GMT
ENV NODE_VERSION=14.21.2
# Tue, 21 Nov 2023 20:18:44 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 20:18:45 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 21 Nov 2023 20:18:46 GMT
VOLUME [/app/uploads]
# Tue, 21 Nov 2023 20:18:46 GMT
ENV RC_VERSION=6.2.12
# Tue, 21 Nov 2023 20:18:46 GMT
WORKDIR /app
# Tue, 21 Nov 2023 20:19:58 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Tue, 21 Nov 2023 20:20:02 GMT
USER rocketchat
# Tue, 21 Nov 2023 20:20:02 GMT
WORKDIR /app/bundle
# Tue, 21 Nov 2023 20:20:02 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 21 Nov 2023 20:20:02 GMT
EXPOSE 3000
# Tue, 21 Nov 2023 20:20:03 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:0fc9206bc4affb32fe13185a20b8184271c753e9b7cb81484bf770054fc69737`  
		Last Modified: Tue, 21 Nov 2023 05:27:19 GMT  
		Size: 27.2 MB (27187457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc2f8415975b346c44580bd5169ea12b50a0945628e62dcc04e8b1ec14331a`  
		Last Modified: Tue, 21 Nov 2023 20:22:22 GMT  
		Size: 36.5 MB (36530733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a03b97a8a458dec6c46d61f13705f0be9e6e2783723195c15c023d9748dcb1`  
		Last Modified: Tue, 21 Nov 2023 20:22:16 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4e2e1e24702c4201510ee1b5833ff8f538b5e53bf6350fe3d48881a35f6ef6`  
		Last Modified: Tue, 21 Nov 2023 20:22:59 GMT  
		Size: 249.6 MB (249605922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:6.2.12`

```console
$ docker pull rocket.chat@sha256:8a72a506e164761bbf6edecee1232ee2dc43f31a828087b9c9cb93a56ecadaf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:6.2.12` - linux; amd64

```console
$ docker pull rocket.chat@sha256:ec199e133b30dfbf1f28c177511befe96f0ad3045f7311ae6330e527c8b0ef95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313325918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b3e2e08ca98cba85c098116928bbd46766f5b0475cc281a851ce3e3c954191`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 21 Nov 2023 05:22:20 GMT
ADD file:7672eb709be933bb0edec47b8141cd2ebff266a770dfae1278205f7cee43c71a in / 
# Tue, 21 Nov 2023 05:22:20 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:16:26 GMT
ENV NODE_ENV=production
# Tue, 21 Nov 2023 20:18:20 GMT
ENV NODE_VERSION=14.21.2
# Tue, 21 Nov 2023 20:18:44 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 20:18:45 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 21 Nov 2023 20:18:46 GMT
VOLUME [/app/uploads]
# Tue, 21 Nov 2023 20:18:46 GMT
ENV RC_VERSION=6.2.12
# Tue, 21 Nov 2023 20:18:46 GMT
WORKDIR /app
# Tue, 21 Nov 2023 20:19:58 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Tue, 21 Nov 2023 20:20:02 GMT
USER rocketchat
# Tue, 21 Nov 2023 20:20:02 GMT
WORKDIR /app/bundle
# Tue, 21 Nov 2023 20:20:02 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 21 Nov 2023 20:20:02 GMT
EXPOSE 3000
# Tue, 21 Nov 2023 20:20:03 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:0fc9206bc4affb32fe13185a20b8184271c753e9b7cb81484bf770054fc69737`  
		Last Modified: Tue, 21 Nov 2023 05:27:19 GMT  
		Size: 27.2 MB (27187457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cc2f8415975b346c44580bd5169ea12b50a0945628e62dcc04e8b1ec14331a`  
		Last Modified: Tue, 21 Nov 2023 20:22:22 GMT  
		Size: 36.5 MB (36530733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a03b97a8a458dec6c46d61f13705f0be9e6e2783723195c15c023d9748dcb1`  
		Last Modified: Tue, 21 Nov 2023 20:22:16 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4e2e1e24702c4201510ee1b5833ff8f538b5e53bf6350fe3d48881a35f6ef6`  
		Last Modified: Tue, 21 Nov 2023 20:22:59 GMT  
		Size: 249.6 MB (249605922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:6.3`

```console
$ docker pull rocket.chat@sha256:6da47633ecc666fb3061a3eed49815d4c5fdba9c90d5b22f14dedd8b8a7bf80e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:6.3` - linux; amd64

```console
$ docker pull rocket.chat@sha256:0320f084386b2df144817516ee98fda6e4a0f01faedb21305c00f164986fc897
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.2 MB (320240168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db3dc28ba52118a5babfe5b158fef79257caafc1025e4f653af4938c5c534fa5`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 21 Nov 2023 05:22:20 GMT
ADD file:7672eb709be933bb0edec47b8141cd2ebff266a770dfae1278205f7cee43c71a in / 
# Tue, 21 Nov 2023 05:22:20 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:16:26 GMT
ENV NODE_ENV=production
# Tue, 21 Nov 2023 20:16:26 GMT
ENV NODE_VERSION=14.21.3
# Tue, 21 Nov 2023 20:16:54 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 20:16:55 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 21 Nov 2023 20:16:55 GMT
VOLUME [/app/uploads]
# Tue, 21 Nov 2023 20:16:55 GMT
ENV RC_VERSION=6.3.10
# Tue, 21 Nov 2023 20:16:55 GMT
WORKDIR /app
# Tue, 21 Nov 2023 20:18:01 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Tue, 21 Nov 2023 20:18:05 GMT
USER rocketchat
# Tue, 21 Nov 2023 20:18:06 GMT
WORKDIR /app/bundle
# Tue, 21 Nov 2023 20:18:06 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 21 Nov 2023 20:18:06 GMT
EXPOSE 3000
# Tue, 21 Nov 2023 20:18:06 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:0fc9206bc4affb32fe13185a20b8184271c753e9b7cb81484bf770054fc69737`  
		Last Modified: Tue, 21 Nov 2023 05:27:19 GMT  
		Size: 27.2 MB (27187457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fff4c7ebc61836d428a876f3b5035b2d8c6d6a938d47cdd74c637b6e424ca1b`  
		Last Modified: Tue, 21 Nov 2023 20:21:28 GMT  
		Size: 35.7 MB (35734339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712a976873d0ff1c73201b4c6f7e914b7bd0b9a75c325adb0588e5962cd1788b`  
		Last Modified: Tue, 21 Nov 2023 20:21:23 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6dc6d7c29987386c9a9a1cc055e997a6b54a034e7afc59d880cdd0921a1b1e`  
		Last Modified: Tue, 21 Nov 2023 20:22:08 GMT  
		Size: 257.3 MB (257316566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:6.3.10`

```console
$ docker pull rocket.chat@sha256:6da47633ecc666fb3061a3eed49815d4c5fdba9c90d5b22f14dedd8b8a7bf80e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:6.3.10` - linux; amd64

```console
$ docker pull rocket.chat@sha256:0320f084386b2df144817516ee98fda6e4a0f01faedb21305c00f164986fc897
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.2 MB (320240168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db3dc28ba52118a5babfe5b158fef79257caafc1025e4f653af4938c5c534fa5`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 21 Nov 2023 05:22:20 GMT
ADD file:7672eb709be933bb0edec47b8141cd2ebff266a770dfae1278205f7cee43c71a in / 
# Tue, 21 Nov 2023 05:22:20 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:16:26 GMT
ENV NODE_ENV=production
# Tue, 21 Nov 2023 20:16:26 GMT
ENV NODE_VERSION=14.21.3
# Tue, 21 Nov 2023 20:16:54 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 20:16:55 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 21 Nov 2023 20:16:55 GMT
VOLUME [/app/uploads]
# Tue, 21 Nov 2023 20:16:55 GMT
ENV RC_VERSION=6.3.10
# Tue, 21 Nov 2023 20:16:55 GMT
WORKDIR /app
# Tue, 21 Nov 2023 20:18:01 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Tue, 21 Nov 2023 20:18:05 GMT
USER rocketchat
# Tue, 21 Nov 2023 20:18:06 GMT
WORKDIR /app/bundle
# Tue, 21 Nov 2023 20:18:06 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 21 Nov 2023 20:18:06 GMT
EXPOSE 3000
# Tue, 21 Nov 2023 20:18:06 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:0fc9206bc4affb32fe13185a20b8184271c753e9b7cb81484bf770054fc69737`  
		Last Modified: Tue, 21 Nov 2023 05:27:19 GMT  
		Size: 27.2 MB (27187457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fff4c7ebc61836d428a876f3b5035b2d8c6d6a938d47cdd74c637b6e424ca1b`  
		Last Modified: Tue, 21 Nov 2023 20:21:28 GMT  
		Size: 35.7 MB (35734339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712a976873d0ff1c73201b4c6f7e914b7bd0b9a75c325adb0588e5962cd1788b`  
		Last Modified: Tue, 21 Nov 2023 20:21:23 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6dc6d7c29987386c9a9a1cc055e997a6b54a034e7afc59d880cdd0921a1b1e`  
		Last Modified: Tue, 21 Nov 2023 20:22:08 GMT  
		Size: 257.3 MB (257316566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:6.4`

```console
$ docker pull rocket.chat@sha256:9e593d35628636b5686d79400a22fc9f47e8969159356a61039833dab3580e91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:6.4` - linux; amd64

```console
$ docker pull rocket.chat@sha256:4f5f249f13ceb4d46d4330132d2091933d49b71aafa2b52934381e22d9000a3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (353004803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5d7997de8cfa63b4e721d12fae33fedf3094b0470608141db02854d77c72bf`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:14:33 GMT
ENV NODE_ENV=production
# Tue, 21 Nov 2023 20:14:33 GMT
ENV NODE_VERSION=14.21.3
# Tue, 21 Nov 2023 20:14:57 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 20:14:58 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 21 Nov 2023 20:14:58 GMT
VOLUME [/app/uploads]
# Tue, 21 Nov 2023 20:14:58 GMT
ENV RC_VERSION=6.4.2
# Tue, 21 Nov 2023 20:14:58 GMT
WORKDIR /app
# Tue, 21 Nov 2023 20:16:08 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Tue, 21 Nov 2023 20:16:13 GMT
USER rocketchat
# Tue, 21 Nov 2023 20:16:13 GMT
WORKDIR /app/bundle
# Tue, 21 Nov 2023 20:16:13 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 21 Nov 2023 20:16:13 GMT
EXPOSE 3000
# Tue, 21 Nov 2023 20:16:13 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527ff252bcd31a42a8eb4a25cafda21a89dff4fc92e1e4053944b5fbb7d42736`  
		Last Modified: Tue, 21 Nov 2023 20:20:26 GMT  
		Size: 35.8 MB (35762171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0839e00e325a0b1c7cb7408dd4cde6befae1575466cceadf323e013b309324c`  
		Last Modified: Tue, 21 Nov 2023 20:20:21 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a82115aa490bbb14cbcec79500ca261f4ce69a3fde84bb3158422a8e07597b`  
		Last Modified: Tue, 21 Nov 2023 20:21:11 GMT  
		Size: 285.8 MB (285822998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:6.4.2`

```console
$ docker pull rocket.chat@sha256:9e593d35628636b5686d79400a22fc9f47e8969159356a61039833dab3580e91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:6.4.2` - linux; amd64

```console
$ docker pull rocket.chat@sha256:4f5f249f13ceb4d46d4330132d2091933d49b71aafa2b52934381e22d9000a3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (353004803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5d7997de8cfa63b4e721d12fae33fedf3094b0470608141db02854d77c72bf`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:14:33 GMT
ENV NODE_ENV=production
# Tue, 21 Nov 2023 20:14:33 GMT
ENV NODE_VERSION=14.21.3
# Tue, 21 Nov 2023 20:14:57 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 20:14:58 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 21 Nov 2023 20:14:58 GMT
VOLUME [/app/uploads]
# Tue, 21 Nov 2023 20:14:58 GMT
ENV RC_VERSION=6.4.2
# Tue, 21 Nov 2023 20:14:58 GMT
WORKDIR /app
# Tue, 21 Nov 2023 20:16:08 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Tue, 21 Nov 2023 20:16:13 GMT
USER rocketchat
# Tue, 21 Nov 2023 20:16:13 GMT
WORKDIR /app/bundle
# Tue, 21 Nov 2023 20:16:13 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 21 Nov 2023 20:16:13 GMT
EXPOSE 3000
# Tue, 21 Nov 2023 20:16:13 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527ff252bcd31a42a8eb4a25cafda21a89dff4fc92e1e4053944b5fbb7d42736`  
		Last Modified: Tue, 21 Nov 2023 20:20:26 GMT  
		Size: 35.8 MB (35762171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0839e00e325a0b1c7cb7408dd4cde6befae1575466cceadf323e013b309324c`  
		Last Modified: Tue, 21 Nov 2023 20:20:21 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a82115aa490bbb14cbcec79500ca261f4ce69a3fde84bb3158422a8e07597b`  
		Last Modified: Tue, 21 Nov 2023 20:21:11 GMT  
		Size: 285.8 MB (285822998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rocket.chat:latest`

```console
$ docker pull rocket.chat@sha256:9e593d35628636b5686d79400a22fc9f47e8969159356a61039833dab3580e91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rocket.chat:latest` - linux; amd64

```console
$ docker pull rocket.chat@sha256:4f5f249f13ceb4d46d4330132d2091933d49b71aafa2b52934381e22d9000a3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.0 MB (353004803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5d7997de8cfa63b4e721d12fae33fedf3094b0470608141db02854d77c72bf`
-	Default Command: `["node","main.js"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:14:33 GMT
ENV NODE_ENV=production
# Tue, 21 Nov 2023 20:14:33 GMT
ENV NODE_VERSION=14.21.3
# Tue, 21 Nov 2023 20:14:57 GMT
RUN ARCH="x64"   && set -eux   && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl wget gnupg dirmngr xz-utils   && rm -rf /var/lib/apt/lists/*   && for key in   4ED778F539E3634C779C87C6D7062848A1AB005C   94AE36675C464D64BAFA68DD7434390BDBE9B9C5   74F12602B6F1C4E913FAA37AD3A89613643B6201   71DCFD284A79C3B38668286BC97EC7A07EDE3FC1   8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600   C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8   C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C   DD8F2338BAE7501E3DD5AC78C273792F7D83545D   A48C2BEE680E841632CD4E44F07496B3EB3C1762   108F52B48DB57BB0CC439B2997B01419BD92F80A   B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do   gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||   gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && apt-mark auto '.*' > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 21 Nov 2023 20:14:58 GMT
RUN groupadd -r rocketchat   && useradd -r -g rocketchat rocketchat   && mkdir -p /app/uploads   && chown rocketchat:rocketchat /app/uploads
# Tue, 21 Nov 2023 20:14:58 GMT
VOLUME [/app/uploads]
# Tue, 21 Nov 2023 20:14:58 GMT
ENV RC_VERSION=6.4.2
# Tue, 21 Nov 2023 20:14:58 GMT
WORKDIR /app
# Tue, 21 Nov 2023 20:16:08 GMT
RUN set -eux   && apt-get update   && apt-get install -y --no-install-recommends fontconfig   && aptMark="$(apt-mark showmanual)"   && apt-get install -y --no-install-recommends g++ make python ca-certificates curl gnupg   && rm -rf /var/lib/apt/lists/*   && gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 0E163286C20D07B9787EBE9FD7F9D0414FD08104   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/download" -o rocket.chat.tgz   && curl -fSL "https://releases.rocket.chat/${RC_VERSION}/asc" -o rocket.chat.tgz.asc   && gpg --batch --verify rocket.chat.tgz.asc rocket.chat.tgz   && tar zxf rocket.chat.tgz   && rm rocket.chat.tgz rocket.chat.tgz.asc   && cd bundle/programs/server   && npm install   && apt-mark auto '.*' > /dev/null   && apt-mark manual $aptMark > /dev/null   && find /usr/local -type f -executable -exec ldd '{}' ';'   | awk '/=>/ { print $(NF-1) }'   | sort -u   | xargs -r dpkg-query --search   | cut -d: -f1   | sort -u   | xargs -r apt-mark manual   && apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false   && npm cache clear --force   && chown -R rocketchat:rocketchat /app
# Tue, 21 Nov 2023 20:16:13 GMT
USER rocketchat
# Tue, 21 Nov 2023 20:16:13 GMT
WORKDIR /app/bundle
# Tue, 21 Nov 2023 20:16:13 GMT
ENV DEPLOY_METHOD=docker-official MONGO_URL=mongodb://db:27017/meteor HOME=/tmp PORT=3000 ROOT_URL=http://localhost:3000 Accounts_AvatarStorePath=/app/uploads
# Tue, 21 Nov 2023 20:16:13 GMT
EXPOSE 3000
# Tue, 21 Nov 2023 20:16:13 GMT
CMD ["node" "main.js"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527ff252bcd31a42a8eb4a25cafda21a89dff4fc92e1e4053944b5fbb7d42736`  
		Last Modified: Tue, 21 Nov 2023 20:20:26 GMT  
		Size: 35.8 MB (35762171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0839e00e325a0b1c7cb7408dd4cde6befae1575466cceadf323e013b309324c`  
		Last Modified: Tue, 21 Nov 2023 20:20:21 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a82115aa490bbb14cbcec79500ca261f4ce69a3fde84bb3158422a8e07597b`  
		Last Modified: Tue, 21 Nov 2023 20:21:11 GMT  
		Size: 285.8 MB (285822998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
