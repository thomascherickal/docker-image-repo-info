## `node:current`

```console
$ docker pull node@sha256:b862ecc842609196fbd32b767ddb0c28aa5769465be5074e46bba14d1a4e3b25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `node:current` - linux; amd64

```console
$ docker pull node@sha256:0d53bb9b0e4131544940a7bf260db1838a592311664586ad97585ecfa8961363
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.0 MB (361965010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a23e6f36bbcfa64edcfe9966edc69c995366e6a091d0bf30f035b6e63fbddeb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 10 Sep 2020 00:30:04 GMT
ADD file:d8d46fb9e0436b304449f4155e3b1a86d8fdfd809364286726e5b33746db53c0 in / 
# Thu, 10 Sep 2020 00:30:05 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:11:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:11:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:11:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:12:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 12:37:14 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Thu, 10 Sep 2020 12:37:14 GMT
ENV NODE_VERSION=14.10.0
# Thu, 10 Sep 2020 12:37:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Thu, 10 Sep 2020 12:37:23 GMT
ENV YARN_VERSION=1.22.5
# Thu, 10 Sep 2020 12:37:26 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Thu, 10 Sep 2020 12:37:27 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Thu, 10 Sep 2020 12:37:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 12:37:27 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:4f250268ed6a0b777b9a3d9e0659754a8c97f28420f30cb78c184c3eead07d14`  
		Last Modified: Thu, 10 Sep 2020 00:37:25 GMT  
		Size: 45.4 MB (45366726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b49aa113642e1d83773ca83de882e12c4981ed565d47b4c7da998855ad182e1`  
		Last Modified: Thu, 10 Sep 2020 01:19:16 GMT  
		Size: 10.8 MB (10750802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159512f4cc2a5f8c64890a32b7766e2662b61241ef585cc28daf194bccaf1c1`  
		Last Modified: Thu, 10 Sep 2020 01:19:14 GMT  
		Size: 4.3 MB (4340512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8439168fd8dcb35b71c06211b4c23c02bd846e1d37f72cfe5638ada30c196556`  
		Last Modified: Thu, 10 Sep 2020 01:19:35 GMT  
		Size: 50.1 MB (50109858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55abbc6cc15820e59f3f9effd6987da17f809be3666d5db2c7ccb5795f8b35ed`  
		Last Modified: Thu, 10 Sep 2020 01:20:31 GMT  
		Size: 214.3 MB (214254178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c5821cd8891e4cb78b57e971882385cf3d9541a6071c9ae64263c7ed8152b4`  
		Last Modified: Thu, 10 Sep 2020 12:45:55 GMT  
		Size: 4.2 KB (4169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9f91ab325e36461d0df9fe78945252aed8862d853e3feab787e817b1369db3`  
		Last Modified: Thu, 10 Sep 2020 12:46:04 GMT  
		Size: 34.8 MB (34776490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35b4f289c8c1c5fd28b3bf1aaeac2194c809074f5a484832a20011e16c11296`  
		Last Modified: Thu, 10 Sep 2020 12:45:56 GMT  
		Size: 2.4 MB (2361983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd9e558de13c397f65888761071731264a19140bbcbf8e7f11d6b31da8c5e2d`  
		Last Modified: Thu, 10 Sep 2020 12:45:55 GMT  
		Size: 292.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:current` - linux; arm variant v7

```console
$ docker pull node@sha256:9310eee22219aa72beb807d62d800f3ea1487cbe6a95b2f0f8499ddaeb893353
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.2 MB (332158697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d673a4c4dcd589380f4703c598f949136c8eba93e4bfe68cf56b18dd8e76c759`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Thu, 10 Sep 2020 00:13:17 GMT
ADD file:3da15ca153ab01cc777bb2a828e1097edc064f49012d96e9b0789cc4cbe9c205 in / 
# Thu, 10 Sep 2020 00:13:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:54:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:55:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:58:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 07:53:56 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 11 Sep 2020 00:17:25 GMT
ENV NODE_VERSION=14.10.1
# Fri, 11 Sep 2020 00:17:39 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 11 Sep 2020 00:17:41 GMT
ENV YARN_VERSION=1.22.5
# Fri, 11 Sep 2020 00:17:47 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 11 Sep 2020 00:17:48 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Fri, 11 Sep 2020 00:17:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 00:17:50 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:2dc31d01bd52bc4550017dd5cb9e295a7998fbfa6b3ea3f612efb5da666b3600`  
		Last Modified: Thu, 10 Sep 2020 00:21:14 GMT  
		Size: 42.1 MB (42111430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f054c3bb715838c3b5b7a1b87d44bb27e66b730c6f46043718676fd2b5f82a9`  
		Last Modified: Thu, 10 Sep 2020 02:05:53 GMT  
		Size: 9.4 MB (9443974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7852e0ac40ce276d38d43909de6fc6e0283548a22510dba9ed39e9c093895f`  
		Last Modified: Thu, 10 Sep 2020 02:05:52 GMT  
		Size: 3.9 MB (3919884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee36d6b27968e04921e9febd754fab4304b42cd2a81762078e12818d8103e04`  
		Last Modified: Thu, 10 Sep 2020 02:06:17 GMT  
		Size: 46.4 MB (46413983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8a29d5e049b55a7bc0c5923b6a4015cf8efe9bbb01620f16f40b715dc1f4f5`  
		Last Modified: Thu, 10 Sep 2020 02:07:15 GMT  
		Size: 194.9 MB (194897269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e71e03509b2ff9726deb1a1be415611d197dd54c8201604174cf4473a7f7e0`  
		Last Modified: Thu, 10 Sep 2020 08:18:46 GMT  
		Size: 4.2 KB (4179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7f46ae94b06fbff8a8b6b31dd76539451cefcf5c17e6676f31e5c8526ad637`  
		Last Modified: Fri, 11 Sep 2020 00:40:25 GMT  
		Size: 33.0 MB (33016356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bc7d95c8600d134235ed251bd83f536b89128f9f5042c0269f34a2e78527d4`  
		Last Modified: Fri, 11 Sep 2020 00:39:58 GMT  
		Size: 2.4 MB (2351326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09a1d129b5e8ba65f625688ccd6a76a29f4f8e350a3f21667f018f2bf99f0bb`  
		Last Modified: Fri, 11 Sep 2020 00:39:57 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `node:current` - linux; arm64 variant v8

```console
$ docker pull node@sha256:cd7635de252fdaa03898bb5bd84f63516c34abf35baf3a5b12eacb1e30b64d02
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.9 MB (343887370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83b42bca649ac5d97818364c898b2d9fccc90db801b190421823f2eb4b1bbe2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["node"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:23 GMT
ADD file:f74bb8d38ef70a022988428f254630d1f424ed9a3b957687b0cd0f85b9d49e29 in / 
# Wed, 09 Sep 2020 23:54:25 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:35:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:36:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:38:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 10:14:04 GMT
RUN groupadd --gid 1000 node   && useradd --uid 1000 --gid node --shell /bin/bash --create-home node
# Fri, 11 Sep 2020 01:33:07 GMT
ENV NODE_VERSION=14.10.1
# Fri, 11 Sep 2020 01:33:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)"   && case "${dpkgArch##*-}" in     amd64) ARCH='x64';;     ppc64el) ARCH='ppc64le';;     s390x) ARCH='s390x';;     arm64) ARCH='arm64';;     armhf) ARCH='armv7l';;     i386) ARCH='x86';;     *) echo "unsupported architecture"; exit 1 ;;   esac   && set -ex   && for key in     4ED778F539E3634C779C87C6D7062848A1AB005C     94AE36675C464D64BAFA68DD7434390BDBE9B9C5     71DCFD284A79C3B38668286BC97EC7A07EDE3FC1     8FCCA13FEF1D0C2E91008E09770F7A9A5AE15600     C4F0DFFF4E8C1A8236409D08E73BC641CC11F4C8     C82FA3AE1CBEDC6BE46B9360C43CEC45C17AB93C     DD8F2338BAE7501E3DD5AC78C273792F7D83545D     A48C2BEE680E841632CD4E44F07496B3EB3C1762     108F52B48DB57BB0CC439B2997B01419BD92F80A     B9E2F5981AA6E0CD28160D9FF13993A75599653C   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/node-v$NODE_VERSION-linux-$ARCH.tar.xz"   && curl -fsSLO --compressed "https://nodejs.org/dist/v$NODE_VERSION/SHASUMS256.txt.asc"   && gpg --batch --decrypt --output SHASUMS256.txt SHASUMS256.txt.asc   && grep " node-v$NODE_VERSION-linux-$ARCH.tar.xz\$" SHASUMS256.txt | sha256sum -c -   && tar -xJf "node-v$NODE_VERSION-linux-$ARCH.tar.xz" -C /usr/local --strip-components=1 --no-same-owner   && rm "node-v$NODE_VERSION-linux-$ARCH.tar.xz" SHASUMS256.txt.asc SHASUMS256.txt   && ln -s /usr/local/bin/node /usr/local/bin/nodejs   && node --version   && npm --version
# Fri, 11 Sep 2020 01:33:22 GMT
ENV YARN_VERSION=1.22.5
# Fri, 11 Sep 2020 01:33:28 GMT
RUN set -ex   && for key in     6A010C5166006599AA17F08146C2130DFD2497F5   ; do     gpg --batch --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys "$key" ||     gpg --batch --keyserver hkp://ipv4.pool.sks-keyservers.net --recv-keys "$key" ||     gpg --batch --keyserver hkp://pgp.mit.edu:80 --recv-keys "$key" ;   done   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz"   && curl -fsSLO --compressed "https://yarnpkg.com/downloads/$YARN_VERSION/yarn-v$YARN_VERSION.tar.gz.asc"   && gpg --batch --verify yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && mkdir -p /opt   && tar -xzf yarn-v$YARN_VERSION.tar.gz -C /opt/   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarn /usr/local/bin/yarn   && ln -s /opt/yarn-v$YARN_VERSION/bin/yarnpkg /usr/local/bin/yarnpkg   && rm yarn-v$YARN_VERSION.tar.gz.asc yarn-v$YARN_VERSION.tar.gz   && yarn --version
# Fri, 11 Sep 2020 01:33:29 GMT
COPY file:238737301d47304174e4d24f4def935b29b3069c03c72ae8de97d94624382fce in /usr/local/bin/ 
# Fri, 11 Sep 2020 01:33:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 01:33:30 GMT
CMD ["node"]
```

-	Layers:
	-	`sha256:3b396f138ad78ffceac749b105c676dce568fa15a7b9f2273c2ee13ba023cea1`  
		Last Modified: Thu, 10 Sep 2020 00:01:33 GMT  
		Size: 43.2 MB (43171697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5db606bd1ccd8d11ca18492ee5d5122fdae2e7172ceb0df9cd15dc4d9f3c259`  
		Last Modified: Thu, 10 Sep 2020 00:45:55 GMT  
		Size: 9.7 MB (9700841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd3b5402f1859618a8e455e6bf04a916c8460da1c5f115568ba530c96f6ba3`  
		Last Modified: Thu, 10 Sep 2020 00:45:52 GMT  
		Size: 4.1 MB (4095176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb81e51c7d923c71bc53fedd00e3247cbe38545e27848eb452110320aedf641`  
		Last Modified: Thu, 10 Sep 2020 00:46:19 GMT  
		Size: 48.0 MB (48044000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6077cb8785bbbed8f14fef78ee07d648b12216bfc6551532fd1029138ffce0d9`  
		Last Modified: Thu, 10 Sep 2020 00:47:20 GMT  
		Size: 201.6 MB (201623831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10459ed06a37221dbcbe6039ddce6da2562d6ef27bfecfb4f879c180469af2c`  
		Last Modified: Thu, 10 Sep 2020 10:32:05 GMT  
		Size: 4.2 KB (4201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e05a941ff205a9c3f59a7cdd9a66e6a7b9853738b29fad3e4a815dfb700b2fe`  
		Last Modified: Fri, 11 Sep 2020 02:00:09 GMT  
		Size: 34.9 MB (34885371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f3e9677be6bdb6c17fe0b6513841beda2be5cb3957dedf551de4a979d5331e`  
		Last Modified: Fri, 11 Sep 2020 01:59:51 GMT  
		Size: 2.4 MB (2361958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c8ff70ca6857172c9618e6d273e218f6befbbd099cf8130277a61da5b065b8`  
		Last Modified: Fri, 11 Sep 2020 01:59:50 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
