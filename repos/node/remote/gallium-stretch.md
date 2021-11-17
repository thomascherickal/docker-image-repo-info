## `node:gallium-stretch`

```console
$ docker pull node@sha256:b9131d5a3bea3459ddda8a145a07d7aeff4ef4b204b4cd5224c024a1a9c7bfb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `node:gallium-stretch` - linux; amd64

```console
$ docker pull node@sha256:547162e078af6b106bd425e2cf19473269bdb4c8ff8366f4f2df0fa994e30672
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.0 MB (360962385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4dcf774ee722702aa99e236c1cbe938411f3881a4950602fd952cb892b5527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:48:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:48:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 15:49:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:50:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 05:45:14 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 27 Oct 2021 18:23:52 GMT
ENV NODE_VERSION=16.13.0
# Wed, 27 Oct 2021 18:24:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 27 Oct 2021 18:24:28 GMT
ENV YARN_VERSION=1.22.15
# Wed, 27 Oct 2021 18:24:34 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 27 Oct 2021 18:24:34 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 27 Oct 2021 18:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Oct 2021 18:24:35 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a43d3c11106306de19fd422e9da4a6f9b96de147d92c6213d6dbbc395be81b3`  
		Last Modified: Tue, 12 Oct 2021 15:57:10 GMT  
		Size: 11.3 MB (11301072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243ae34810fbd860a43ecf1a7da887386e7a1155913bf13ed95681c98a1cfa84`  
		Last Modified: Tue, 12 Oct 2021 15:57:08 GMT  
		Size: 4.3 MB (4342414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01c447bcebcc60440b9d84f429ded8ce8d836952f1061c96cce5047230ab696`  
		Last Modified: Tue, 12 Oct 2021 15:57:31 GMT  
		Size: 49.8 MB (49762475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d07840244ef02090cd7f447e6ab7b021a238b24864e9513e7a37d2891f4fb57`  
		Last Modified: Tue, 12 Oct 2021 15:58:09 GMT  
		Size: 214.4 MB (214435253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df57a36055e9d7d2081a5c4e9310b473498a97c69eba1d2c71778a86f92db0b`  
		Last Modified: Wed, 13 Oct 2021 06:05:15 GMT  
		Size: 4.2 KB (4189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25661a6fefbbebf6d5649a360c36ef919f78d09e91ee630c6e8068b6018b6fa2`  
		Last Modified: Wed, 27 Oct 2021 18:34:41 GMT  
		Size: 33.4 MB (33421470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030f50cd5d9905379645431c86e7933d6c913e943473d56a6bcbcf993c387659`  
		Last Modified: Wed, 27 Oct 2021 18:34:37 GMT  
		Size: 2.3 MB (2315396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cab36d35bc3dd2f31de65b1299367a26916ea468d26b7b4f17b33364cfc8133`  
		Last Modified: Wed, 27 Oct 2021 18:34:36 GMT  
		Size: 465.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:gallium-stretch` - linux; arm variant v7

```console
$ docker pull node@sha256:d76038a74eafc6cd72ad322fa6f8812ff6e0f50d13b66c0199fe732b67345174
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.2 MB (330219037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b8b4b5e2b4230e0ad55897538119d81a21bb1039bec54659c3bac1b437189a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Wed, 17 Nov 2021 02:04:57 GMT
ADD file:61da3fcef3aea99b4927189cfcb823a65b0e911a3f4436e44ea84a57a7919ff3 in / 
# Wed, 17 Nov 2021 02:04:58 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:54:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:54:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:57:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:34 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 17 Nov 2021 08:39:30 GMT
ENV NODE_VERSION=16.13.0
# Wed, 17 Nov 2021 08:39:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 17 Nov 2021 08:39:57 GMT
ENV YARN_VERSION=1.22.15
# Wed, 17 Nov 2021 08:40:05 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 17 Nov 2021 08:40:06 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 17 Nov 2021 08:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 08:40:07 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:e4d54b576c2fcdd259e57bac14c4e1a2623f6e5dc9a0b1facaed7fe59d891e86`  
		Last Modified: Wed, 17 Nov 2021 02:22:03 GMT  
		Size: 42.1 MB (42116868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04dd2447fcded30a4c9a8d7a054ccb2e4c4db4118989ea05bf2e56d60a8924`  
		Last Modified: Wed, 17 Nov 2021 03:14:24 GMT  
		Size: 10.0 MB (9956153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b37c8e78d6ca4f8e5467e0ec7ef61eef6101e99c8154472df98aa34159f5974`  
		Last Modified: Wed, 17 Nov 2021 03:14:21 GMT  
		Size: 3.9 MB (3921214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fcf28009119cc468ce87b98d583e8c51d3703937d10d502a704f1032bc2b26`  
		Last Modified: Wed, 17 Nov 2021 03:15:08 GMT  
		Size: 46.1 MB (46126162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b8b79b0de7febe2c3b866e2f14fe48bca033ef5ee3eda5193c147f47eb3f55`  
		Last Modified: Wed, 17 Nov 2021 03:17:08 GMT  
		Size: 195.1 MB (195052532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c44865c2fdc6b15a8201de29a28ec484a7143eb2ad3bc060758c9ed0e5b25cb`  
		Last Modified: Wed, 17 Nov 2021 09:19:09 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32749371b5c919239f8e60a831cccad2d1d118dca134a91b8425c8a3d410ca9e`  
		Last Modified: Wed, 17 Nov 2021 09:25:35 GMT  
		Size: 30.7 MB (30736570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c557f12fd5e60cf7dd067fc60f8cce9086c4f0438cc1e1bfc883d1e48a810d84`  
		Last Modified: Wed, 17 Nov 2021 09:25:15 GMT  
		Size: 2.3 MB (2304897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8445f76d8a7fdaf8879c221cead42a8b5030f5dbae20941d3f6abfb6b64afec7`  
		Last Modified: Wed, 17 Nov 2021 09:25:14 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:gallium-stretch` - linux; arm64 variant v8

```console
$ docker pull node@sha256:b1545869cfcd430aeb55c0015f3069f87ca7d9b2760ee9d8a90d123de73ac1ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.7 MB (342650819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:127925fb34690e0661190b9c1cb5f0a79d7c27578a7309082b2082ef37d8c3bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:03:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:03:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 03:03:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 03:04:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 11:05:54 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 27 Oct 2021 20:43:11 GMT
ENV NODE_VERSION=16.13.0
# Wed, 27 Oct 2021 20:43:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 27 Oct 2021 20:43:46 GMT
ENV YARN_VERSION=1.22.15
# Wed, 27 Oct 2021 20:43:52 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 27 Oct 2021 20:43:54 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Wed, 27 Oct 2021 20:43:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Oct 2021 20:43:56 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607051b9b8b0e248adc1dbae78b910c62d134181c4945e4df5e165ba533f7dea`  
		Last Modified: Sat, 16 Oct 2021 03:18:13 GMT  
		Size: 10.2 MB (10216060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c91f590ca18c241c146cf6ad6fb66517634bedc0681afcc69d37ee25828046`  
		Last Modified: Sat, 16 Oct 2021 03:18:12 GMT  
		Size: 3.9 MB (3873851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e454b57055514895812b6c056855e692fa41c1c6c1ba7f0cf0a57c78e9a0b8c`  
		Last Modified: Sat, 16 Oct 2021 03:18:31 GMT  
		Size: 47.7 MB (47733794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21de0b7ad6c69f39e1549dfe74c8e144c7db5ddf9434ed52e9a925d372a4af7`  
		Last Modified: Sat, 16 Oct 2021 03:19:09 GMT  
		Size: 201.8 MB (201760994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c386511c38cbc44b438822953c897089f48e6ff3d7c704c32e8152e8f09ecfe0`  
		Last Modified: Sat, 16 Oct 2021 11:18:58 GMT  
		Size: 4.1 KB (4088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01553c03db167b7cd9e4955ed8f369b4083b9ee065396d4f9b23492b1a9be72`  
		Last Modified: Wed, 27 Oct 2021 20:59:06 GMT  
		Size: 33.6 MB (33567875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0781c3f12a8fdea3e3ca7542eb19b94ba864699c1e4db7aaf9e9630b0db4b308`  
		Last Modified: Wed, 27 Oct 2021 20:59:01 GMT  
		Size: 2.3 MB (2316994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9b03201aaaf78ac704ce4a31af3bbed9f0c67e76583a3bdde7f6a10892b453`  
		Last Modified: Wed, 27 Oct 2021 20:59:01 GMT  
		Size: 466.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
