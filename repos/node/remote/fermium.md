## `node:fermium`

```console
$ docker pull node@sha256:ad15a07d80218bf34c31e0bbc4d30efe30e222b84a15cf83957f5e7b3db2187a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `node:fermium` - linux; amd64

```console
$ docker pull node@sha256:3397e2dc4b2b740a4a293c8185af6845f4d1df16cb45a80dd40f82ccdb8cae6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.3 MB (363277076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:903c2c873ea4473a1cc8b272b1015b578068f9dbede6f60e068facaa157a73f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 17 Mar 2022 04:06:37 GMT
ADD file:0d1703dd365e8d6f8625b40addc388cab8f0423af2bca03b0baea5d27f585a9c in / 
# Thu, 17 Mar 2022 04:06:37 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:35:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:35:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Mar 2022 06:36:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:37:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 21:40:00 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 21:52:02 GMT
ENV NODE_VERSION=14.19.1
# Fri, 18 Mar 2022 21:52:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     141F07595B7B3FFE74309A937405533BE57C7D57     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 18 Mar 2022 21:52:42 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 21:52:47 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 18 Mar 2022 21:52:47 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 21:52:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 21:52:47 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:d172ccdc78ea7d453ae5fa3feafee94e3837e6f8e282d8501e668329c49551ed`  
		Last Modified: Thu, 17 Mar 2022 04:13:38 GMT  
		Size: 45.4 MB (45427778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f105b7903980816bf5941ec222e4372a54ab3a577c78837ab69c91736c6a110`  
		Last Modified: Fri, 18 Mar 2022 07:07:26 GMT  
		Size: 11.3 MB (11302667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ae525c10a70b17275982d1dc19125faa52b3dcf3c595e3f7fb2c22e2a11c6d`  
		Last Modified: Fri, 18 Mar 2022 07:07:25 GMT  
		Size: 4.3 MB (4343017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72215048f7839267fc858586027c7c15c3eb397a65da996f6d39d6c3d6844dbb`  
		Last Modified: Fri, 18 Mar 2022 07:07:53 GMT  
		Size: 49.8 MB (49765334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfa9c61a0aba9b870a8482784e81582c09a8cdfe909d598c163ff253d567d48`  
		Last Modified: Fri, 18 Mar 2022 07:08:43 GMT  
		Size: 214.5 MB (214473690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6b791c006f1d92186ef46d1d9c71d27efa55115391f6be885c9d4201fa6814`  
		Last Modified: Fri, 18 Mar 2022 22:08:03 GMT  
		Size: 4.2 KB (4191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6138e26477a6c70e00bbc87608f7ddf891be1b99e49de6bba9394d69df479af8`  
		Last Modified: Fri, 18 Mar 2022 22:15:40 GMT  
		Size: 35.6 MB (35618513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d956a575b58730fbecc07b760c39524754df90d822f15f67e765c6e200a30e`  
		Last Modified: Fri, 18 Mar 2022 22:15:33 GMT  
		Size: 2.3 MB (2341424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac0f5d179f70331a3b8b1937f99389abf75b4870f0758c78d3e95b19731df61`  
		Last Modified: Fri, 18 Mar 2022 22:15:33 GMT  
		Size: 462.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:fermium` - linux; arm variant v7

```console
$ docker pull node@sha256:41d3cd2d2b875dc7b2bfd90974de55999bd6ebd8020e321509d3df237f1ca877
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.3 MB (333273232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e8c792f8df9e857d0789f50ae5da9951ade23c9e054ed6d0e6c3bb93a3e1d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:52 GMT
ADD file:32b09ecc1f1473cc68b2fe74354febc64a9530d26aa83549020fed06caa8ba8b in / 
# Tue, 01 Mar 2022 02:08:53 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 09:37:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 09:37:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 09:38:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 09:41:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 15:20:07 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Tue, 01 Mar 2022 15:37:01 GMT
ENV NODE_VERSION=14.19.0
# Tue, 01 Mar 2022 15:37:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Tue, 01 Mar 2022 15:37:40 GMT
ENV YARN_VERSION=1.22.17
# Tue, 01 Mar 2022 15:37:48 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Tue, 01 Mar 2022 15:37:48 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Tue, 01 Mar 2022 15:37:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 15:37:49 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:57f32f9fdf459a27691c3a29131c270edd06bf53c003de1f42bb0a6ff8824e31`  
		Last Modified: Tue, 01 Mar 2022 02:25:39 GMT  
		Size: 42.1 MB (42116971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e724a8423f66e29c28d1f7eb411c0fc8b5e925a2dba9d9984b26ba548383e5`  
		Last Modified: Tue, 01 Mar 2022 09:59:33 GMT  
		Size: 10.0 MB (9956523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcdac683edae6f35034917112b5fe629e9a55d8911f2afdd7746b8dfba6c1638`  
		Last Modified: Tue, 01 Mar 2022 09:59:30 GMT  
		Size: 3.9 MB (3921197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3159be5381536c8d0bda312974531e6cb3f82099028dc433bb1d7c20c0cd05e`  
		Last Modified: Tue, 01 Mar 2022 10:00:17 GMT  
		Size: 46.1 MB (46127771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b46599bd21a433897c0082a8bb422524e6395ebd461a85fe445b71c57e2224`  
		Last Modified: Tue, 01 Mar 2022 10:02:20 GMT  
		Size: 195.1 MB (195062760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c99c3c044aaf7fbdcf2d06f727b725c0faa1487ecfa15ea4e76d68cfaa421d8`  
		Last Modified: Tue, 01 Mar 2022 16:06:46 GMT  
		Size: 4.2 KB (4176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e893ebe1669b210f430adaa00164d162b3724aa195425c200be546edd7ce4960`  
		Last Modified: Tue, 01 Mar 2022 16:17:36 GMT  
		Size: 33.8 MB (33757656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06aac5bd10441f39d1d9719deeba4913457ee0a2441184d7f3d9bef823f8535c`  
		Last Modified: Tue, 01 Mar 2022 16:17:13 GMT  
		Size: 2.3 MB (2325715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17888aab4b64e02137d1f01f6c8157e42b6941411a0e22edbd36d6b7329ec335`  
		Last Modified: Tue, 01 Mar 2022 16:17:11 GMT  
		Size: 463.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:fermium` - linux; arm64 variant v8

```console
$ docker pull node@sha256:3099506ea46b4b0de39176ebed48d91da35a21638981ebdec10e89245e14c044
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.9 MB (344890463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:255f3f4b2abb58b35e96a412037c3c8c269f9ebd2ec0a6d09e604f3050662ace`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 17 Mar 2022 03:24:02 GMT
ADD file:eb07f8b0889bb0b4499fbba08599cdf04f3efaafdec453e96fa4175723f4fec1 in / 
# Thu, 17 Mar 2022 03:24:03 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:15:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 22:15:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:16:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:02:04 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 18 Mar 2022 09:38:30 GMT
ENV NODE_VERSION=14.19.0
# Fri, 18 Mar 2022 09:39:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     74F12602B6F1C4E913FAA37AD3A89613643B6201     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do       gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||       gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 18 Mar 2022 09:40:01 GMT
ENV YARN_VERSION=1.22.17
# Fri, 18 Mar 2022 09:40:07 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$key" ||     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 18 Mar 2022 09:40:09 GMT
COPY file:4d192565a7220e135cab6c77fbc1c73211b69f3d9fb37e62857b2c6eb9363d51 in /usr/local/bin/ 
# Fri, 18 Mar 2022 09:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 09:40:11 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:0d6ecff05d590b97ebc357d19bd439c17d4142359ceceb25dda468284e978583`  
		Last Modified: Thu, 17 Mar 2022 03:32:27 GMT  
		Size: 43.2 MB (43213043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf8187d7f23f7722584cf9a7359b8e6859ca891c112d0398819cecdac7fa008`  
		Last Modified: Thu, 17 Mar 2022 22:24:30 GMT  
		Size: 10.2 MB (10217652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9ad8247187d77aea7d1a40486c48551a68a63e2b6be93a43c47cc27d726beb`  
		Last Modified: Thu, 17 Mar 2022 22:24:29 GMT  
		Size: 3.9 MB (3874519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b13fc30419a0a45924b8386c468bbaf3f0ba8ebcfe179f82d46e2317ff28066`  
		Last Modified: Thu, 17 Mar 2022 22:24:48 GMT  
		Size: 47.7 MB (47735576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e9503348f7f70fb00c6b14f28af508a9f91c54d3ded7864c44ad947e9b6c14`  
		Last Modified: Thu, 17 Mar 2022 22:25:25 GMT  
		Size: 201.8 MB (201793625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8bef0856eadb995b1c0c33b992e5c02cba24cbed97255d7fff43bb98357eca`  
		Last Modified: Fri, 18 Mar 2022 10:10:28 GMT  
		Size: 4.1 KB (4086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee0f4c12cf5e92863791a6c53f4a6a63b308578bde714377b1097b57711cd7f`  
		Last Modified: Fri, 18 Mar 2022 10:18:19 GMT  
		Size: 35.7 MB (35717915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b390e03cdb617bf01e76ced400a7ea8d4f40c64d53371909aaae28e2a99fbc7`  
		Last Modified: Fri, 18 Mar 2022 10:18:13 GMT  
		Size: 2.3 MB (2333584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff23fd40b8c4925b62d167805ab75a9406ac7d9c0ebb6c00d906aecfbcc3b94`  
		Last Modified: Fri, 18 Mar 2022 10:18:13 GMT  
		Size: 463.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
