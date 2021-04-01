## `node:lts-buster`

```console
$ docker pull node@sha256:e09a63130ce4ec4b20af5bd07e2029a0ef26f64f1f496f0854f5b1ff1aa69575
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `node:lts-buster` - linux; amd64

```console
$ docker pull node@sha256:ba10d674532e56ed647a17e2593896ca4affa72dd4c64320407836243198c735
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.3 MB (349296108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61560e1cedb8101d32b5fba18dacceae39c1bbac5b75027cb65a662b38a36780`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:03:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:05:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:00:19 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 31 Mar 2021 05:03:11 GMT
ENV NODE_VERSION=14.16.0
# Wed, 31 Mar 2021 05:03:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 31 Mar 2021 05:03:19 GMT
ENV YARN_VERSION=1.22.5
# Wed, 31 Mar 2021 05:03:22 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 31 Mar 2021 05:03:22 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 31 Mar 2021 05:03:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 05:03:23 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234b70d0479d7f16d7ee8d04e4ffdacc57d7d14313faf59d332f18b2e9418743`  
		Last Modified: Tue, 30 Mar 2021 23:14:37 GMT  
		Size: 51.8 MB (51840782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa07a00e2f029c4b2c7f177a2b696f1b3510040cde4f5bb06ddbca98e7fbf76`  
		Last Modified: Tue, 30 Mar 2021 23:15:30 GMT  
		Size: 192.4 MB (192350814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879ffd9f5570ab015879af67aa6d0ddb179d0d80799fe812fde19511a84af47f`  
		Last Modified: Wed, 31 Mar 2021 05:14:32 GMT  
		Size: 4.2 KB (4200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b10819766623687ff37b080abaf2d18e0d8b2e41f1f370dfec6ef10e4226f0e`  
		Last Modified: Wed, 31 Mar 2021 05:17:19 GMT  
		Size: 34.5 MB (34523291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124761c792fe5250ffd63f34e7dfd89be01a297817e4d994c79f9ce0b64dc2d3`  
		Last Modified: Wed, 31 Mar 2021 05:17:13 GMT  
		Size: 2.3 MB (2314080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff21b348f42f0af45827f1f93fdc4a30f08eabee2c939f3ed3c6ea9dc262b90`  
		Last Modified: Wed, 31 Mar 2021 05:17:13 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:lts-buster` - linux; arm variant v7

```console
$ docker pull node@sha256:de4719705826007577c2fc9c8cc87cc3fa5a87c94f3a5685435b8fb06625ac5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313345247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77357f7825cb7cea1773167b68c34d4a371c856fa4c70b9b9b595bd81c70c313`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 30 Mar 2021 23:08:08 GMT
ADD file:bd48b3fec0eec547919c9e90c2055f1d879c78e4eb7d92598bf55c0f83c44836 in / 
# Tue, 30 Mar 2021 23:08:12 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:22:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:22:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 01:23:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:25:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:48:49 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 31 Mar 2021 02:53:35 GMT
ENV NODE_VERSION=14.16.0
# Wed, 31 Mar 2021 02:53:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 31 Mar 2021 02:53:51 GMT
ENV YARN_VERSION=1.22.5
# Wed, 31 Mar 2021 02:53:55 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 31 Mar 2021 02:53:59 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 31 Mar 2021 02:54:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 02:54:01 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:0bf0c5f21d801f530938b2464483aaad40947de697c29cedece44096ead1522c`  
		Last Modified: Tue, 30 Mar 2021 23:15:55 GMT  
		Size: 45.9 MB (45915428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec8c35c4e8e932b85e0233ff1c20dcdd8bc13a0238128bcfcde181c0b04b037`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 7.1 MB (7123902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d88df2bbeddb232fbd4bf0ffd8efd62285f56f8eb6e2007c1a89ecfdc0f3ad`  
		Last Modified: Wed, 31 Mar 2021 01:36:36 GMT  
		Size: 9.3 MB (9343731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f670f49de9ae76f27610a984da50b932e5dc0d3fecb1935aea3c51a2714e828f`  
		Last Modified: Wed, 31 Mar 2021 01:37:03 GMT  
		Size: 47.4 MB (47356820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff664f5847c6609c75c99b51acb1bbe1ec5b7e03f7aac8750ef864f5ff36cecb`  
		Last Modified: Wed, 31 Mar 2021 01:37:59 GMT  
		Size: 168.6 MB (168551883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5be65b5ccb912adf5282c8524f0f71f008ec944a49369208b9185938f9e73d`  
		Last Modified: Wed, 31 Mar 2021 03:09:53 GMT  
		Size: 4.2 KB (4195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ed1fc95d4bd5442f90c347311e7de5f5b82d075ea8b01701f1289e1167a79e`  
		Last Modified: Wed, 31 Mar 2021 03:12:17 GMT  
		Size: 32.7 MB (32744963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88416c3e40d680de6b62ebaabcc10e019c32b07f0074963653f28db6d2eac28`  
		Last Modified: Wed, 31 Mar 2021 03:12:07 GMT  
		Size: 2.3 MB (2304042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a2ed4c0ab224c35af7585cdf3973ad247b01f59186a5ff044a13282b1fc041`  
		Last Modified: Wed, 31 Mar 2021 03:12:05 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:lts-buster` - linux; arm64 variant v8

```console
$ docker pull node@sha256:df7c7f4ec2e4479fed822b2b314e4565ffdabe6d816f7c4370dd0da4d4a25534
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.9 MB (339930541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12b918e329f1752c50db00e716bedb15c1aa96d6f1a12c7987249274c79a84c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:15:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:18:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:01:28 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 31 Mar 2021 01:06:41 GMT
ENV NODE_VERSION=14.16.0
# Wed, 31 Mar 2021 01:06:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 31 Mar 2021 01:06:59 GMT
ENV YARN_VERSION=1.22.5
# Wed, 31 Mar 2021 01:07:05 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 31 Mar 2021 01:07:07 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:07:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 01:07:08 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70c372ae296f23e908bf1e1ed9f4c0c81a8a6d7fc48c0e2db16035bb9b7a54`  
		Last Modified: Wed, 31 Mar 2021 00:30:24 GMT  
		Size: 52.2 MB (52165620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc089388c7ca4407aec7247a44601b896e57e96d53a858fb0e8c6f2f94ab8da`  
		Last Modified: Wed, 31 Mar 2021 00:31:19 GMT  
		Size: 183.9 MB (183900636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754863281868391e5f6c82b8b29b874f9e1830f1919ac097ca6560a6ef747976`  
		Last Modified: Wed, 31 Mar 2021 01:21:49 GMT  
		Size: 4.2 KB (4204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238768c628173281bc3162a29cef7923808d66159e7249d80620b4221632200b`  
		Last Modified: Wed, 31 Mar 2021 01:24:08 GMT  
		Size: 34.6 MB (34640917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec755c817ff697a94525832b7ac0c6e41048d90ac0da7e9454a5fe5c1a04caf9`  
		Last Modified: Wed, 31 Mar 2021 01:23:59 GMT  
		Size: 2.3 MB (2314153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7f255f49584b155894f79821624b3502337e5825df64c3be03a07f04fb1691`  
		Last Modified: Wed, 31 Mar 2021 01:23:59 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:lts-buster` - linux; ppc64le

```console
$ docker pull node@sha256:7d3ebbdced84486fe2968097b344eb8795ba66dbd5aee4fb2295c8cf2f596d2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.6 MB (372564592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c265482afd5aaf0b36ea5539607422c481c2a16a721eede81e1dd75e1204f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 30 Mar 2021 22:35:16 GMT
ADD file:74f62575b50eebcaed9b3ba5dc5831f946ac72e01a5b2c74bd28ae7b978dd255 in / 
# Tue, 30 Mar 2021 22:35:25 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 02:25:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:27:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 02:31:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 02:52:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 21:34:00 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 31 Mar 2021 23:01:38 GMT
ENV NODE_VERSION=14.16.0
# Wed, 31 Mar 2021 23:02:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 31 Mar 2021 23:02:20 GMT
ENV YARN_VERSION=1.22.5
# Wed, 31 Mar 2021 23:02:31 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 31 Mar 2021 23:02:33 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 31 Mar 2021 23:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 23:02:39 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:38c5dfa64be2090539ac26f739f111c457ae78ae6864ae0361c5355144c7936e`  
		Last Modified: Tue, 30 Mar 2021 22:42:08 GMT  
		Size: 54.2 MB (54179784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba1a4ccdf1bda9cf7f483e60e0934b4e30d67c6784672b23f2127046367c787`  
		Last Modified: Wed, 31 Mar 2021 03:26:29 GMT  
		Size: 8.3 MB (8271776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9327bab5d767fa86a8a5f40d035f76dd387470a6dd1dd5e07a8a42be42e753`  
		Last Modified: Wed, 31 Mar 2021 03:26:29 GMT  
		Size: 10.7 MB (10727812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fee58c9046288bf199d75b0f016a65a12906618da199b84e55864d8da3f4424`  
		Last Modified: Wed, 31 Mar 2021 03:26:57 GMT  
		Size: 57.5 MB (57457357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b93e8d4af613b1cdba4820bc9f49bc99e967bd6042a6dd33e4aa7252b7165f1`  
		Last Modified: Wed, 31 Mar 2021 03:27:51 GMT  
		Size: 203.2 MB (203195727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e6c5cfbff9ac1407df97fd623f10ef223e0201b3132e7b042a72a142ae7277`  
		Last Modified: Thu, 01 Apr 2021 00:33:14 GMT  
		Size: 4.2 KB (4214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ff231b7afcf98eaf04be464db84124edd1ba99c48dddde71b31ac43438b9b6`  
		Last Modified: Thu, 01 Apr 2021 00:41:26 GMT  
		Size: 36.4 MB (36413544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee2d2531d4929433db3bb4721cf8dd671f2a51c6df9e4b65985f95498d7120d`  
		Last Modified: Thu, 01 Apr 2021 00:40:21 GMT  
		Size: 2.3 MB (2314094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6051a0d738274aad5b34d5d17a22c2f0e15c0f500144653d07a0db9d9fdf03b`  
		Last Modified: Thu, 01 Apr 2021 00:40:20 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:lts-buster` - linux; s390x

```console
$ docker pull node@sha256:73065bdbf190a24b106d3eb66c6b34dea4b2fe104f7d32e82dc8966ef45c6b7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.3 MB (331264799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0566a85cd3a97e433eea65a44fff25e1c26a8e98f1838d591ec1a90225f311b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:29 GMT
ADD file:79040b5dceaf577162ccacdf7ef9e018f89e7ae399d59b4f80b3860a0471177b in / 
# Tue, 30 Mar 2021 21:42:32 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:43:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 22:43:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:44:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 03:53:57 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Wed, 31 Mar 2021 03:54:50 GMT
ENV NODE_VERSION=14.16.0
# Wed, 31 Mar 2021 03:55:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Wed, 31 Mar 2021 03:55:05 GMT
ENV YARN_VERSION=1.22.5
# Wed, 31 Mar 2021 03:55:18 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Wed, 31 Mar 2021 03:55:19 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Wed, 31 Mar 2021 03:55:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 03:55:20 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:dd4a1caade48d16285d95f8062825cc6952224e43c64222e0cdcf13bc87b44ee`  
		Last Modified: Tue, 30 Mar 2021 21:46:01 GMT  
		Size: 49.0 MB (49000451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488b7badadfabcedd6ad7a531fa8681ffb922e9853deb7bb142c86c78fdd05b`  
		Last Modified: Tue, 30 Mar 2021 22:49:21 GMT  
		Size: 7.4 MB (7399948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab15bd749c981c81cfe3ea27b9a7aa17ecf7dc0ce0357b9fe7774d8006622fa`  
		Last Modified: Tue, 30 Mar 2021 22:49:21 GMT  
		Size: 9.9 MB (9883132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e972cd743ab6520beed6242099fac9a59889445dfb7a01e42ee1ced09ac0e5`  
		Last Modified: Tue, 30 Mar 2021 22:49:41 GMT  
		Size: 51.4 MB (51379958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df5b10ced3ee54342c6e637945570c630f619af47c72e827eeb7b03dc9dbba8`  
		Last Modified: Tue, 30 Mar 2021 22:50:16 GMT  
		Size: 176.9 MB (176868317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50ae9cfcebbae48ca42352e6e46a432394fcbc41d8ff9727ca62aea6aaac14e`  
		Last Modified: Wed, 31 Mar 2021 03:58:41 GMT  
		Size: 4.2 KB (4201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef8eac8489b2b5434e1497d9cb26d7ec1502d609078dceda14d15c540456b90`  
		Last Modified: Wed, 31 Mar 2021 03:59:18 GMT  
		Size: 34.4 MB (34412266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1741a0648ed1098dba2e3944bfd2c8121dde7677afbc4708507695a646aa7fd8`  
		Last Modified: Wed, 31 Mar 2021 03:59:12 GMT  
		Size: 2.3 MB (2316243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c66b0e81d71784237fd749fc4c1a7ca4266289a8a1e168225aa08592cea5978`  
		Last Modified: Wed, 31 Mar 2021 03:59:12 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
