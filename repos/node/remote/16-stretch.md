## `node:16-stretch`

```console
$ docker pull node@sha256:e452f5525539abc70a703e1bd69b9c9006e2c61b94336704497f0c5f9a0c806c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `node:16-stretch` - linux; amd64

```console
$ docker pull node@sha256:3586638cac87dc18211f4cdd56e8ea7111698f09c645da09f88dee4ae201d4f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.8 MB (361794876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ecbffda8b5ddf3065f272b7d9aadbcc199ae58fdbfdce8701ca787da1d0114f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Fri, 03 Sep 2021 01:23:33 GMT
ADD file:835effce8521d3a6cb00dc8bb358711e7a6ba1fd057b798681d9e006825dd3c1 in / 
# Fri, 03 Sep 2021 01:23:33 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:36:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:36:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 06:36:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:37:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 07:49:24 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 23 Sep 2021 18:44:45 GMT
ENV NODE_VERSION=16.10.0
# Thu, 23 Sep 2021 18:45:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 23 Sep 2021 18:45:32 GMT
ENV YARN_VERSION=1.22.5
# Thu, 23 Sep 2021 18:45:39 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 23 Sep 2021 18:45:39 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 23 Sep 2021 18:45:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 18:45:39 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:1c05d83e138cea8cb6ddd17442ab2138423db80e58408d93059f2ea25065952e`  
		Last Modified: Fri, 03 Sep 2021 01:31:39 GMT  
		Size: 45.4 MB (45379797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394ee1959bac9492a9fc64334844549eccd4274280678d81d6b5b19af703e2a6`  
		Last Modified: Fri, 03 Sep 2021 06:42:58 GMT  
		Size: 11.3 MB (11295763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5f175d1abbc6d4a7774bd2912a927aa78b90fb04fb43d591e3dda317c9bb96`  
		Last Modified: Fri, 03 Sep 2021 06:42:57 GMT  
		Size: 4.3 MB (4342391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7885553ee256f7f9d1dd3016c0fd0c72fcd46217439371e3e1f610af0d159004`  
		Last Modified: Fri, 03 Sep 2021 06:43:17 GMT  
		Size: 49.8 MB (49761954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444120dfcd5ee8b1a6036ac87371c1912f9901705670c15ade07478e931fed3b`  
		Last Modified: Fri, 03 Sep 2021 06:43:56 GMT  
		Size: 214.4 MB (214428177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606c05f394942673e1d9cc6701eae15cee71fe34bb30e168b3b4b093894c69fb`  
		Last Modified: Fri, 03 Sep 2021 08:07:39 GMT  
		Size: 4.2 KB (4188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e8ec626bce35e71af869e38c350e8bce823bbbe61fe2beaee974c69ebe89cf`  
		Last Modified: Thu, 23 Sep 2021 18:56:26 GMT  
		Size: 34.3 MB (34263273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b44dc0bba764119161f299d5be3645af7cc524fab38c88fef60aa21838fa36`  
		Last Modified: Thu, 23 Sep 2021 18:56:19 GMT  
		Size: 2.3 MB (2319037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0626975322907ae0ced91dec48915a181d3a68a8885a5caefcbbdf021bb316d2`  
		Last Modified: Thu, 23 Sep 2021 18:56:19 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:16-stretch` - linux; arm variant v7

```console
$ docker pull node@sha256:afe4d3984f3ba80adea10859945f3e901318af6e6af10d08b17698bd957bd279
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.1 MB (331054693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d2a97c0b6a9e75d075d6518c341e7e7095cd0e8134bece09420431f9173fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Fri, 03 Sep 2021 01:04:44 GMT
ADD file:f3526ca980237b2ca5289ca7a6c67760fc5726ce3c325de10f3f3111c1d4bdcd in / 
# Fri, 03 Sep 2021 01:04:45 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 03:03:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 03:03:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 03:04:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 03:06:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 08:18:34 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 23 Sep 2021 20:25:30 GMT
ENV NODE_VERSION=16.10.0
# Thu, 23 Sep 2021 20:26:00 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 23 Sep 2021 20:26:01 GMT
ENV YARN_VERSION=1.22.5
# Thu, 23 Sep 2021 20:26:08 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 23 Sep 2021 20:26:09 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 23 Sep 2021 20:26:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Sep 2021 20:26:10 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:aba3565275cf0ab544dbd3d27fb468b4682c0273b64b5f3d8c8fe06ca3467237`  
		Last Modified: Fri, 03 Sep 2021 01:21:57 GMT  
		Size: 42.1 MB (42119584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d7b8704af020029979f5a4bfc12eaea904235f452d75b61476aa90807ec20b`  
		Last Modified: Fri, 03 Sep 2021 03:22:05 GMT  
		Size: 10.0 MB (9951651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef77f0ed56b31ff8d57db5fd7149505dac04ef41f4919d6a59ed5e3725a6f4e`  
		Last Modified: Fri, 03 Sep 2021 03:22:03 GMT  
		Size: 3.9 MB (3921218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612339c5de82d58230628e90ab66882406b5153ad5eecc07c42f9418c7404e11`  
		Last Modified: Fri, 03 Sep 2021 03:22:49 GMT  
		Size: 46.1 MB (46125736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43545e002b261585c18c3195a8c56088a38b5ca2b4a8d2e48bc88ef35e822f4d`  
		Last Modified: Fri, 03 Sep 2021 03:24:48 GMT  
		Size: 195.0 MB (195048804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed34c8c2b67721cef910116c860f208fac60c8b3713fb760549915a0f5c4da0`  
		Last Modified: Fri, 03 Sep 2021 08:56:08 GMT  
		Size: 4.2 KB (4175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5dbd12926bc0d9a06238571bcf91eb87fb97d82da54da014376a66a97992f5`  
		Last Modified: Thu, 23 Sep 2021 20:52:15 GMT  
		Size: 31.6 MB (31572262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2643ee86a03391b4d82d274766c14bc39d720f87dff4b072abab7f45ec8af8b`  
		Last Modified: Thu, 23 Sep 2021 20:51:55 GMT  
		Size: 2.3 MB (2310970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ab8d9e8ed1e7619bdce655a5fd6752608ca016b5dceb30a7addd3d2878b9ac`  
		Last Modified: Thu, 23 Sep 2021 20:51:53 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:16-stretch` - linux; arm64 variant v8

```console
$ docker pull node@sha256:10bbcfdd7378b0ed9de88af36e48abef75332ef77f3586da9e7dc85674093901
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.7 MB (343705119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c81941488782274370d3df30c07554f2c71b25392a2d3e380cf02143d7a01dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:10 GMT
ADD file:d66cac067d9b02a4946e6816144b6c89b971f95947a48715a50600a63d153b56 in / 
# Tue, 28 Sep 2021 01:43:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:20:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:20:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:20:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:21:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 05:06:04 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 28 Sep 2021 05:06:04 GMT
ENV NODE_VERSION=16.10.0
# Tue, 28 Sep 2021 05:06:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Tue, 28 Sep 2021 05:06:49 GMT
ENV YARN_VERSION=1.22.5
# Tue, 28 Sep 2021 05:06:57 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Tue, 28 Sep 2021 05:06:58 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Tue, 28 Sep 2021 05:06:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 05:06:58 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:7b4ff8ad8c828f0855329495e1260f28de7fc1e828e3339b7dddc2d116d19742`  
		Last Modified: Tue, 28 Sep 2021 01:52:24 GMT  
		Size: 43.2 MB (43176860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056e66b20944d4cb1ecbb1744d2851e6e3f89c80e9db3afff03b3fc1c1291768`  
		Last Modified: Tue, 28 Sep 2021 02:28:21 GMT  
		Size: 10.2 MB (10216473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac70c4411ef34b85e9e038bdd0e1c5fb4b27ce5be304cdb9479fe829e2ab9886`  
		Last Modified: Tue, 28 Sep 2021 02:28:19 GMT  
		Size: 4.1 MB (4096542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65cdaa18192aee6f9c254882a3a7f4e57f28681ee263e9fd155fefcd6d9a7e7f`  
		Last Modified: Tue, 28 Sep 2021 02:28:40 GMT  
		Size: 47.7 MB (47737758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445c016c41e0197a8c0587a7bdc804370e31412e49c9bd80ba6baa0b67074d1c`  
		Last Modified: Tue, 28 Sep 2021 02:29:20 GMT  
		Size: 201.8 MB (201758610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c6aceb7b4ffa8a31e71d409d5f1d1c8ee341e4e320eea9d0fdcae2044480d3`  
		Last Modified: Tue, 28 Sep 2021 05:27:43 GMT  
		Size: 4.2 KB (4197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76af17abc585cd670c2d727e87f378f7ae3e191ae4a7eca1440f358b0d0f7db2`  
		Last Modified: Tue, 28 Sep 2021 05:27:48 GMT  
		Size: 34.4 MB (34399928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddac7ee9ea8f4d3f4f97f8a98d747485e5d82c0f4034bef418733931876457c9`  
		Last Modified: Tue, 28 Sep 2021 05:27:43 GMT  
		Size: 2.3 MB (2314458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54f8981bcc6a24fa5890b3a6ab0f40e0f78cedc3caa011159cbbe982eaecdf0`  
		Last Modified: Tue, 28 Sep 2021 05:27:42 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
