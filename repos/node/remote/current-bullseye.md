## `node:current-bullseye`

```console
$ docker pull node@sha256:0cc15c9c3b1f0a8d654f403f5d0230d196021cc0ff998f0c3374954301bfb558
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `node:current-bullseye` - linux; amd64

```console
$ docker pull node@sha256:40783e69e336a19805e4281c0f41a9579aa653132dae9509c01959301dbbc576
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.4 MB (358421484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a9851e7f345969c3487462ca57196bbfe7eb2bcdd86ee30e7a3620751152022`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:07 GMT
ADD file:1fedf68870782f1b44cd50691444aab4061cc0c70f24e5fabe9c562cc46eb9af in / 
# Fri, 03 Sep 2021 01:21:08 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:31:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:31:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:31:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:32:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:45:54 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 23 Sep 2021 18:41:22 GMT
ENV NODE_VERSION=16.10.0
# Thu, 23 Sep 2021 18:41:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 23 Sep 2021 18:41:39 GMT
ENV YARN_VERSION=1.22.5
# Thu, 23 Sep 2021 18:41:43 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 23 Sep 2021 18:41:43 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 23 Sep 2021 18:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 18:41:44 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:955615a668ce169f8a1443fc6b6e6215f43fe0babfb4790712a2d3171f34d366`  
		Last Modified: Fri, 03 Sep 2021 01:26:55 GMT  
		Size: 54.9 MB (54926871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2756ef5f69a5190f4308619e0f446d95f5515eef4a814dbad0bcebbbbc7b25a8`  
		Last Modified: Fri, 03 Sep 2021 06:39:22 GMT  
		Size: 5.2 MB (5153100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911ea9f2bd51e53a455297e0631e18a72a86d7e2c8e1807176e80f991bde5d64`  
		Last Modified: Fri, 03 Sep 2021 06:39:23 GMT  
		Size: 10.9 MB (10871687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b0a22ee906271a6ce9ddd1754fdd7d3b59078e0b57b6cc054c7ed7ac301587`  
		Last Modified: Fri, 03 Sep 2021 06:39:45 GMT  
		Size: 54.6 MB (54566834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8584d51a9262f9a3a436dea09ba40fa50f85802018f9bd299eee1bf538481077`  
		Last Modified: Fri, 03 Sep 2021 06:40:23 GMT  
		Size: 196.4 MB (196447011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273180d834eeded1f4e496068623630c96f611322452607830823e6a9a28c43f`  
		Last Modified: Fri, 03 Sep 2021 08:05:22 GMT  
		Size: 4.2 KB (4196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d81ddee044cbbd55489dcd45ba158f494148446381b78b92f4c84d004739c7c`  
		Last Modified: Thu, 23 Sep 2021 18:54:09 GMT  
		Size: 34.2 MB (34191296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a360336b1f958461db0632f44abd4eb830e662d69270b14670497dde163f89`  
		Last Modified: Thu, 23 Sep 2021 18:54:03 GMT  
		Size: 2.3 MB (2260208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6686fb3e4f6a4195f0350a7902afb4fc7fc0c028fa4ec53fcb952d5e14c47b`  
		Last Modified: Thu, 23 Sep 2021 18:54:01 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:current-bullseye` - linux; arm variant v7

```console
$ docker pull node@sha256:bb9d9ebc20fa016cb2bc6c2d9423393b81008fa7a0b812e2a33d1c3a9c095c9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.2 MB (316238623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5029d1719b5518919cf6985d40a54ca7b9d98eddcff593ac3fda078f1891c0c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Fri, 03 Sep 2021 00:59:03 GMT
ADD file:a885b024f19da3fff424486fd5495eaae458dea6a1038715198e0449b6b00518 in / 
# Fri, 03 Sep 2021 00:59:04 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:52:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:52:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 02:53:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:55:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:13:31 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 23 Sep 2021 20:20:38 GMT
ENV NODE_VERSION=16.10.0
# Thu, 23 Sep 2021 20:20:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 23 Sep 2021 20:20:59 GMT
ENV YARN_VERSION=1.22.5
# Thu, 23 Sep 2021 20:21:04 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 23 Sep 2021 20:21:04 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 23 Sep 2021 20:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 20:21:05 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:ff8c004d0dc8a6ef263acdc2f23760be64e46bb9a75384a950f29b2c5d8b5c98`  
		Last Modified: Fri, 03 Sep 2021 01:14:05 GMT  
		Size: 50.1 MB (50127257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09133804e9cabca8aa15fc0b84dbfd8d87f0f01e28c315b5f5ea48ab2c913450`  
		Last Modified: Fri, 03 Sep 2021 03:13:16 GMT  
		Size: 4.9 MB (4922592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00fc4682956757d850f7d8ed7259e823f6c972e63fdcd37082e1673502aa085`  
		Last Modified: Fri, 03 Sep 2021 03:13:18 GMT  
		Size: 10.2 MB (10216805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2ed13e4cb879d0509b38f09a3fd873792d4e751b5be323450dd7b65f2b7f8a`  
		Last Modified: Fri, 03 Sep 2021 03:14:10 GMT  
		Size: 50.3 MB (50328201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a08aff1bdbb8475edc41c0a2e7a57ea7b0be1c8c347cb9260fe96b36ac9fa4`  
		Last Modified: Fri, 03 Sep 2021 03:16:00 GMT  
		Size: 166.9 MB (166892763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f34e8e8e4309f04807dd595dfd9c5dddfc251fda0ec0f87095c5ed851fe5ea`  
		Last Modified: Fri, 03 Sep 2021 08:52:21 GMT  
		Size: 4.2 KB (4185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b2a5d3c65f9a6e7887bcde2ea47fa1ff4e9ad66eafca24d20928b52224101b`  
		Last Modified: Thu, 23 Sep 2021 20:48:32 GMT  
		Size: 31.5 MB (31495309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995fa412e760624709975964060739d63f79a2c8c94f8eebf495668e801f6683`  
		Last Modified: Thu, 23 Sep 2021 20:48:12 GMT  
		Size: 2.3 MB (2251228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00060adb2ae5e401f4bfe09e0a0f813a434ed95efe98a57cc64c57706161767`  
		Last Modified: Thu, 23 Sep 2021 20:48:11 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:current-bullseye` - linux; arm64 variant v8

```console
$ docker pull node@sha256:805e3c4cd725e0ee3304983d2e583d654d6c86ddf2022ce090a370cf37b973e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.2 MB (350232484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dddecdf584f1698538a9e4f31e67caae3a6b64feccee56fe25eb356faecf9c8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:26 GMT
ADD file:08680140d1528c796f24dc7d0f5a83fa0ceb307a1d5da1e6ccef21471d975cd9 in / 
# Tue, 28 Sep 2021 01:40:26 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:15:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:16:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:16:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:17:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:03:19 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 28 Sep 2021 05:03:20 GMT
ENV NODE_VERSION=16.10.0
# Tue, 28 Sep 2021 05:03:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Tue, 28 Sep 2021 05:03:39 GMT
ENV YARN_VERSION=1.22.5
# Tue, 28 Sep 2021 05:03:42 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Tue, 28 Sep 2021 05:03:43 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Sep 2021 05:03:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 05:03:43 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:fa98001816c83c32d601f854ff21729167d2205310fcab15f8f9c26bdf6788d7`  
		Last Modified: Tue, 28 Sep 2021 01:47:53 GMT  
		Size: 53.6 MB (53613599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e49121c0cc80005dda9ec19bc412bdadef800cf7dc4a832b8ff229a65f82a`  
		Last Modified: Tue, 28 Sep 2021 02:24:39 GMT  
		Size: 5.1 MB (5142706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ba7d1384865fdb5a3dfafbb1264e84d27ec4e80462b8bf358f141a8cf14b64`  
		Last Modified: Tue, 28 Sep 2021 02:24:40 GMT  
		Size: 10.9 MB (10872788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7e4e85949ee45bae139f288bc1cd85a740b408abdefaaba118c4c4626b021e`  
		Last Modified: Tue, 28 Sep 2021 02:25:03 GMT  
		Size: 54.7 MB (54669786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69e7bcc0bc59e0f5c70e40bc8adebeb94f60240a71e7f8add74d8b9146bbc16`  
		Last Modified: Tue, 28 Sep 2021 02:25:44 GMT  
		Size: 189.3 MB (189337402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b37dacec8eb2a7cc25da3e72755e7374314bd1abc969ec70879b3fbcc778e2`  
		Last Modified: Tue, 28 Sep 2021 05:25:15 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227f224f6b82ce1471a8602c7fd52c0a2d0a135c0c3d9597e169237bf5b1ef71`  
		Last Modified: Tue, 28 Sep 2021 05:25:20 GMT  
		Size: 34.3 MB (34326314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af763f3b7cf9e942a1c91c59b49a6c42622be93174f2babf750791c74de55707`  
		Last Modified: Tue, 28 Sep 2021 05:25:16 GMT  
		Size: 2.3 MB (2265404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a363c7e2b7ba0a36bf5f35dc025015586a7ebe1cea530544f40c28cc5f501a04`  
		Last Modified: Tue, 28 Sep 2021 05:25:15 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:current-bullseye` - linux; ppc64le

```console
$ docker pull node@sha256:3d076bc667b55c62ddc7cf83c4b7314d71e85641ca231e6bd13697feb621a2a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **369.0 MB (368992637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98cab59ac3ff150f5c343d90917fe07611175e533421c5a35ad6c00dcd2b357e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Fri, 03 Sep 2021 01:22:22 GMT
ADD file:3d1033153ba97e1c4e4f513c14db9d9f913ee4c4ce2eeb554bcaf6c5c9665c80 in / 
# Fri, 03 Sep 2021 01:22:35 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 05:56:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 05:56:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 05:59:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:13:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 10:54:05 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 23 Sep 2021 21:30:18 GMT
ENV NODE_VERSION=16.10.0
# Thu, 23 Sep 2021 21:30:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 23 Sep 2021 21:31:09 GMT
ENV YARN_VERSION=1.22.5
# Thu, 23 Sep 2021 21:31:21 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 23 Sep 2021 21:31:24 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 23 Sep 2021 21:31:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 21:31:35 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:5180655d8cc68420b0aa96b7c8db9131c02ad0ca93c166dffc9a3a49b22005c2`  
		Last Modified: Fri, 03 Sep 2021 01:35:56 GMT  
		Size: 58.8 MB (58819434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da65065c5d0fce3d2a476e0889f0f7a8b7930d0c520fac7b518ea03e759ee66`  
		Last Modified: Fri, 03 Sep 2021 07:08:23 GMT  
		Size: 5.4 MB (5401774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33292258b5feea63dc49d85ead1ab3ab4ec648ab4c231dc8aa7db7886e21ab`  
		Last Modified: Fri, 03 Sep 2021 07:08:26 GMT  
		Size: 11.6 MB (11625942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708d04ed929be54f33cfa94416648dcac9edd8c01746ecc6e250ce046aa54ac0`  
		Last Modified: Fri, 03 Sep 2021 07:09:38 GMT  
		Size: 58.8 MB (58849139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287624e1f6e58d3860703363b792d02bb699c973abd9dadfa2db8495b51ceb93`  
		Last Modified: Fri, 03 Sep 2021 07:12:15 GMT  
		Size: 195.8 MB (195799046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd09529b633e239ac7c7ed32d2190ca685174cb88f42b747c9b39dbaf55b2be`  
		Last Modified: Fri, 03 Sep 2021 11:31:55 GMT  
		Size: 4.2 KB (4207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d2de9316bdd09324b1b41410aba7f74ecb1d285df1bd5efc2194dde9484a85`  
		Last Modified: Thu, 23 Sep 2021 22:05:11 GMT  
		Size: 36.2 MB (36232432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0911bbc09325d34695d30730fdbb21e4b201f11d433a94cd150af95c2c1a1c8`  
		Last Modified: Thu, 23 Sep 2021 22:05:04 GMT  
		Size: 2.3 MB (2260379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d1b2c7f5782a9e82de493113bd5752c9d5929c7a04403579e54d58e599f829`  
		Last Modified: Thu, 23 Sep 2021 22:05:04 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:current-bullseye` - linux; s390x

```console
$ docker pull node@sha256:d2201da3953c8a8d7f9a88b1a548fd8f8158dd9154e2af5a9dddea729d2c5c9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.9 MB (331944837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d406d486e49a8035d94e17d5aa5eb0136a8f7305a791eb760262b134df5fced5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:37 GMT
ADD file:2d93c4b98e1e98912eba220db7199c0db4b5851b041060537344b8c10bbc629a in / 
# Tue, 28 Sep 2021 01:42:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:08:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:08:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:12:54 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 28 Sep 2021 05:12:54 GMT
ENV NODE_VERSION=16.10.0
# Tue, 28 Sep 2021 05:13:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Tue, 28 Sep 2021 05:13:09 GMT
ENV YARN_VERSION=1.22.5
# Tue, 28 Sep 2021 05:13:11 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Tue, 28 Sep 2021 05:13:12 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Sep 2021 05:13:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 05:13:12 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:7b4e23a1e82dd30f03dd6b905b483772b2a8c6ac0ddd98136e1a4e0ae32674e0`  
		Last Modified: Tue, 28 Sep 2021 01:48:39 GMT  
		Size: 53.2 MB (53202311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef1f0a40a3af0d4eb38f09512ca5a72fafea0adbabe3f755677de5bdaf72fc0`  
		Last Modified: Tue, 28 Sep 2021 02:15:48 GMT  
		Size: 5.1 MB (5137147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a596155541c43ae3bbd49ee04b738fa3b8831941ce969d402e295085f04fa38b`  
		Last Modified: Tue, 28 Sep 2021 02:15:49 GMT  
		Size: 10.8 MB (10761154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f5b44618c39b6606db01fa6d460b6b7e1415b3a9c5a0b2f8b179c9b2c3fcfe`  
		Last Modified: Tue, 28 Sep 2021 02:16:05 GMT  
		Size: 54.0 MB (54049595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6589c0454003c1deeaf24f87ae908e9816d7cb9a945148cf89e75038aba3c8`  
		Last Modified: Tue, 28 Sep 2021 02:16:32 GMT  
		Size: 172.4 MB (172435364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aadbfa5bf8f30766af63ab6064d6e19a0acdb032f69d1aecd4341387fe6b588`  
		Last Modified: Tue, 28 Sep 2021 05:25:05 GMT  
		Size: 4.2 KB (4202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72c5f16744f38509b6a49e7ab68e5202a19d98a3c232a4090aa399080cf1e4e`  
		Last Modified: Tue, 28 Sep 2021 05:25:09 GMT  
		Size: 34.1 MB (34088728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c687c63cf68ef4465fe65b808cd3ef8f5e381e97cceff761647e6812ebe63433`  
		Last Modified: Tue, 28 Sep 2021 05:25:05 GMT  
		Size: 2.3 MB (2266056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd51de83cf8ec37d76f48af7b09b59b81cdb0cede10c3d9514e485297952b36b`  
		Last Modified: Tue, 28 Sep 2021 05:25:05 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
