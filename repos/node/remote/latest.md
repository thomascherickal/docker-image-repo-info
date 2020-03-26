## `node:latest`

```console
$ docker pull node@sha256:ad341aff5db73b2c13b55b83fbf7e2aa5164b90c365dfdd7d6e33cd1aa74a108
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `node:latest` - linux; amd64

```console
$ docker pull node@sha256:4532612779da5a878786b8ce91e8d4c3a9441958a397494bfa2f2cb3bbb8488c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362256311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ada5fbfe5a54200452926354d7246571b949bc997622e7d03d36a0c16e1bc3d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:14 GMT
ADD file:08c5ab7c53526da155d6be40a9795fc08afc9f47bd333c096e90185fe9fab2b1 in / 
# Wed, 26 Feb 2020 00:41:14 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:17:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:17:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:17:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:18:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 06:41:17 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 26 Mar 2020 20:24:53 GMT
ENV NODE_VERSION=13.11.0
# Thu, 26 Mar 2020 20:25:07 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     77984A986EBC2AA786BC0F66B01FBB92821C587A     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     4ED778F539E3634C779C87C6D7062848A1AB005C     A48C2BEE680E841632CD4E44F07496B3EB3C1762     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 26 Mar 2020 20:25:07 GMT
ENV YARN_VERSION=1.22.4
# Thu, 26 Mar 2020 20:25:12 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 26 Mar 2020 20:25:13 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 26 Mar 2020 20:25:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Mar 2020 20:25:14 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:c0c53f743a403d45480d026864d9611d6eb898e897d60c13ae854ad453d462a4`  
		Last Modified: Wed, 26 Feb 2020 00:47:05 GMT  
		Size: 45.4 MB (45375932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66997431d390aecfd02e57222c9b5752d314a4508de82c9b43c66812c3434ed4`  
		Last Modified: Wed, 26 Feb 2020 01:23:37 GMT  
		Size: 10.8 MB (10797283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea865e2909f355d736daef9076ecda63b3075c6267b858d9eaaf2e3966fc0d2`  
		Last Modified: Wed, 26 Feb 2020 01:23:36 GMT  
		Size: 4.3 MB (4340193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584bf23912b71bbd038602cb98cf5207cb2183a8b7b49fa4b16fa2018e09f508`  
		Last Modified: Wed, 26 Feb 2020 01:23:52 GMT  
		Size: 50.1 MB (50070212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4c73959f29d362478996015b71e5f4ba5360b835ec71c2435ff03f4d3f3112`  
		Last Modified: Wed, 26 Feb 2020 01:24:38 GMT  
		Size: 214.9 MB (214895058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e05266fc4bb48f2013a48199c304cc521640ffb0be9fd1895a8a4d2cf9c5df`  
		Last Modified: Wed, 26 Feb 2020 06:57:54 GMT  
		Size: 4.2 KB (4163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d214fbc04d587a02c510460b41e91fbdc0deb1176a113c46826d45340c63beb`  
		Last Modified: Thu, 26 Mar 2020 20:32:52 GMT  
		Size: 34.4 MB (34398719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdea17640a8be7ec275a7fc4d93d4f2209f32a935ba3f6a969a50344cc1eba8d`  
		Last Modified: Thu, 26 Mar 2020 20:32:42 GMT  
		Size: 2.4 MB (2374457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3f35547985ca53e94ed9f9e32fd7c24f5ad095b0ab050f9c00f58f85eba335`  
		Last Modified: Thu, 26 Mar 2020 20:32:41 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:latest` - linux; arm variant v7

```console
$ docker pull node@sha256:0ee9a92644ad16db016684f496d80c64c4a2e440f0bee3b0b9c6d559cb38c69d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.3 MB (332276369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33dc4a69b76c6a3b00499ca00342d7506e408f967f24e4737b19264ed921b301`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Wed, 26 Feb 2020 00:59:40 GMT
ADD file:6497e2f777f4487d9221931005a8b4b81c021442a769b581e223cf30c81ff553 in / 
# Wed, 26 Feb 2020 00:59:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:27:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:27:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 02:28:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:30:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:15:00 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 26 Mar 2020 20:27:56 GMT
ENV NODE_VERSION=13.11.0
# Thu, 26 Mar 2020 20:28:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     77984A986EBC2AA786BC0F66B01FBB92821C587A     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     4ED778F539E3634C779C87C6D7062848A1AB005C     A48C2BEE680E841632CD4E44F07496B3EB3C1762     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 26 Mar 2020 20:28:28 GMT
ENV YARN_VERSION=1.22.4
# Thu, 26 Mar 2020 20:28:34 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 26 Mar 2020 20:28:34 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 26 Mar 2020 20:28:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Mar 2020 20:28:36 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:2478a2ed882cb5fbb5e4e92c9f580da9ca52f5fc78b8bb439ecbf3ac18023caa`  
		Last Modified: Wed, 26 Feb 2020 01:11:29 GMT  
		Size: 42.1 MB (42100335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c541086e0dffa72464d4077dcc60504a1c08a73ecec554c159269786ba08fed`  
		Last Modified: Wed, 26 Feb 2020 02:37:24 GMT  
		Size: 9.5 MB (9498391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf0f97b070f73118badb36d21af3459f8317d4ac6d45aec680092cc962f1c47`  
		Last Modified: Wed, 26 Feb 2020 02:37:23 GMT  
		Size: 3.9 MB (3918781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d620eb05d9fd9184b8f200537b866a27af44aa6d7ef4dd6113bf1b51421d4795`  
		Last Modified: Wed, 26 Feb 2020 02:37:45 GMT  
		Size: 46.4 MB (46391794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f6d10893167716e03df782cfd3f378f099999787bc15655d27fd06cc601e46`  
		Last Modified: Wed, 26 Feb 2020 02:38:40 GMT  
		Size: 195.5 MB (195548773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1934fd204d094c749c5f5a793b048dda0950d338045e106046a054d00a5e9763`  
		Last Modified: Wed, 26 Feb 2020 16:42:28 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59881337d53f7dffaf0046013caeeebc21ad988f8e6bad62a414f79cf9a24c1`  
		Last Modified: Thu, 26 Mar 2020 20:42:26 GMT  
		Size: 32.4 MB (32448806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524baa08be0b86b5154e916bc28959577081a9debbf9779688f2ed1723131950`  
		Last Modified: Thu, 26 Mar 2020 20:42:15 GMT  
		Size: 2.4 MB (2365017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571520ac522c1194e71ae6de4c552506ceaf5e03e7971565853576afb2dc5b20`  
		Last Modified: Thu, 26 Mar 2020 20:42:14 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:latest` - linux; arm64 variant v8

```console
$ docker pull node@sha256:f8232a30af45a12f5828c26ae03a5cbc831f7f83e6b1df9e9ef98e3d29b5e327
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.2 MB (344220369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdcc3afd6b201ff95a5f5fa498d2d27a04d30debb6bab11c1de30a4f16813de8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:03 GMT
ADD file:c82c7dc82c2eb3b50218c35e1b848f707b134d2df957f57125408f69aaeb9b96 in / 
# Wed, 26 Feb 2020 00:50:15 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:59:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:59:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 04:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:02:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 18:42:11 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 26 Mar 2020 20:08:40 GMT
ENV NODE_VERSION=13.11.0
# Thu, 26 Mar 2020 20:08:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     77984A986EBC2AA786BC0F66B01FBB92821C587A     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     4ED778F539E3634C779C87C6D7062848A1AB005C     A48C2BEE680E841632CD4E44F07496B3EB3C1762     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 26 Mar 2020 20:08:54 GMT
ENV YARN_VERSION=1.22.4
# Thu, 26 Mar 2020 20:09:00 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 26 Mar 2020 20:09:01 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 26 Mar 2020 20:09:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Mar 2020 20:09:03 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:668c278237ef972312df4979c8fb1a927b38db5da09f094ae4fcc84a061dedf8`  
		Last Modified: Wed, 26 Feb 2020 00:58:30 GMT  
		Size: 43.2 MB (43158146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b41cac09012800692bd13a1238260bfb293c18c7864536c494809f2983ad770`  
		Last Modified: Wed, 26 Feb 2020 04:08:32 GMT  
		Size: 9.7 MB (9748511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094b353938273b0bbc576a8a80a232614ca2d9bfe48769641eee7055f3db6a5e`  
		Last Modified: Wed, 26 Feb 2020 04:08:31 GMT  
		Size: 4.1 MB (4094435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fba2538bf9e06bc84462d53d1effc13ecb38f026a6bc0df91cb9da3ffc0fb1`  
		Last Modified: Wed, 26 Feb 2020 04:08:53 GMT  
		Size: 48.0 MB (48024341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1c9497c36a170d2db3389cf07b65d1cb488f7af1bf0f048be8458986d60567`  
		Last Modified: Wed, 26 Feb 2020 04:09:50 GMT  
		Size: 202.3 MB (202280174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a4932b0ed28d335cf72cf6fdd5877c3eb39ecd85b6f4e411c2da1afa07b189`  
		Last Modified: Wed, 26 Feb 2020 18:55:51 GMT  
		Size: 4.2 KB (4194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29393e9cbc39c17774157fd7ccaa65c533137e10c2e1af9b1f8f523137d557b5`  
		Last Modified: Thu, 26 Mar 2020 20:35:51 GMT  
		Size: 34.5 MB (34535956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9655b26cf3705e1af57dccec87369ce08d012724be0fa1daa3269b0502f7ee`  
		Last Modified: Thu, 26 Mar 2020 20:35:40 GMT  
		Size: 2.4 MB (2374319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52bbc683b7d823e19f53284984dc3f7edbedcb445efb36e1b3eba221ddb6d3b`  
		Last Modified: Thu, 26 Mar 2020 20:35:40 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:latest` - linux; ppc64le

```console
$ docker pull node@sha256:8979d64cd25859a286bbdc41acdd143eae395ca8ebaa94b134f7bee46f0da17c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.2 MB (357157983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d25db1ea0b04c0985e7c5e78fbe8390abb7045653c01ac3e85558ee5ffc386`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Wed, 26 Feb 2020 01:36:21 GMT
ADD file:734d2a25bec5d510e72f822b21a5ef5786a928c6cb933209a04c6358fd600b67 in / 
# Wed, 26 Feb 2020 01:36:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 08:30:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 08:31:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 08:33:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 08:44:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 16:09:49 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 26 Mar 2020 20:09:34 GMT
ENV NODE_VERSION=13.11.0
# Thu, 26 Mar 2020 20:09:51 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     77984A986EBC2AA786BC0F66B01FBB92821C587A     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     4ED778F539E3634C779C87C6D7062848A1AB005C     A48C2BEE680E841632CD4E44F07496B3EB3C1762     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 26 Mar 2020 20:09:55 GMT
ENV YARN_VERSION=1.22.4
# Thu, 26 Mar 2020 20:10:08 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 26 Mar 2020 20:10:10 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 26 Mar 2020 20:10:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Mar 2020 20:10:15 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:3a8babb46b416d2208716bc29bc3e805dd074b943418fc44ac89d66e363bc68a`  
		Last Modified: Wed, 26 Feb 2020 02:03:30 GMT  
		Size: 45.6 MB (45647081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b58107739cb9bc4ee26b798057c5699d3917b41fdd5074d870c116173ef2b88d`  
		Last Modified: Wed, 26 Feb 2020 08:54:46 GMT  
		Size: 10.0 MB (10002548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2a9dde531080020a5aecc53631e693820a9b6870602303e1eec2d17f6591e1`  
		Last Modified: Wed, 26 Feb 2020 08:54:43 GMT  
		Size: 4.3 MB (4296749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d0a325b030abc66d25e8263d0ed1e03cd7c249159491c7681e444b6cf13fd8`  
		Last Modified: Wed, 26 Feb 2020 08:55:34 GMT  
		Size: 50.1 MB (50083192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28ed0e030df85f26e512a53e9ab53fea54fb890f9659448426dacc339ef6838`  
		Last Modified: Wed, 26 Feb 2020 08:57:33 GMT  
		Size: 210.5 MB (210509590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ca23a7e3dff2ac2b82a0df7abf699a0620829f172e6580b3820e79faf641f2`  
		Last Modified: Wed, 26 Feb 2020 16:45:32 GMT  
		Size: 4.2 KB (4211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8c7b89c7b8d2a8343390a68ac8abb8fda175ff35ef6bde7493f9ecb68a5727`  
		Last Modified: Thu, 26 Mar 2020 21:01:05 GMT  
		Size: 34.2 MB (34239881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9aa1a8ba79c893aa997fbe84970dbfaf5beb75e92a52b73bc6ce0580153e71`  
		Last Modified: Thu, 26 Mar 2020 21:00:47 GMT  
		Size: 2.4 MB (2374436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8685b1ba00a3ef71df78954ddcacc1a51074925488375687bf134f4e8cf273a`  
		Last Modified: Thu, 26 Mar 2020 21:00:47 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:latest` - linux; s390x

```console
$ docker pull node@sha256:609b6a94f5275d9789d6e0ab74792e3b3f3d50c409f27e64e3a578029bd7f6ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.3 MB (354259790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28b0f74153f7fdd89ae88a4f791b57a8b9518ace83fbb35d40ab0a2146c9a9fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Wed, 26 Feb 2020 00:44:30 GMT
ADD file:bb76ab55808bcd0567a32c3d7328d5c1719147f0f723a4aa574872eb8f12b4d4 in / 
# Wed, 26 Feb 2020 00:44:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:42:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 04:42:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:44:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 07:41:18 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 26 Mar 2020 20:35:04 GMT
ENV NODE_VERSION=13.11.0
# Thu, 26 Mar 2020 20:35:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     FD3A5288F042B6850C66B31F09FE44734EB7990E     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     B9AE9905FFD7803F25714661B63B535A4C206CA9     77984A986EBC2AA786BC0F66B01FBB92821C587A     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     4ED778F539E3634C779C87C6D7062848A1AB005C     A48C2BEE680E841632CD4E44F07496B3EB3C1762     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 26 Mar 2020 20:35:29 GMT
ENV YARN_VERSION=1.22.4
# Thu, 26 Mar 2020 20:35:35 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 26 Mar 2020 20:35:36 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 26 Mar 2020 20:35:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Mar 2020 20:35:38 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:a2baf8ed1bce68a4f36469f3537f12b9e5bebc860ab4aac0954714901595c575`  
		Last Modified: Wed, 26 Feb 2020 00:49:08 GMT  
		Size: 45.2 MB (45232848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58b9c529db9ec73f2bb8ba3f678b389c4df7bdb3ff1083ebf516aee839533b2`  
		Last Modified: Wed, 26 Feb 2020 04:49:17 GMT  
		Size: 10.3 MB (10325927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d9d2deeb51ba62efa7f9206911520eae29fdd6a401851f5f400f881ef0fbc8`  
		Last Modified: Wed, 26 Feb 2020 04:49:16 GMT  
		Size: 4.4 MB (4372671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:945d494eee6f349916e86f798c51b0ee9e6c3e769f797eb840c23ce5857bed41`  
		Last Modified: Wed, 26 Feb 2020 04:49:30 GMT  
		Size: 50.5 MB (50500268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32172ae2ff63a2a428c16879a62e110ef908cf42a10b9fc15275a5bc9bb8707c`  
		Last Modified: Wed, 26 Feb 2020 04:50:00 GMT  
		Size: 206.9 MB (206915719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f19e02b0ca62a61816a8f1b60cd79d2c09e85e064da7ee89ac2f9baea5e84`  
		Last Modified: Wed, 26 Feb 2020 07:55:02 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b52d0b8e5189e43af75a97d617ae2123d397c61c3471a5112ad9e0f44f34fc`  
		Last Modified: Thu, 26 Mar 2020 21:30:44 GMT  
		Size: 34.5 MB (34530163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66865c91946e6f4484218ba6de5771aa0f19773aad59138a1ad2b40295a8330`  
		Last Modified: Thu, 26 Mar 2020 21:30:26 GMT  
		Size: 2.4 MB (2377709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9dbe5ea18a5f7bcc1d839495c6a3538165123dc75f3c1768e249b75e7ced3c2`  
		Last Modified: Thu, 26 Mar 2020 21:30:26 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
