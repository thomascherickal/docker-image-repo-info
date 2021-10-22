## `node:fermium`

```console
$ docker pull node@sha256:ab6c8cd32006f8a4c1c795e55ddfbc7f54f5a3fb7318506ecb355cab8f5e7182
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `node:fermium` - linux; amd64

```console
$ docker pull node@sha256:e0dd89382d4f7da3b2be5d5fb74c65bfa1836deecae3c5f88919f44b469025f9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.7 MB (362700136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31421e72129c508a69ae6b4681101596908a091c9097591b73851fd4470264b7`
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
# Wed, 13 Oct 2021 05:50:56 GMT
ENV NODE_VERSION=14.18.1
# Wed, 13 Oct 2021 05:51:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 13 Oct 2021 05:51:33 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 05:51:39 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 22 Oct 2021 18:55:45 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:55:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 18:55:45 GMT
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
	-	`sha256:5037d4710e071cf1f6f5bf24831fab5093d28a1e5fc58b9fff5309bfa193b7bc`  
		Last Modified: Wed, 13 Oct 2021 06:09:33 GMT  
		Size: 35.1 MB (35140833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714346faf07fac8b4573637cb4d6e768b07d7583677b3046dd8d76efff72270a`  
		Last Modified: Wed, 13 Oct 2021 06:09:28 GMT  
		Size: 2.3 MB (2333785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a56afa5a7808121dd05fd91cfe718eb46f8ecc22a34539eca6274e193ba2237`  
		Last Modified: Fri, 22 Oct 2021 19:09:16 GMT  
		Size: 464.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:fermium` - linux; arm variant v7

```console
$ docker pull node@sha256:f91ead644b76572f85c1634fa25c68659ab155b4126fcdf5b6e035aed8d1e800
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.8 MB (332812794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7612c9559ad4ce6cccb910860f99213f60a250559c9a94a3e5f63186fbec6c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:07 GMT
ADD file:eb5955ccd54a486767e85aeb1c03ffc6d8667b5476d0cf17b892ca407f1c8853 in / 
# Tue, 12 Oct 2021 01:34:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:48:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 18:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:51:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 03:03:05 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 13 Oct 2021 04:36:16 GMT
ENV NODE_VERSION=14.18.1
# Wed, 13 Oct 2021 04:36:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 13 Oct 2021 04:36:49 GMT
ENV YARN_VERSION=1.22.15
# Wed, 13 Oct 2021 04:36:56 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 22 Oct 2021 18:13:26 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 18:13:27 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:8e9db3616ec4491d75e6c28254ff2376f24900797e7c4cc464f36a0c502b111f`  
		Last Modified: Tue, 12 Oct 2021 01:51:20 GMT  
		Size: 42.1 MB (42119423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdf02e61fe0ab1563ba0431b63fade0e2dc7930d82d8c1a7ec6ee395072fdb3`  
		Last Modified: Tue, 12 Oct 2021 19:06:50 GMT  
		Size: 10.0 MB (9955968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a752ebf54d1b82943abce28e108346c5d28e94fdb8f419cfffea0b639341ce6`  
		Last Modified: Tue, 12 Oct 2021 19:06:46 GMT  
		Size: 3.9 MB (3921159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38df34fca09f092dbbe9b57c3c215fd84572924c049269f617cdc79e0e8be50c`  
		Last Modified: Tue, 12 Oct 2021 19:07:34 GMT  
		Size: 46.1 MB (46126075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a60d616f09d782db77be5964859fbefcfd130ef1614004ac408c1f856d5b9d1`  
		Last Modified: Tue, 12 Oct 2021 19:09:30 GMT  
		Size: 195.1 MB (195050378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd5f91ad14f521d3ea8eb8f0d71f9b48302e340730d97f9114fa1fdec58b4a5`  
		Last Modified: Wed, 13 Oct 2021 06:12:10 GMT  
		Size: 4.2 KB (4177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8381dcb5ef9c4a2599103fc13eb2fc4187ede2b732086e129dc86af6664c6f`  
		Last Modified: Wed, 13 Oct 2021 06:20:43 GMT  
		Size: 33.3 MB (33309498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd8121d4c195950c56ebce83f2c035e5c4fbb1243c84312523481545b29544e`  
		Last Modified: Wed, 13 Oct 2021 06:20:21 GMT  
		Size: 2.3 MB (2325651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e16e29ee3499d673fb76a9333f0ad2bee9496d53624e7b814db19d48259e12`  
		Last Modified: Fri, 22 Oct 2021 18:43:23 GMT  
		Size: 465.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:fermium` - linux; arm64 variant v8

```console
$ docker pull node@sha256:af986e243e415ab3e2c5d33eccb7258ca18855209c7aeb8a9f7ef5c7a3475c15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.3 MB (344339523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae0da6f36a6a63be93c2c1c2b715f7abccde13c85fbbed9d39d08cf2f35648c`
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
# Sat, 16 Oct 2021 11:08:50 GMT
ENV NODE_VERSION=14.18.1
# Sat, 16 Oct 2021 11:09:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Sat, 16 Oct 2021 11:09:23 GMT
ENV YARN_VERSION=1.22.15
# Sat, 16 Oct 2021 11:09:29 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 22 Oct 2021 17:48:06 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 22 Oct 2021 17:48:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Oct 2021 17:48:09 GMT
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
	-	`sha256:279ddcb6e47b9f84b52a2bfa8fd6a8b80d4be9b4c5f86ecb41582505637d356e`  
		Last Modified: Sat, 16 Oct 2021 11:20:46 GMT  
		Size: 35.2 MB (35241800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6588c2fa1bd01a71a79dae91784f13638a6cc8115d5ad7031c544ca4c3235d9`  
		Last Modified: Sat, 16 Oct 2021 11:20:40 GMT  
		Size: 2.3 MB (2331776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4d550485c6fae7cdc0d59adc2d3c0e0d546013367d830267179cecd1c3007c`  
		Last Modified: Fri, 22 Oct 2021 18:05:30 GMT  
		Size: 463.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
