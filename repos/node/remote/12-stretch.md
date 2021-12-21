## `node:12-stretch`

```console
$ docker pull node@sha256:5ffc6678529a9c492ea1e2fa14865f6ac219030e548e7ca8741e1c5442339625
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `node:12-stretch` - linux; amd64

```console
$ docker pull node@sha256:53f65798edb602b9001e171d472dec8ad07705d032e49988fc1e372a6cab0ed9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.3 MB (351291572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0812db557c778a5c8d4f9a540ba7f703484222f825a0d51c1eecdeb0cef7dbd9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:19 GMT
ADD file:80aa4dde5bfd685e5e660dc6ff1db4713d69bacf53ff51b7e85f8fcff80513eb in / 
# Thu, 02 Dec 2021 02:50:20 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:45:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:45:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 03:45:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:47:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 10:09:00 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Sat, 18 Dec 2021 04:32:29 GMT
ENV NODE_VERSION=12.22.8
# Sat, 18 Dec 2021 04:33:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Sat, 18 Dec 2021 04:33:03 GMT
ENV YARN_VERSION=1.22.17
# Sat, 18 Dec 2021 04:33:09 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Sat, 18 Dec 2021 04:33:10 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 18 Dec 2021 04:33:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 04:33:10 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:a44d60f8dd45ac8efc157e797930e23cf3e360bb4aae7c745efcb02c562c3e4c`  
		Last Modified: Thu, 02 Dec 2021 02:57:12 GMT  
		Size: 45.4 MB (45381394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368c5e7052170a880eff5a8f1669746c215797100578cc50a2a4903aab88a0c`  
		Last Modified: Thu, 02 Dec 2021 03:53:06 GMT  
		Size: 11.3 MB (11301554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c54a7a0d1190cf72ddfa68662ea3a2304a24dee22be784222db411737343966`  
		Last Modified: Thu, 02 Dec 2021 03:53:05 GMT  
		Size: 4.3 MB (4342399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c33912b65a4c3de70b83b983446f8fc3cde54b8d5bc9c69152a692489fdc6a7`  
		Last Modified: Thu, 02 Dec 2021 03:53:24 GMT  
		Size: 49.8 MB (49761759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606725a9d1d203885fa6b161b85d812ac3952e187d52699c683d239625142303`  
		Last Modified: Thu, 02 Dec 2021 03:54:12 GMT  
		Size: 214.4 MB (214447808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a25133c4863ee195306b999b1537c69b349e5b836f23bc54dd16bee8c211908`  
		Last Modified: Thu, 02 Dec 2021 10:34:19 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cecf40ae9249c504d2b2f2c025314d82ebed5213ddf3266d9d892505e8478bf`  
		Last Modified: Sat, 18 Dec 2021 04:42:00 GMT  
		Size: 23.7 MB (23718804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e17fed4bb72d6768796b52bb91e65ce809eb420e80b50a1d4526193edb43c9`  
		Last Modified: Sat, 18 Dec 2021 04:41:57 GMT  
		Size: 2.3 MB (2333199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994ae5bc8f9cf9ee4969987de8b5067130fb8187895700fedaab387e84101b3f`  
		Last Modified: Sat, 18 Dec 2021 04:41:56 GMT  
		Size: 464.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:12-stretch` - linux; arm variant v7

```console
$ docker pull node@sha256:de990847113a60e46a43cfabfbc3ca4ec776f33bccbb3d4524be68d8ff1ca8ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321241180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6570a34cc253d9aaf5eb82f72d96a48fe0b2e2b74c5a0ad17397e3ef7642161`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 21 Dec 2021 02:05:07 GMT
ADD file:60b016ba67df7136a5c9120c3bda872fe6fc9264670eaec4af04649094d2c53d in / 
# Tue, 21 Dec 2021 02:05:08 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:57:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:57:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:58:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:01:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 08:57:09 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 21 Dec 2021 09:23:27 GMT
ENV NODE_VERSION=12.22.8
# Tue, 21 Dec 2021 09:23:55 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Tue, 21 Dec 2021 09:23:56 GMT
ENV YARN_VERSION=1.22.17
# Tue, 21 Dec 2021 09:24:04 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Tue, 21 Dec 2021 09:24:05 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 21 Dec 2021 09:24:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Dec 2021 09:24:06 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:1680a7a0944ad84261b1979d7a37cbfaab55a5d7841917a0fb9a78ccc086ee83`  
		Last Modified: Tue, 21 Dec 2021 02:22:04 GMT  
		Size: 42.1 MB (42116934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feceeddac91e698bf009a378cca3bc65e3bee1199adb92912590e31192ac0437`  
		Last Modified: Tue, 21 Dec 2021 03:20:32 GMT  
		Size: 10.0 MB (9956591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee13a902270fb35c27560bff16e80e54c7122abb938b35cc5188ca753ba23cc`  
		Last Modified: Tue, 21 Dec 2021 03:20:29 GMT  
		Size: 3.9 MB (3921249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cb66d53e7811ef080c8e19ffc98281d9a7e1f083d7f574f6a709b728c2fc01`  
		Last Modified: Tue, 21 Dec 2021 03:21:16 GMT  
		Size: 46.1 MB (46125906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00532520fb2a4106350b26b3efe24eb9105f2b8775d744a041d3d6d54883b448`  
		Last Modified: Tue, 21 Dec 2021 03:23:19 GMT  
		Size: 195.1 MB (195070855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029050c827a8ba3992d61cff7f8714f132c7b9187c5d56756311a5e54924a2f6`  
		Last Modified: Tue, 21 Dec 2021 09:45:47 GMT  
		Size: 4.2 KB (4181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ce2d3b77cbc5fa40bd4d56136d3af1d226f6a7efe3b06fb5bbf5e0ade47f6d`  
		Last Modified: Tue, 21 Dec 2021 10:01:55 GMT  
		Size: 21.7 MB (21721021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a619261d98b896c715a45108359066dacfe9b627f7270eaecb2f227772ec839e`  
		Last Modified: Tue, 21 Dec 2021 10:01:39 GMT  
		Size: 2.3 MB (2323979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbbad6652fa21f40e71150e172d9225276c17f8664c2a87d5611fa6890f6ee1`  
		Last Modified: Tue, 21 Dec 2021 10:01:38 GMT  
		Size: 464.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:12-stretch` - linux; arm64 variant v8

```console
$ docker pull node@sha256:71fe301f9ee8a740131cf50b5e9e9523ac1888a848e8c65a39b23f4812e842d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.8 MB (332775599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3834431a947c21001ad0f499bced0ec409c7f0869b9a0066a48639e928ca1884`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 02 Dec 2021 08:10:09 GMT
ADD file:7be59c7e3b187d010c0e8625e45324f421a21518258e6bd35bab6e0e86c9494c in / 
# Thu, 02 Dec 2021 08:10:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 09:57:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:58:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 09:58:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 09:59:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 00:30:58 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Sat, 18 Dec 2021 04:38:28 GMT
ENV NODE_VERSION=12.22.8
# Sat, 18 Dec 2021 04:39:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Sat, 18 Dec 2021 04:39:04 GMT
ENV YARN_VERSION=1.22.17
# Sat, 18 Dec 2021 04:39:10 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Sat, 18 Dec 2021 04:39:12 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Sat, 18 Dec 2021 04:39:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Dec 2021 04:39:14 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:6965f119641a6f16b55da01b7c12884960366228a181268b0bf7d0b7d50b2336`  
		Last Modified: Thu, 02 Dec 2021 08:44:30 GMT  
		Size: 43.2 MB (43173684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e211a2e7bbb27084e1f8cd62281719dc9d90e3ddb76b862e471b1cde61512cb`  
		Last Modified: Thu, 02 Dec 2021 10:08:36 GMT  
		Size: 10.2 MB (10216757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca410b1e11dc0ad76bc18c383eafa45a44c94916e27e4f327bc75a9373a250ca`  
		Last Modified: Thu, 02 Dec 2021 10:08:34 GMT  
		Size: 3.9 MB (3873863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c7b6f285f6115be3423f6435cf3cb41ad88d3e8e284f342de24037cc5c1824`  
		Last Modified: Thu, 02 Dec 2021 10:08:54 GMT  
		Size: 47.7 MB (47735220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd35086810a2cd2b28d7d530262f916fb20d560f53287127821161c2ee68d9ce`  
		Last Modified: Thu, 02 Dec 2021 10:09:31 GMT  
		Size: 201.8 MB (201765097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75d88af06f71509387690d26be5d6da38be1f4d29ded843ef8c78157e4cffc7`  
		Last Modified: Fri, 03 Dec 2021 00:46:56 GMT  
		Size: 4.1 KB (4085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f94c09efa6cad9033d3373915844eca59a83fa82e6288211a579e8aa01ff48`  
		Last Modified: Sat, 18 Dec 2021 04:51:13 GMT  
		Size: 23.7 MB (23673412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49eaf4785acb7a3a22882f38d7fc478125d580feaa6558ff35c36867948f1e5`  
		Last Modified: Sat, 18 Dec 2021 04:51:09 GMT  
		Size: 2.3 MB (2333018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe27b176924322fc001b77b3384b9c0dbe2866427ab5315f9b5fd538d3282a9f`  
		Last Modified: Sat, 18 Dec 2021 04:51:08 GMT  
		Size: 463.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
