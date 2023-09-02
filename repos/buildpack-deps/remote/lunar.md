## `buildpack-deps:lunar`

```console
$ docker pull buildpack-deps@sha256:42b399503c94a281a93e719d42f84b3f325236ae4a702588270239bd8273f38c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1a5c5e7cb1d0b8121f6af03e5d81b2903f193eff7d9d8680767bfd31587cc9a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268569702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddcddba17812f7b0067d772977bf987dba5a1298b2cf5249d50ea340bc08ec0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:28:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:28:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:28:32 GMT
ADD file:7392bed4dbab9fb7c9ad5bde6f3bfcde3bcbf1885c336af9c231af6defaa31e1 in / 
# Wed, 16 Aug 2023 04:28:33 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:03:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:04:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:07:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05cdbc478740a42a5ebb092eefd6fc221933f796ee343c49cb920ee60025bab8`  
		Last Modified: Sat, 02 Sep 2023 00:12:48 GMT  
		Size: 27.7 MB (27651898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea73fe152c7c1b43c8962bdf8054f83c720b0d6251821ccf461eef843531c42`  
		Last Modified: Sat, 02 Sep 2023 00:12:47 GMT  
		Size: 13.7 MB (13744690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e8d218b3d1561b5d122cd9db4c10b2fa28d00a9d62a5fa468005767a3c57ad`  
		Last Modified: Sat, 02 Sep 2023 00:13:03 GMT  
		Size: 44.4 MB (44386354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1579db9ae1a076a64156b02ae82feb2f9ce83e2e9b3b34ac15a03af76804c4fb`  
		Last Modified: Sat, 02 Sep 2023 00:13:36 GMT  
		Size: 182.8 MB (182786760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d6ea0b47ff94fd43214fdbd375e76439c8e482c0e2c23a5689a77ccefbbb1914
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232402102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:481c72f11a0bc3f30e41361cfa3dd8e82a21af43aa0ae32812af60475b4e626e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:11 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:16 GMT
ADD file:1f1c9502544acdbb6a7450226ced78cfe982a6305f2aea77ab7d1f73b50fc7f0 in / 
# Wed, 16 Aug 2023 04:16:16 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:45:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:49:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9fce615a928dd3a3068e1de48019af925a9120537cb22174bef3b5bc6c81aa30`  
		Last Modified: Fri, 01 Sep 2023 23:55:36 GMT  
		Size: 25.4 MB (25429153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226718c385cfaf19fd9705f67eadf089cc077b99eacfccbae1ec6906f4cdfcbc`  
		Last Modified: Fri, 01 Sep 2023 23:55:34 GMT  
		Size: 12.7 MB (12664290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0762989993ef4516781509cf1b0ef7cbb69316eb39606703587e43c2d4339752`  
		Last Modified: Fri, 01 Sep 2023 23:55:52 GMT  
		Size: 48.7 MB (48671689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf6327fba60d1befcc2cfc5794210eba5c425fedcbb218b33f976d848c72516`  
		Last Modified: Fri, 01 Sep 2023 23:56:20 GMT  
		Size: 145.6 MB (145636970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c35cff9ee39e8ccefb8a64cf70c0d70fe38ccd97a73096d01f7830df0bd5395b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258101641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:838c33af0279b9480fe0ff02a8e940444b7d1af54825a3243b58b9aad7a6c766`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:15:57 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:15:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:15:57 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:01 GMT
ADD file:adea2962926b29b76eb8da76ae9e830c5ad7050ae9b19f5427191b338c8a2c56 in / 
# Wed, 16 Aug 2023 04:16:02 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:17:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:17:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:21:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b3bb2adde9f4704b6cbca4cd0cd3d0035b2dbab8b3cc6fe17ec006b386e1ebd`  
		Last Modified: Fri, 01 Sep 2023 23:26:49 GMT  
		Size: 27.0 MB (27006213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cd1935e47d8915d0f0ab87a4d0c823b0c698145c21215e144b766365ffd8c3`  
		Last Modified: Fri, 01 Sep 2023 23:26:48 GMT  
		Size: 13.3 MB (13333801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2c77b1d5d537e25307eba90cccef89858a69e1a468e51d157eab0cce01dc9f`  
		Last Modified: Fri, 01 Sep 2023 23:27:02 GMT  
		Size: 44.2 MB (44235660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3251e45b821cec25f5abb11d43083d605c727b98be2b71576bf18a39010c51`  
		Last Modified: Fri, 01 Sep 2023 23:27:29 GMT  
		Size: 173.5 MB (173525967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e3108463e296ffe459ea82aa555c65cc845d282c08c133cbc3c89b478efebeed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.0 MB (293045547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f528798424c0d5cbae974a62b5d3633cb2e55806c2fc356882a9bb10757052d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:18:51 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:18:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:18:54 GMT
ADD file:98fe279e3c3239702ac2eef51540228e24a3e15e923342cb3e7cd7dd3684a090 in / 
# Mon, 31 Jul 2023 17:18:54 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:32:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:38:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8f1d2c62b1aacc6f999b01ed9c6ef10bc5fd3a989af86649162cf5292934393`  
		Last Modified: Thu, 03 Aug 2023 03:51:49 GMT  
		Size: 32.0 MB (32013471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1b07037748833f21cbeb83084ac8ff4a0ca93e61d3e0ac3914daf1beac24`  
		Last Modified: Thu, 03 Aug 2023 03:51:45 GMT  
		Size: 15.8 MB (15842395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e1c2370aa8951d8926c5924bcf24547ca74703904b0527c7f23e46740815f0`  
		Last Modified: Thu, 03 Aug 2023 03:52:13 GMT  
		Size: 49.1 MB (49086146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa281b8d2db730035bc9fca050c2d962532df63e59ee2bf70160dc162d8fc5e`  
		Last Modified: Thu, 03 Aug 2023 03:53:10 GMT  
		Size: 196.1 MB (196103535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b03c2d5655663b83f6a221f35784d8902b4af4751413f0a874d38b81c25573ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240157223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df5b35e4a07ed4da761b7644d6c49ad1a8694b981e74aaff067b260dec6c54a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:16:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:19:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9a6157a42893e6f99bd42ba05c70c5313add95c69f61f12e51517c0100470b8`  
		Last Modified: Fri, 01 Sep 2023 23:24:13 GMT  
		Size: 26.2 MB (26223925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f88ef015543162519d8e086a0bb86351d03f27b98218ff39b27f3b8b7bc2cd`  
		Last Modified: Fri, 01 Sep 2023 23:24:12 GMT  
		Size: 14.0 MB (14005753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad80a5cffb7414f3bd06d5dafc212e2f5a767d3312bead7347e2ba8fae5be35`  
		Last Modified: Fri, 01 Sep 2023 23:24:25 GMT  
		Size: 44.3 MB (44275476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f495142834cd7cf92ea01d1b100c2b74a416627d5613eefc2c858d2b4c774d2`  
		Last Modified: Fri, 01 Sep 2023 23:24:50 GMT  
		Size: 155.7 MB (155652069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
